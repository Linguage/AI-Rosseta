
# 智能体
「Google白皮书」智能体（Agent）
- 单位：Google
- 作者：Julia Wiesinger, Patrick Marlow 和 Vladimir Vuskovic
- 原文：[Agent](https://www.kaggle.com/whitepaper-agents)

![](https://cdn-mineru.openxlab.org.cn/extract/7b099934-d40b-403d-8804-2269062d890e/1e617186aa14acffc2355bf30615e8ccb40d24be539626e598f7d93f16c094df.jpg)



## 目录
```
1. 引言 4
2. 什么是智能体？ 5
3. 模型 6
4. 工具 7
5. 编排层 7
6. 智能体 vs. 模型 8
7. 认知架构：智能体如何运作 8
8. 工具：我们通往外部世界的钥匙 12
9. 扩展 13
10. 扩展示例 15
11. 函数 18
12. 用例 21
13. 函数示例代码 24
14. 数据存储 27
15. 实现与应用 28
16. 工具回顾 32
17. 通过目标学习提升模型性能 33
18. 使用 LangChain 快速开始智能体开发 35
19. 使用 Vertex AI 智能体进行生产应用 38
20. 总结 40
21. 尾注 42
```


这种将推理、逻辑和对外部信息的访问结合起来，并全部连接到生成式 AI 模型的方式，引出了智能体的概念。

# 引言

人类非常擅长处理混乱的模式识别任务。然而，在得出结论之前，他们通常依赖书籍、Google 搜索或计算器等工具来补充先前的知识。与人类一样，生成式 AI 模型也可以被训练使用工具来访问实时信息或建议现实世界的行动。例如，模型可以利用数据库检索工具访问特定信息，如客户的购买历史，以便生成量身定制的购物推荐。或者，根据用户的查询，模型可以进行各种 API 调用，代表您向同事发送电子邮件回复或完成金融交易。为此，模型不仅需要访问一组外部工具，还需要具备以自我导向的方式规划和执行任何任务的能力。这种将推理、逻辑和对外部信息的访问结合起来，并全部连接到生成式 AI 模型的方式，引出了智能体（Agent）的概念，即一个超越了独立生成式 AI 模型能力的程序。本白皮书将更详细地探讨所有这些及相关方面。

## 什么是智能体？

在其最基本的形式中，生成式 AI 智能体可以定义为一个应用程序，它试图通过观察世界并使用其可用的工具对其采取行动来达到目标。智能体是自主的，可以在没有人为干预的情况下独立行动，尤其是在为其设定了明确的目标或要实现的目的时。智能体在实现目标的方法上也可以是主动的。即使在没有人类明确指令集的情况下，智能体也可以推理出下一步应该做什么来实现其最终目标。虽然 AI 中智能体的概念非常普遍且强大，但本白皮书侧重于发布时生成式 AI 模型能够构建的特定类型的智能体。

为了理解智能体的内部工作原理，让我们首先介绍驱动智能体行为、行动和决策的基础组件。这些组件的组合可以描述为一个认知架构，通过混合和匹配这些组件可以实现许多这样的架构。关注核心功能，智能体的认知架构中有三个基本组件，如图 1 所示。

![](https://cdn-mineru.openxlab.org.cn/extract/7b099934-d40b-403d-8804-2269062d890e/84926dd6c958870f1d39d138e0b8752636fb1c816080558319cce62629158ea1.jpg)
图 1. 通用智能体架构和组件

### 模型

在智能体的范围内，模型指的是将用作智能体过程的中心决策者的语言模型（LM）。智能体使用的模型可以是一个或多个任何大小（小型/大型）的语言模型，这些模型能够遵循基于指令的推理和逻辑框架，如 ReAct、思维链（Chain-of-Thought）或思维树（Tree-of-Thoughts）。模型可以是通用的、多模态的或根据特定智能体架构的需求进行微调的。为了获得最佳的生产结果，您应该利用最适合您期望的最终应用程序的模型，并且理想情况下，该模型已经在与您计划在认知架构中使用的工具相关的数据特征上进行了训练。需要注意的是，模型通常不会针对智能体的特定配置设置（例如工具选择、编排/推理设置）进行训练。但是，可以通过向模型提供展示智能体能力的示例（包括智能体在各种上下文中使用特定工具或推理步骤的实例）来进一步为智能体的任务优化模型。

### 工具

基础模型尽管在文本和图像生成方面表现出色，但仍然受到无法与外部世界互动的限制。工具弥合了这一差距，使智能体能够与外部数据和服务交互，同时解锁了超越底层模型本身的更广泛行动范围。工具可以采取多种形式，并具有不同的复杂程度，但通常与常见的 Web API 方法（如 GET、POST、PATCH 和 DELETE）保持一致。例如，工具可以更新数据库中的客户信息或获取天气数据以影响智能体向用户提供的旅行建议。借助工具，智能体可以访问和处理现实世界的信息。这使它们能够支持更专业的系统，如检索增强生成（RAG），这显著扩展了智能体的能力，超越了基础模型本身所能达到的水平。我们将在下面更详细地讨论工具，但最重要的是要理解工具弥合了智能体内部能力与外部世界之间的差距，解锁了更广泛的可能性。

### 编排层

编排层描述了一个循环过程，该过程管理智能体如何接收信息、执行一些内部推理，并使用该推理来指导其下一步行动或决策。通常，这个循环将持续进行，直到智能体达到其目标或某个停止点。编排层的复杂性可能因智能体及其执行的任务而有很大差异。一些循环可以是带有决策规则的简单计算，而另一些则可能包含链式逻辑、涉及额外的机器学习算法或实现其他概率推理技术。我们将在认知架构部分更详细地讨论智能体编排层的具体实现。

### 智能体 vs. 模型

为了更清楚地理解智能体和模型之间的区别，请参考下表：

<html><body><table><tr><td>模型</td><td>智能体</td></tr><tr><td>知识仅限于其训练数据中可用的内容。</td><td>通过工具与外部系统连接来扩展知识。</td></tr><tr><td>基于用户查询的单次推理/预测。除非为模型明确实现，否则没有会话历史或连续上下文的管理（例如聊天历史记录）。</td><td>管理的会话历史（例如聊天历史记录），允许基于用户查询和编排层中做出的决策进行多轮推理/预测。在此上下文中，“轮”定义为交互系统与智能体之间的一次交互（例如，1 个传入事件/查询和 1 个智能体响应）。</td></tr><tr><td>没有原生工具实现。</td><td>工具在智能体架构中原生实现。</td></tr><tr><td>没有实现原生逻辑层。用户可以将提示表述为简单问题，或使用推理框架（CoT、ReAct 等）形成复杂提示来指导模型进行预测。</td><td>使用 CoT、ReAct 等推理框架或 LangChain 等其他预构建智能体框架的原生认知架构。</td></tr></table></body></html>

### 认知架构：智能体如何运作

想象一下繁忙厨房里的厨师。他们的目标是为餐厅顾客制作美味佳肴，这涉及规划、执行和调整的某种循环。

*   他们收集信息，例如顾客的订单以及食品储藏室和冰箱里有哪些食材。
*   他们根据刚刚收集到的信息，对可以制作的菜肴和风味进行一些内部推理。
*   他们采取行动制作菜肴：切蔬菜、混合香料、煎肉。

在过程的每个阶段，厨师都会根据需要进行调整，随着食材耗尽或收到客户反馈而完善他们的计划，并使用先前结果集来确定下一个行动计划。这种信息接收、规划、执行和调整的循环描述了厨师为实现其目标所采用的独特认知架构。

就像厨师一样，智能体可以使用认知架构，通过迭代处理信息、做出明智决策以及根据先前输出完善下一步行动来达到其最终目标。智能体认知架构的核心是编排层，负责维护记忆、状态、推理和规划。它利用快速发展的提示工程领域及相关框架来指导推理和规划，使智能体能够更有效地与其环境互动并完成任务。语言模型的提示工程框架和任务规划领域的研究正在迅速发展，产生了各种有前途的方法。虽然不是详尽的列表，但以下是本出版物发布时一些最流行的框架和推理技术：

*   ReAct：一种提示工程框架，为语言模型提供了一种思考过程策略，用于对用户查询进行推理（Reason）和采取行动（Action），无论是否有上下文示例。ReAct 提示已被证明优于几种 SOTA 基线，并提高了 LLM 的人类互操作性和可信赖度。
*   思维链（CoT）：一种提示工程框架，通过中间步骤实现推理能力。CoT 有多种子技术，包括自洽性（self-consistency）、主动提示（active-prompt）和多模态 CoT，每种技术根据具体应用都有其优缺点。
*   思维树（ToT）：一种提示工程框架，非常适合探索或战略前瞻任务。它泛化了思维链提示，并允许模型探索各种思维链，这些思维链作为使用语言模型解决一般问题的中间步骤。

智能体可以利用上述推理技术之一或许多其他技术来为给定的用户请求选择下一个最佳行动。例如，让我们考虑一个被编程为使用 ReAct 框架为用户查询选择正确行动和工具的智能体。事件序列可能如下所示：

1.  用户向智能体发送查询。
2.  智能体开始 ReAct 序列。
3.  智能体向模型提供提示，要求其生成下一个 ReAct 步骤及其对应的输出：
    a.  问题：来自用户查询的输入问题，随提示提供。
    b.  思考：模型关于下一步应该做什么的想法。
    c.  行动：模型决定下一步采取什么行动。
        i.  这里可能发生工具选择。
        ii. 例如，一个行动可以是 [Flights, Search, Code, None] 中的一个，其中前 3 个代表模型可以选择的已知工具，最后一个代表“无工具选择”。
    d.  行动输入：模型决定向工具提供什么输入（如果有的话）。
    e.  观察：行动/行动输入序列的结果。
        i.  这个思考/行动/行动输入/观察序列可以根据需要重复 N 次。
    f.  最终答案：模型提供给原始用户查询的最终答案。
4.  ReAct 循环结束，最终答案返回给用户。

![](https://cdn-mineru.openxlab.org.cn/extract/7b099934-d40b-403d-8804-2269062d890e/bffed5a0602be449eda387d3797146d1c100fb292d00f8fc288875cd8d654545.jpg)
图 2. 在编排层中使用 ReAct 推理的智能体示例

如图 2 所示，模型、工具和智能体配置协同工作，根据用户的原始查询向用户提供有根据、简洁的响应。虽然模型本可以根据其先验知识猜测（幻觉）一个答案，但它使用了工具（Flights）来搜索实时的外部信息。这些额外的信息被提供给模型，使其能够基于真实的 factual 数据做出更明智的决策，并将这些信息总结给用户。

总之，智能体响应的质量直接关系到模型对这些各种任务进行推理和行动的能力，包括选择正确工具的能力，以及该工具被定义的程度。就像厨师用新鲜食材精心制作菜肴并关注顾客反馈一样，智能体依靠合理的推理和可靠的信息来提供最佳结果。在下一节中，我们将深入探讨智能体连接新鲜数据的各种方式。

## 工具：我们通往外部世界的钥匙

虽然语言模型擅长处理信息，但它们缺乏直接感知和影响现实世界的能力。这限制了它们在需要与外部系统或数据交互的情况下的用用性。这意味着，在某种意义上，语言模型的好坏取决于它从训练数据中学到的知识。但无论我们向模型投入多少数据，它们仍然缺乏与外部世界互动的基本能力。那么，我们如何才能让我们的模型与外部系统进行实时、具有上下文感知的交互呢？函数（Functions）、扩展（Extensions）、数据存储（Data Stores）和插件（Plugins）都是为模型提供这种关键能力的方式。

虽然它们有许多名称，但工具是连接我们的基础模型与外部世界的纽带。这种与外部系统和数据的连接使我们的智能体能够执行更广泛的任务，并且更准确、更可靠地完成这些任务。例如，工具可以使智能体调整智能家居设置、更新日历、从数据库中获取用户信息，或根据一组特定的指令发送电子邮件。

截至本出版物发布之日，Google 模型能够与之交互的主要工具类型有三种：扩展（Extensions）、函数（Functions）和数据存储（Data Stores）。通过为智能体配备工具，我们释放了它们不仅能理解世界，还能对其采取行动的巨大潜力，为无数新的应用和可能性打开了大门。

### 扩展 (Extensions)

理解扩展最简单的方法是将它们视为以标准化方式弥合 API 和智能体之间差距的桥梁，允许智能体无缝执行 API，而不管其底层实现如何。假设您构建了一个旨在帮助用户预订航班的智能体。您知道想要使用 Google Flights API 来检索航班信息，但不确定如何让您的智能体调用此 API 端点。

![](https://cdn-mineru.openxlab.org.cn/extract/7b099934-d40b-403d-8804-2269062d890e/79c5ef7bc54f939d5d51eb54330c181f97abe1665855fc595b04af3ed5b9a6b2.jpg)
图 3. 智能体如何与外部 API 交互？

一种方法是实现自定义代码，该代码将接收传入的用户查询，解析查询以获取相关信息，然后进行 API 调用。例如，在航班预订用例中，用户可能会说“我想预订从奥斯汀到苏黎世的航班。”在这种情况下，我们的自定义代码解决方案需要从用户查询中提取“奥斯汀”和“苏黎世”作为相关实体，然后才能尝试进行 API 调用。但是，如果用户说“我想预订去苏黎世的航班”并且从未提供出发城市，会发生什么？API 调用将在没有所需数据的情况下失败，并且需要实现更多代码来捕获此类边缘和极端情况。这种方法不可扩展，并且在任何超出已实现自定义代码范围的情况下都很容易崩溃。

一种更具弹性的方法是使用扩展。扩展通过以下方式弥合了智能体和 API 之间的差距：

1.  使用示例教智能体如何使用 API 端点。
2.  教智能体成功调用 API 端点需要哪些参数。

![](https://cdn-mineru.openxlab.org.cn/extract/7b099934-d40b-403d-8804-2269062d890e/8f094e4e8bd23c2e5cc1eddd2a9ed8f543a15661f7b1fa5806975bf91aa9b3f2.jpg)
图 4. 扩展连接智能体与外部 API

扩展可以独立于智能体制作，但应作为智能体配置的一部分提供。智能体在运行时使用模型和示例来决定哪个扩展（如果有）适合解决用户的查询。这突显了扩展的一个关键优势，即其内置的示例类型，允许智能体动态选择最适合任务的扩展。

![](https://cdn-mineru.openxlab.org.cn/extract/7b099934-d40b-403d-8804-2269062d890e/8f3dd21d88359a2aa3bf116715eccbadb3bff0830c4dbc5d1495497e5310e94d.jpg)
图 5. 智能体、扩展和 API 之间的一对多关系

可以将其视为软件开发人员在为用户问题进行解决方案设计时决定使用哪些 API 端点的方式。如果用户想预订航班，开发人员可能会使用 Google Flights API。如果用户想知道离他们位置最近的咖啡店在哪里，开发人员可能会使用 Google Maps API。以同样的方式，智能体/模型堆栈使用一组已知的扩展来决定哪一个最适合用户的查询。如果您想看到扩展的实际应用，可以在 Gemini 应用程序中尝试它们，方法是转到“设置”>“扩展”，然后启用您想要测试的任何扩展。例如，您可以启用 Google Flights 扩展，然后询问 Gemini “显示下周五从奥斯汀到苏黎世的航班。”

#### 扩展示例

为了简化扩展的使用，Google 提供了一些开箱即用的扩展，可以快速导入到您的项目中，并以最少的配置使用。例如，代码片段 1 中的代码解释器扩展允许您通过自然语言描述生成并运行 Python 代码。

```python
import vertexai
import pprint

# 修正：使用标准的变量赋值
PROJECT_ID = "YOUR_PROJECT_ID"
REGION = "us-central1"

vertexai.init(project=PROJECT_ID, location=REGION)

from vertexai.preview.extensions import Extension

# 修正：使用标准的变量赋值
extension_code_interpreter = Extension.from_hub("code_interpreter")

# 修正：使用标准的变量赋值。翻译注释内容。
# CODE_QUERY = """Write a python method to invert a binary tree in O(n) time."""
CODE_QUERY = """编写一个 Python 方法，以 O(n) 时间复杂度反转二叉树。"""

# 修正：使用标准的变量赋值
response = extension_code_interpreter.execute(
    operation_id="generate_and_execute",
    operation_params={"query": CODE_QUERY}
)

print("生成的代码:")
# 修正：确保打印的是正确的字段，这里假设 response 字典中有 'generated_code' 键
# 注意：pprint.pprint({...}) 会打印一个包含单个键值对的字典，可能不是预期行为。
# 通常直接打印值即可。
if 'generated_code' in response:
    print(response['generated_code'])
else:
    pprint.pprint(response) # 如果没有 'generated_code'，打印整个响应以调试

# 上述代码片段将生成以下代码。

# 生成的代码:
# （注意：以下代码是示例输出，由上面的 Python 代码生成并打印）
class TreeNode:
    # 修正：移除希腊字母，使用 Python 默认值语法
    def __init__(self, val=0, left=None, right=None):
        # 修正：使用标准的变量赋值
        self.val = val
        self.left = left
        self.right = right
# ...接下页

# （续上）
# 修正：移除等号后的空格，确保是函数定义
def invert_binary_tree(root):
    """反转二叉树。

    Args:
        root: 二叉树的根节点。

    Returns:
        反转后的二叉树的根节点。
    """
    if not root:
        return None

    # 递归地交换左右子节点
    # 修正：使用标准的变量赋值
    root.left, root.right = invert_binary_tree(root.right), invert_binary_tree(root.left)

    return root

# 示例用法:

# 构建一个示例二叉树
# 修正：使用标准的变量赋值
root = TreeNode(4)
root.left = TreeNode(2)
root.right = TreeNode(7)
root.left.left = TreeNode(1)
root.left.right = TreeNode(3)
# 修正：使用标准的变量赋值
root.right.left = TreeNode(6)
root.right.right = TreeNode(9)

# 反转二叉树
# 修正：使用标准的变量赋值
inverted_root = invert_binary_tree(root)
```

代码片段 1. 使用代码解释器扩展生成并运行 Python 代码

总之，扩展为智能体提供了以多种方式感知、交互和影响外部世界的方法。这些扩展的选择和调用由示例的使用来指导，所有这些都在扩展配置中定义。

## 函数 (Functions)

在软件工程领域，函数被定义为完成特定任务并可根据需要重用的自包含代码模块。当软件开发人员编写程序时，他们通常会创建许多函数来执行各种任务。他们还会定义何时调用函数_a 与函数_b 的逻辑，以及预期的输入和输出。

在智能体世界中，函数的工作方式非常相似，但我们可以用模型来代替软件开发人员。模型可以获取一组已知的函数，并根据其规范决定何时使用每个函数以及函数需要哪些参数。函数与扩展在几个方面有所不同，最显著的是：

1.  模型输出一个函数及其参数，但不进行实时 API 调用。
2.  函数在客户端执行，而扩展在智能体端执行。

再次使用我们的 Google Flights 示例，一个简单的函数设置可能如图 7 所示。

![](https://cdn-mineru.openxlab.org.cn/extract/7b099934-d40b-403d-8804-2269062d890e/dc701da088dcfcb10c176b555c9de5798dd13271c9c92dfe5b8bc45904656ae3.jpg)
图 7. 函数如何与外部 API 交互？

注意，这里的主要区别在于函数和智能体都不直接与 Google Flights API 交互。那么 API 调用实际上是如何发生的呢？

使用函数时，调用实际 API 端点的逻辑和执行被从智能体卸载回客户端应用程序，如下面的图 8 和图 9 所示。这为开发人员提供了对应用程序中数据流的更精细控制。开发人员可能选择使用函数而不是扩展的原因有很多，但一些常见的用例是：

*   API 调用需要在应用程序堆栈的另一层进行，在直接的智能体架构流程之外（例如，中间件系统、前端框架等）。
*   安全或身份验证限制阻止智能体直接调用 API（例如，API 未暴露给互联网，或智能体基础设施无法访问）。
*   时间或操作顺序约束阻止智能体实时进行 API 调用（例如，批处理操作、人在环路审查等）。
*   需要对智能体无法执行的 API 响应应用额外的数据转换逻辑。例如，考虑一个不提供用于限制返回结果数量的过滤机制的 API 端点。在客户端使用函数为开发人员提供了进行这些转换的额外机会。
*   开发人员希望在不为 API 端点部署额外基础设施的情况下迭代智能体开发（即，函数调用可以像 API 的“存根”一样工作）。

虽然如图 8 所示，两种方法在内部架构上的差异很微妙，但对外部基础设施的额外控制和解耦依赖性使得函数调用成为开发人员的一个有吸引力的选择。

![](https://cdn-mineru.openxlab.org.cn/extract/7b099934-d40b-403d-8804-2269062d890e/0e9745e0d1037e27ff0c0d42cfbf369e7f46b9fc101d2396fcbf44d1a7cbef09.jpg)
图 8. 划分扩展和函数调用的客户端与智能体端控制

### 用例

模型可以用来调用函数，以处理最终用户的复杂客户端执行流程，而智能体开发人员可能不希望语言模型管理 API 执行（就像扩展的情况一样）。让我们考虑以下示例，其中一个智能体被训练为旅行礼宾，与想要预订度假旅行的用户互动。目标是让智能体生成一个城市列表，我们可以在我们的中间件应用程序中使用该列表来下载用户旅行计划的图像、数据等。用户可能会说：

我想和家人去滑雪旅行，但不确定去哪里。在对模型的典型提示中，输出可能如下所示：当然，这里有一些您可以考虑的家庭滑雪旅行城市列表：

*   美国科罗拉多州克雷斯特德比特（Crested Butte）
*   加拿大不列颠哥伦比亚省惠斯勒（Whistler）
*   瑞士采尔马特（Zermatt）

虽然上述输出包含我们需要的数据（城市名称），但其格式不适合解析。通过函数调用，我们可以教模型以结构化样式（如 JSON）格式化此输出，这种样式更便于另一个系统解析。给定用户相同的输入提示，来自函数的示例 JSON 输出可能如代码片段 5 所示。

#### Unset (可能是 Protobuf 文本格式或类似结构化文本)

```text
function_call {
  name: "display_cities"
  args: {
    "cities": ["Crested Butte", "Whistler", "Zermatt"],
    "preferences": "skiing"
  }
}
```

代码片段 5. 显示城市列表和用户偏好的示例函数调用负载

这个 JSON 负载由模型生成，然后发送到我们的客户端服务器，以便我们可以对其执行任何我们想要的操作。在这个具体案例中，我们将调用 Google Places API，获取模型提供的城市并查找图像，然后将它们作为格式化的富内容返回给我们的用户。请考虑图 9 中的序列图，该图逐步详细显示了上述交互。

![](https://cdn-mineru.openxlab.org.cn/extract/7b099934-d40b-403d-8804-2269062d890e/9fc9561759c935978073450184a16c11d36ef499e92e30ffdc18dc1797d28996.jpg)
图 9. 显示函数调用生命周期的序列图

图 9 中示例的结果是，利用模型来“填空”，提供客户端 UI 调用 Google Places API 所需的参数。客户端 UI 使用模型在返回的函数中提供的参数来管理实际的 API 调用。这只是函数调用的一个用例，但还有许多其他场景需要考虑，例如：

*   您希望语言模型建议一个可以在代码中使用的函数，但不想在代码中包含凭据。因为函数调用不运行函数，所以您不需要在带有函数信息的代码中包含凭据。
*   您正在运行可能需要几秒钟以上的异步操作。这些场景非常适合函数调用，因为它是异步操作。
*   您希望在与产生函数调用及其参数的系统不同的设备上运行函数。

关于函数要记住的一个关键点是，它们旨在为开发人员提供对 API 调用执行以及整个应用程序数据流的更精细控制。在图 9 的示例中，开发人员选择不将 API 信息返回给智能体，因为它与智能体可能采取的未来行动无关。然而，根据应用程序的架构，将外部 API 调用数据返回给智能体以影响未来的推理、逻辑和行动选择可能是有意义的。最终，由应用程序开发人员选择什么适合特定的应用程序。

#### 函数示例代码

为了从我们的滑雪度假场景中获得上述输出，让我们构建每个组件，使其与我们的 `gemini-1.5-flash-001` 模型一起工作。

首先，我们将 `display_cities` 函数定义为一个简单的 Python 方法。

#### Python

```python
# 修正：导入 Optional
from typing import Optional, List

# 修正：使用 List 而不是 list[str] (Python 3.9+ 才支持 list[str])
# 修正：移除希腊字母，使用标准的变量赋值
def display_cities(cities: List[str], preferences: Optional[str] = None):
    """根据用户的搜索查询和偏好提供城市列表。

    Args:
        preferences (str): 用户的搜索偏好，如滑雪、海滩、餐厅、烧烤等。
        cities (list[str]): 推荐给用户的城市列表。

    Returns:
        list[str]: 推荐给用户的城市列表。
    """
    return cities
```

代码片段 6. 定义 `display_cities` 函数

接下来，我们将实例化我们的模型，构建工具，然后将我们的用户查询和工具传递给模型。执行下面的代码将产生代码片段底部所示的输出。

#### Python

```python
from vertexai.generative_models import GenerativeModel, Tool, FunctionDeclaration
# 修正：导入之前定义的函数
# from snippet_6 import display_cities # 假设 display_cities 在 snippet_6.py 中
# 或者直接在这里定义

# 修正：使用 List 和 Optional (如果之前没有导入)
from typing import Optional, List

def display_cities(cities: List[str], preferences: Optional[str] = None):
    """根据用户的搜索查询和偏好提供城市列表。

    Args:
        preferences (str): 用户的搜索偏好，如滑雪、海滩、餐厅、烧烤等。
        cities (list[str]): 推荐给用户的城市列表。

    Returns:
        list[str]: 推荐给用户的城市列表。
    """
    return cities

# 修正：移除希腊字母，使用标准的变量赋值
model = GenerativeModel("gemini-1.5-flash-001")

# 修正：移除希腊字母，使用标准的变量赋值
display_cities_function = FunctionDeclaration.from_func(display_cities)

# 修正：移除希腊字母，使用标准的变量赋值
tool = Tool(function_declarations=[display_cities_function])

# 修正：移除希腊字母，使用标准的变量赋值，翻译字符串
# message = "I’d like to take a ski trip with my family but I’m not sure where to go."
message = "我想和家人去滑雪旅行，但不确定去哪里。"

# 修正：移除希腊字母，使用标准的变量赋值 `tools=[tool]`
res = model.generate_content(message, tools=[tool])

# 假设 res.candidates[0].content.parts[0].function_call 存在且有 name 和 args 属性
# 注意：实际 API 响应结构可能需要检查
try:
    function_call = res.candidates[0].content.parts[0].function_call
    print(f"函数名称: {function_call.name}")
    # 修正：args 通常是一个类字典对象，直接打印可能更好
    # print(f"函数参数: {function_call.args}")
    import json # 导入 json 模块以便更好地格式化打印 args
    print(f"函数参数: {json.dumps(dict(function_call.args), indent=2, ensure_ascii=False)}") # 转换为字典并格式化打印
except (IndexError, AttributeError) as e:
    print(f"无法提取函数调用信息: {e}")
    print("完整响应:")
    print(res)


# > 函数名称: display_cities
# > 函数参数: {'preferences': 'skiing', 'cities': ['Aspen', 'Vail', 'Park City']}
# (注意：上面的输出是基于英文示例的预期输出，实际中文输出的城市可能不同)
# 预期格式化输出示例：
# 函数名称: display_cities
# 函数参数: {
#  "preferences": "skiing",
#  "cities": [
#    "阿斯彭",
#    "韦尔",
#    "帕克城"
#  ]
# }
```

代码片段 7. 构建工具，将其与用户查询一起发送给模型，并允许函数调用发生

总之，函数提供了一个简单的框架，使应用程序开发人员能够对数据流和系统执行进行细粒度控制，同时有效地利用智能体/模型生成关键输入。开发人员可以选择性地决定是否通过返回外部数据让智能体“保持在循环中”，或者根据特定的应用程序架构要求省略它。

### 数据存储 (Data Stores)

将语言模型想象成一个巨大的图书库，包含其训练数据。但与不断获取新书的图书馆不同，这个图书馆保持静态，只拥有最初训练时获得的知识。这就带来了一个挑战，因为现实世界的知识在不断发展。数据存储（Data Stores）通过提供对更动态、更新信息的访问来解决这个限制，并确保模型的响应保持基于事实和相关性。

考虑一个常见场景，开发人员可能需要向模型提供少量额外数据，也许是以电子表格或 PDF 的形式。

![](https://cdn-mineru.openxlab.org.cn/extract/7b099934-d40b-403d-8804-2269062d890e/98a18643a3b40544149f880cd849987f9ddadfdacc6d5839e31ed6aefc45486e.jpg)
图 10. 智能体如何与结构化和非结构化数据交互？

数据存储允许开发人员以其原始格式向智能体提供额外数据，从而无需进行耗时的数据转换、模型重新训练或微调。数据存储将传入的文档转换为一组向量数据库嵌入，智能体可以使用这些嵌入来提取所需信息，以补充其下一步行动或对用户的响应。

![](https://cdn-mineru.openxlab.org.cn/extract/7b099934-d40b-403d-8804-2269062d890e/b03a7d8543df1611b3d2474cf90b138b909c3fc29fd0fc0784d3afd7a0a12a6a.jpg)
图 11. 数据存储将智能体连接到各种类型的新实时数据源。

### 实现与应用

在生成式 AI 智能体的背景下，数据存储通常实现为开发人员希望智能体在运行时能够访问的向量数据库。虽然我们不会在这里深入探讨向量数据库，但需要理解的关键点是它们以向量嵌入的形式存储数据，这是一种高维向量或所提供数据的数学表示。近年来，数据存储与语言模型结合使用的最广泛的例子之一是基于检索增强生成（RAG）的应用的实现。这些应用程序旨在通过让模型访问各种格式的数据来扩展模型知识的广度和深度，例如：

*   网站内容
*   结构化数据，格式如 PDF、Word 文档、CSV、电子表格等。
*   非结构化数据，格式如 HTML、PDF、TXT 等。

![](https://cdn-mineru.openxlab.org.cn/extract/7b099934-d40b-403d-8804-2269062d890e/b7211048f1b450f0cba1f28a3fc209c39f18a46e0dbbfe6f035736837299e6a9.jpg)
图 12. 智能体和数据存储之间的一对多关系，数据存储可以代表各种类型的预索引数据

每个用户请求和智能体响应循环的底层过程通常建模如图 13 所示。

1.  用户查询被发送到嵌入模型以生成查询的嵌入。
2.  然后使用匹配算法（如 SCaNN）将查询嵌入与向量数据库的内容进行匹配。
3.  匹配的内容以文本格式从向量数据库中检索出来，并发送回智能体。
4.  智能体接收用户查询和检索到的内容，然后制定响应或行动。
5.  最终响应发送给用户。

![](https://cdn-mineru.openxlab.org.cn/extract/7b099934-d40b-403d-8804-2269062d890e/2a9b229ef8d9caf9a2b66b01db8b676f6cb7bc04ca4d45d3b90c90e2a0c6e455.jpg)
图 13. 基于 RAG 的应用程序中用户请求和智能体响应的生命周期

最终结果是一个应用程序，允许智能体通过向量搜索将用户的查询匹配到已知的数据存储，检索原始内容，并将其提供给编排层和模型以进行进一步处理。下一步行动可能是向用户提供最终答案，或执行额外的向量搜索以进一步优化结果。

图 14 展示了实现 RAG 并结合 ReAct 推理/规划的智能体的示例交互。

![](https://cdn-mineru.openxlab.org.cn/extract/7b099934-d40b-403d-8804-2269062d890e/c6a4ab81647fad5f0cd1ba97e6dd32577f9f3bbfb5c575cf4ded4ab5d524ee95.jpg)
图 14. 带有 ReAct 推理/规划的基于 RAG 的应用程序示例

## 工具回顾

总而言之，扩展、函数和数据存储构成了可供智能体在运行时使用的几种不同工具类型。每种工具都有其自身的用途，可以根据智能体开发人员的判断一起使用或独立使用。

<html><body><table><tr><td></td><td>扩展 (Extensions)</td><td>函数调用 (Function Calling)</td><td>数据存储 (Data Stores)</td></tr><tr><td>执行用例</td><td>智能体端执行</td><td>客户端执行</td><td>智能体端执行</td></tr><tr><td>适用场景</td><td><ul><li>开发人员希望智能体控制与 API 端点的交互</li><li>利用原生预构建扩展（例如 Vertex Search、代码解释器等）时很有用</li><li>多跳规划（例如，智能体使用上一个操作/API 调用的输出来决定下一步）</li></ul></td><td><ul><li>安全或身份验证限制阻止智能体直接调用 API</li><li>时间约束或操作顺序约束阻止智能体进行 API 调用（例如，批量操作、人在环路审查等）</li><li>API 未暴露给互联网，或 Google 系统无法访问</li></ul></td><td>开发人员希望使用以下任何数据类型实现检索增强生成 (RAG)：<ul><li>来自预索引域和 URL 的网站内容</li><li>结构化数据，格式如 PDF、电子表格等</li><li>关系型/非关系型数据库</li><li>非结构化数据，格式如 HTML、PDF、TXT 等</li></ul></td></tr></table></body></html>

## 通过目标学习提升模型性能

有效使用模型的一个关键方面是它们在生成输出时选择正确工具的能力，尤其是在生产环境中大规模使用工具时。虽然通用训练有助于模型发展这项技能，但现实世界场景通常需要超出训练数据的知识。可以将其想象成基本烹饪技能与掌握特定菜系之间的区别。两者都需要基础的烹饪知识，但后者需要有针对性的学习才能获得更细致入微的结果。

为了帮助模型获取这类特定知识，存在几种方法：

*   **上下文学习 (In-context learning)**：此方法在推理时为通用模型提供提示、工具和少量示例（few-shot examples），使其能够“即时”学习如何以及何时为特定任务使用这些工具。ReAct 框架是这种自然语言方法的示例。
*   **基于检索的上下文学习 (Retrieval-based in-context learning)**：此技术通过从外部存储器中检索最相关的信息、工具和相关示例来动态填充模型提示。Vertex AI 扩展中的“示例存储”（Example Store）或前面提到的基于 RAG 的数据存储架构就是这种方法的示例。
*   **基于微调的学习 (Fine-tuning based learning)**：此方法涉及在推理之前使用更大的特定示例数据集训练模型。这有助于模型在收到任何用户查询之前理解何时以及如何应用某些工具。

为了进一步阐述每种目标学习方法，让我们回到我们的烹饪类比。

*   想象一位厨师收到了一个特定的食谱（提示）、一些关键食材（相关工具）和一些示例菜肴（少量示例）。基于这些有限的信息和厨师的一般烹饪知识，他们需要“即时”弄清楚如何准备最符合食谱和顾客偏好的菜肴。这就是**上下文学习**。
*   现在让我们想象我们的厨师在一个拥有储备充足的食品储藏室（外部数据存储）的厨房里，里面装满了各种食材和食谱（示例和工具）。厨师现在能够动态地从食品储藏室中选择食材和食谱，从而更好地满足顾客的食谱和偏好。这使得厨师能够利用现有知识和新知识，制作出更明智、更精致的菜肴。这就是**基于检索的上下文学习**。
*   最后，让我们想象一下，我们送厨师回学校学习一种或多种新菜系（在更大的特定示例数据集上进行预训练）。这使得厨师能够以更深入的理解来应对未来未见过的顾客食谱。如果我们希望厨师在特定菜系（知识领域）方面表现出色，这种方法是完美的。这就是**基于微调的学习**。

这些方法中的每一种在速度、成本和延迟方面都有其独特的优缺点。然而，通过在智能体框架中结合这些技术，我们可以利用各种优势并最大限度地减少它们的劣势，从而实现更健壮和适应性更强的解决方案。

## 使用 LangChain 快速开始智能体开发

为了提供一个真实可执行的智能体实例，我们将使用 LangChain 和 LangGraph 库构建一个快速原型。这些流行的开源库允许用户通过将逻辑、推理和工具调用序列“链接”在一起来构建客户智能体，以回答用户的查询。我们将使用我们的 `gemini-1.5-flash-001` 模型和一些简单的工具来回答来自用户的多阶段查询，如代码片段 8 所示。

我们使用的工具是 SerpAPI（用于 Google 搜索）和 Google Places API。在执行代码片段 8 中的程序后，您可以在代码片段 9 中看到示例输出。

```python
# 修正：导入 os 模块以设置环境变量
import os
from langgraph.prebuilt import create_react_agent
from langchain_core.tools import tool
from langchain_community.utilities import SerpAPIWrapper
from langchain_community.tools import GooglePlacesTool
# 修正：导入 ChatVertexAI
from langchain_google_vertexai import ChatVertexAI

# 修正：使用标准赋值。用实际密钥替换 "XXXXX"。
os.environ["SERPAPI_API_KEY"] = "YOUR_SERPAPI_API_KEY" # 替换为您的 SerpAPI 密钥
os.environ["GPLACES_API_KEY"] = "YOUR_GOOGLE_PLACES_API_KEY" # 替换为您的 Google Places API 密钥

@tool
def search(query: str):
    """使用 SerpAPI 进行 Google 搜索。"""
    # 修正：使用标准赋值
    search_wrapper = SerpAPIWrapper()
    return search_wrapper.run(query)

@tool
def places(query: str):
    """使用 Google Places API 进行 Google Places 查询。"""
    # 修正：使用标准赋值
    places_tool = GooglePlacesTool()
    return places_tool.run(query)

# 修正：使用标准赋值。确保模型名称正确。
# model = ChatVertexAI(model="gemini-1.5-flash-001") # 修正：模型名称可能需要调整，例如 'gemini-pro' or the specific identifier
model = ChatVertexAI(model_name="gemini-1.5-flash-001") # 使用 model_name 参数

# 修正：使用标准赋值
tools = [search, places]

# 修正：使用标准赋值。翻译查询字符串。
# query = "Who did the Texas Longhorns play in football last week? What is the address of the other team's stadium?"
query = "德克萨斯长角牛队上周橄榄球比赛的对手是谁？对方球队体育场的地址是什么？"

# 修正：使用标准赋值
agent_executor = create_react_agent(model, tools) # create_react_agent 返回的是一个 executor

# 修正：使用标准赋值
input_data = {"messages": [("human", query)]}

# 修正：使用标准赋值。stream_mode 可能需要调整，具体取决于 LangGraph 版本。
# 修正：迭代 agent_executor.stream 而不是 agent.stream
# 修正：检查 message 类型并打印
for s in agent_executor.stream(input_data, stream_mode="values"): # 尝试使用 "values"
    # s 通常是一个字典，其中包含多个步骤的信息
    # 我们关注的是最新的消息或动作
    # print(s) # 打印整个步骤信息以调试
    if "messages" in s and s["messages"]:
         message = s["messages"][-1]
         if isinstance(message, tuple):
             print(message)
         else:
             # 假设 message 对象有 pretty_print 方法
             try:
                 message.pretty_print()
             except AttributeError:
                 print(message) # 如果没有 pretty_print，直接打印
    elif "agent" in s and "messages" in s["agent"] and s["agent"]["messages"]:
         # 另一种可能的结构
         message = s["agent"]["messages"][-1]
         if isinstance(message, tuple):
             print(message)
         else:
             try:
                 message.pretty_print()
             except AttributeError:
                 print(message)

```

代码片段 8. 使用 LangChain 构建和运行智能体

### Unset (示例输出格式)

```text
====== Human Message ====================================
德克萨斯长角牛队上周橄榄球比赛的对手是谁？对方球队体育场的地址是什么？
====== Ai Message =======================================
Tool Calls:
  search(query='Texas Longhorns football schedule last week')
====== Tool Message =====================================
Name: search
{...搜索结果: "NCAA Division I Football, Georgia, Date..."} (实际结果会更详细)
====== Ai Message =======================================
德克萨斯长角牛队上周与佐治亚斗牛犬队进行了比赛。
Tool Calls:
  places(query='Georgia Bulldogs stadium address')
====== Tool Message =====================================
Name: places
{...Sanford Stadium Address: 100 Sanford...} (实际结果会更详细)
====== Ai Message =======================================
佐治亚斗牛犬队体育场的地址是 100 Sanford Dr, Athens, GA 30602, USA。
```

代码片段 9. 来自 LangChain 智能体的示例输出

虽然这是一个相当简单的智能体示例，但它演示了模型、编排和工具这些基础组件协同工作以实现特定目标。在最后一节中，我们将探讨这些组件如何在 Google 规模的托管产品（如 Vertex AI 智能体和 Generative Playbooks）中结合在一起。

## 使用 Vertex AI 智能体进行生产应用

虽然本白皮书探讨了智能体的核心组件，但构建生产级应用程序需要将它们与用户界面、评估框架和持续改进机制等附加工具集成。Google 的 Vertex AI 平台通过提供一个完全托管的环境来简化此过程，该环境包含了前面介绍的所有基本元素。开发人员可以使用自然语言界面快速定义其智能体的关键元素——目标、任务指令、工具、用于任务委托的子智能体以及示例——以轻松构建所需的系统行为。此外，该平台还附带了一套开发工具，用于测试、评估、衡量智能体性能、调试和提高已开发智能体的整体质量。这使开发人员能够专注于构建和完善他们的智能体，而平台本身则负责管理基础设施、部署和维护的复杂性。

在图 15 中，我们提供了一个基于 Vertex AI 平台构建的智能体示例架构，该架构使用了各种功能，例如 Vertex Agent Builder、Vertex Extensions、Vertex Function Calling 和 Vertex Example Store 等。该架构包含了生产就绪应用程序所需的许多不同组件。

![](https://cdn-mineru.openxlab.org.cn/extract/7b099934-d40b-403d-8804-2269062d890e/1f829b0e148637d465f1e48d0628d666d04758c6bf16e4a337be19f64b07c9be.jpg)
图 15. 基于 Vertex AI 平台构建的示例端到端智能体架构

您可以从我们的[官方文档](https://cloud.google.com/vertex-ai/docs/generative-ai/agents/try-an-agent)尝试此预构建智能体架构的示例。

# 总结

在本白皮书中，我们讨论了生成式 AI 智能体的基本构建模块、它们的组成以及以认知架构形式有效实现它们的方法。本白皮书的一些关键要点包括：

1.  **智能体通过利用工具扩展了语言模型的能力**，使其能够访问实时信息、建议现实世界的操作，并自主规划和执行复杂任务。智能体可以利用一个或多个语言模型来决定何时以及如何转换状态，并使用外部工具来完成模型自身难以或无法完成的任何数量的复杂任务。
2.  **智能体操作的核心是编排层**，这是一个构建推理、规划、决策并指导其行动的认知架构。各种推理技术，如 ReAct、思维链和思维树，为编排层提供了一个框架，使其能够接收信息、执行内部推理，并生成明智的决策或响应。
3.  **工具，例如扩展、函数和数据存储，是智能体通往外部世界的钥匙**，允许它们与外部系统交互并访问其训练数据之外的知识。**扩展**在智能体和外部 API 之间架起了一座桥梁，实现了 API 调用和实时信息的检索。**函数**通过分工为开发人员提供了更细致的控制，允许智能体生成可在客户端执行的函数参数。**数据存储**为智能体提供了对结构化或非结构化数据的访问，从而实现了数据驱动的应用程序。

智能体的未来蕴藏着激动人心的进步，我们才刚刚触及可能性的表面。随着工具变得更加复杂和推理能力的增强，智能体将有能力解决日益复杂的问题。此外，“智能体链”（agent chaining）的战略方法将继续获得发展势头。通过组合专门的智能体——每个智能体都在特定领域或任务中表现出色——我们可以创建一种“智能体专家混合”（mixture of agent experts）的方法，能够在各个行业和问题领域提供卓越的结果。

重要的是要记住，构建复杂的智能体架构需要迭代的方法。实验和改进是为特定业务案例和组织需求寻找解决方案的关键。由于支撑其架构的基础模型的生成性质，没有两个智能体是完全相同的。然而，通过利用这些基础组件各自的优势，我们可以创建有影响力的应用程序，扩展语言模型的能力并驱动现实世界的价值。

# 尾注

1.  Shafran, I., Cao, Y. et al., 2022, 'ReAct: Synergizing Reasoning and Acting in Language Models'. 见: https://arxiv.org/abs/2210.03629
2.  Wei, J., Wang, X. et al., 2023, 'Chain-of-Thought Prompting Elicits Reasoning in Large Language Models'. 见: https://arxiv.org/pdf/2201.11903.pdf.
3.  Wang, X. et al., 2022, 'Self-Consistency Improves Chain of Thought Reasoning in Language Models'. 见: https://arxiv.org/abs/2203.11171.
4.  Diao, S. et al., 2023, 'Active Prompting with Chain-of-Thought for Large Language Models'. 见: https://arxiv.org/pdf/2302.12246.pdf.
5.  Zhang, H. et al., 2023, 'Multimodal Chain-of-Thought Reasoning in Language Models'. 见: https://arxiv.org/abs/2302.00923.
6.  Yao, S. et al., 2023, 'Tree of Thoughts: Deliberate Problem Solving with Large Language Models'. 见: https://arxiv.org/abs/2305.10601.
7.  Long, X., 2023, 'Large Language Model Guided Tree-of-Thought'. 见: https://arxiv.org/abs/2305.08291.
8.  Google. 'Google Gemini Application'. 见: http://gemini.google.com.
9.  Swagger. 'OpenAPI Specification'. 见: https://swagger.io/specification/.
10. Xie, M., 2022, 'How does in-context learning work? A framework for understanding the differences from traditional supervised learning'. 见: https://ai.stanford.edu/blog/understanding-incontext/.
11. Google Research. 'ScaNN (Scalable Nearest Neighbors)'. 见: https://github.com/google-research/google-research/tree/master/scann.
12. LangChain. 'LangChain'. 见: https://python.langchain.com/v0.2/docs/introduction/.

---

## 致谢

**审阅者与贡献者**: 

Evan Huang, Emily Xue, Olcan Sercinoglu, Sebastian Riedel, Satinder Baveja ,Antonio Gulli ,Anant Nawalgaria

![](https://cdn-mineru.openxlab.org.cn/extract/7b099934-d40b-403d-8804-2269062d890e/283a5194e70375647c55e93bb3bedb78d6fb1ed8d820282efc200806ae560775.jpg)

**策划与编辑**

Antonio Gulli, Anant Nawalgaria, Grace Mollison

**技术撰稿人** Joey Haymaker

**设计师** Michael Lanning