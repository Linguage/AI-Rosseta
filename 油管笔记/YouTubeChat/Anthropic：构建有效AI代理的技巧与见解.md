
  - 原文标题：Tips for building AI agents - YouTube  
  - 链接：[Anthropic | YouTube](https://www.youtube.com/watch?v=LP5OCa20Zpg)  
  - **文章类别**：博客/访谈实录  

---

## 概要
本次访谈中，Anthropic 的 Alex、Erik 和 Barry 深入探讨了 AI Agent 的定义、应用、挑战与未来。他们强调了区分“工作流”（预定义步骤的 LLM 调用链）和“Agent”（LLM 自主决定执行步骤，循环直至解决问题）的重要性。

访谈揭示了 Agent 设计的关键：站在模型的角度思考，提供清晰的工具描述和环境上下文，如同对待工程师一样对待模型。 讨论还指出, Agent 在编码和搜索等领域具有巨大潜力，因为这些领域具有可验证性（如单元测试），能为 Agent 提供反馈循环。

尽管 Agent 在企业级应用中前景广阔，有望自动化重复任务、提升效率，但面向消费者的 Agent 目前仍被认为过度炒作，因为完全指定用户偏好和验证结果的成本高昂。

对于开发者，专家建议从简单做起，确保有衡量结果的机制，并构建能随着模型进步而不断改进的产品。未来，多 Agent 环境的交互和涌现行为值得关注，但这仍处于早期探索阶段。 总之, 现在是开发者培养“Agent 思维”的时候了.

### 关键词：
#AI代理 ， #工作流 ， #模型应用 ， #未来趋势

## 访谈框架

```markdown

对话纲要：
├── 开场 (0:00 - 0:24)
│   ├── Alex 提出对消费者 Agent 的过度炒作的看法
│   └── 介绍参与者：Alex, Erik, Barry
├── 定义 AI Agents 和工作流 (0:25 - 1:43)
│   ├── Alex 提问：什么是 Agent？开发者为何关心？
│   └── Erik 回答：
│       ├── 区分“工作流”和“Agent”
│       ├── 工作流：LLM 调用链式连接
│       ├── Agent：LLM 自主决定运行次数，循环直到解决
│       └── Agent 定义：LLM 自主选择路径，更自主；工作流：固定步骤
├── 工作流和 Agent 的区别 (1:44 - 2:51)
│   ├── Alex 追问：区分的背景和惊讶的模式
│   └── Barry 回答：
│       ├── 随着模型和团队复杂化，出现两种模式：
│       │   ├── 工作流：代码预先编排
│       │   └── Agent：更简单，形式不同
│       └── 模型和工具改进，Agent 更普遍、强大
├── Agent 和工作流的代码实现 (2:53 - 4:13)
│    └── Erik 解释：
│       ├── 工作流提示：输入输出链式传递，步骤固定，提示具体
│       └── Agent 提示：开放，提供工具，指示模型持续操作
├── 幕后故事 (4:18 - 7:20)
│   ├── Alex 询问：有趣的故事和用户使用情况
│   ├── Barry 的故事：
│   │   ├── 模拟 Claude 视角理解 Agent 行为
│   │   └── 关键点：明确模型缺乏的上下文和知识
│   └── Erik 的故事：
│       ├── 详细提示与简陋工具的对比
│       ├── 关键点：站在模型角度，工具描述也需提示工程
├── 为什么现在写关于 Agent 的文章 (7:25 - 8:48)
│   ├── Barry：解释清楚，模型能力足够
│   └── Erik：指导使用，避免“大炮打蚊子”
├── Agent 的过度炒作和被低估的方面 (8:50 - 9:52)
│   └── Erik：被低估 - 节省时间，改变做事动态
├── 识别 Agent 的有用应用 (9:52 - 10:43)
│    └── Barry:
│        ├── 最佳应用: 有价值, 复杂, 且低错误成本的任务
│        └── 例子：编码和搜索（可牺牲精度换取召回）
├── 编码 Agent：潜力和挑战 (10:43 - 12:45)
│   ├── 可验证性（单元测试）
│   ├── Erik：反馈循环的重要性
│   └── Erik 的观点：下一个限制是验证，需要更好的测试
├── 2025 年 Agent 的未来 (12:47 - 16:24)
│   ├── Barry：多 Agent 环境（狼人杀游戏），涌现行为
│   ├── Erik：企业广泛采用，自动化重复任务；消费者 Agent 仍过度炒作（偏好难指定，验证成本高）
│   └── Erik：模型需时间积累上下文
└── 给开发者的建议 (16:27 - 18:12)
    ├── Erik：衡量结果，避免真空构建，考虑更简单方法
    ├── Barry：简单开始，可衡量结果，欣赏单 LLM 调用实现
    └── Erik：构建随模型进步而改进的产品
    
```


## 访谈录

### 开场

**Alex:** 大家好！我感觉现在针对消费者的 AI Agent 有点被过度炒作了。你们觉得呢？让一个 Agent 完全帮你预订假期，几乎和自己动手预订一样麻烦。

**Alex:** 今天我们来聊聊我们最近的一篇博文——《构建有效的 Agent》。我是 Alex，Anthropic 的 Claude Relations 负责人。

**Erik:** 我是 Erik，Anthropic 研究团队的成员。

**Barry:** 我是 Barry，来自应用 AI 团队。

### 定义 AI Agents 和工作流

**Alex:** 我们先来个基础问题：对于刚接触的观众，Agent 到底是什么？为什么开发者，或者说正在使用 AI 构建产品的人，应该关心这些？Erik，你先来说说？

**Erik:** 好的。我们在博文里探讨过，首先，很多人说“一切都是 Agent”，几乎任何比单个 LLM 调用更复杂的东西都被称为 Agent。我们在博文里试图区分“工作流”（workflows）和“Agent”。工作流是指一系列 LLM 调用链式连接起来。而我们认为的 Agent，是让 LLM 自己决定运行多少次，它会持续循环，直到找到解决方案。这可以是与客户进行客户支持对话，也可以是迭代代码更改。关键是，你不知道完成它需要多少步，这就是我们所说的 Agent。

**Alex:** 有意思。所以，在 Agent 的定义中，我们是让 LLM 自己选择命运，决定它想做什么，采取什么行动，而不是我们预先为它定义一条路径。

**Erik:** 完全正确。它更自主。而工作流，你可以把它想象成，就像在轨道上，通过固定数量的步骤。

### 工作流和 Agent 的区别

**Alex:** 我猜这种区分是与客户多次对话、与不同团队合作，甚至我们自己尝试的结果。Barry，能不能详细说说，当我们开始区分工作流和 Agent 时，具体情况是怎样的？在这个过程中，哪些模式最让你惊讶？

**Barry:** 当然。老实说，我认为这一切都是随着模型变得更好、团队变得更复杂而演变的。我们与许多非常成熟的客户合作，我们经历了从单个 LLM 到多个 LLM，最终到 LLM 自我编排的过程。我们之所以决定进行这种区分，是因为我们开始看到这两种不同的模式：一种是由代码预先编排的工作流，另一种是 Agent，它更简单，但在其他方面也很复杂，形式不同。随着模型和所有工具越来越好，Agent 变得越来越普遍，能力也越来越强。这就是为什么我们认为现在是时候给出一个正式的定义了。

### Agent 和工作流的代码实现

**Alex:** 那么在实践中，如果一个开发者要实现其中一个，在开始构建时，代码会是什么样子？我们能不能具体到提示层面？Agent 提示或流程是什么样的，工作流又是什么样的？

**Erik:** 工作流提示是这样的：你有一个提示 A，获取它的输出，输入到提示 B，再获取提示 B 的输出，输入到提示 C，然后就完成了。这是一条直线，步骤数量固定。你确切地知道会发生什么，也许你有一些额外的代码来检查中间结果，确保它们没问题。但你确切地知道在其中一条路径中会发生什么。每个提示都非常具体，只是将一个输入转换为另一个输出。例如，其中一个提示可能接收用户问题，并将其分为五个类别之一，以便下一个提示可以更具体。

**Erik:** 相比之下，Agent 提示会更加开放，通常会给模型提供工具或多个检查项，并说：“这是问题，你可以进行网络搜索，或者编辑这些代码文件，或者运行代码，并持续这样做，直到你得到答案。”

**Alex:** 我明白了。所以这里有几个不同的用例。

### 幕后故事

**Alex:** 我们已经从高层次上讨论了我们如何看待这些工作流和 Agent，以及博文的内容。我想深入了解一下幕后的故事。Barry，有没有什么有趣的故事，你从客户那里看到的有趣的事情，或者人们在生产中实际使用这些东西的方式？

**Barry:** 有的，这实际上是我自己构建 Agent 的经验。我在 Sonnet v2 刷新前一个月加入。我的一个入职任务是运行 OSWorld，这是一个计算机使用基准测试。整整一个星期，我和另一位工程师盯着 Agent 的轨迹，这些轨迹对我们来说很不直观。我们不确定为什么模型会做出它所做的决定，考虑到我们给它的指令。所以我们决定像 Claude 一样行动，把自己放在那个环境中。我们会做一件很傻的事情，闭上眼睛整整一分钟，然后对着屏幕眨眼一秒钟，再闭上眼睛，然后想，我必须编写 Python 代码才能在这个环境中操作，我会怎么做？突然之间，一切都变得合理多了。我觉得很多 Agent 设计都归结于此。有很多上下文和知识，模型可能没有，我们必须对模型有同理心，我们必须在提示、工具描述和环境中明确说明。

**Alex:** 我明白了。所以给开发者的一条建议是，几乎就像你通过模型本身的视角来看待一样，考虑什么是最适用的指令？模型是如何看待世界的，这与我们作为人类的操作方式非常不同，因为我们有额外的上下文。Erik，你有没有其他你看到的故事？

**Erik:** 是的，实际上我的想法非常相似。我认为很多人真的忘记了这样做了。也许我看到的最有趣的事情是，人们会花很多精力来创建这些非常漂亮、详细的提示，然后他们给模型提供的工具却非常简陋，没有文档，参数名为 A 和 B。这就像，一个工程师无法使用这个。

**Alex:** 对。

**Erik:** 把它当作一个必须使用的函数来工作。因为没有文档，你怎么能期望 Claude 也使用它呢？所以这是一种缺乏“设身处地为模型着想”的做法。我认为很多人在开始尝试使用工具和函数调用时，他们忘记了他们也必须进行提示，他们把模型看作是一个更经典的编程系统。但它仍然是一个模型，你需要在工具本身的描述中进行提示工程。

**Alex:** 是的，我注意到了。就像人们忘记了这一切都是同一个提示的一部分。所有内容都被输入到上下文窗口中的同一个提示中，编写一个好的工具描述也会影响提示的其他部分。

### 为什么现在写关于 Agent 的文章

**Alex:** Agent 现在是一个热门话题，很多人都在谈论它，也有很多关于这个主题的文章和视频。是什么让你们认为现在是时候我们自己写点东西，更多地谈谈 Agent 的细节？

**Barry:** 当然。我认为对我们来说，最重要的事情之一就是能够很好地解释事情。这是我们很大一部分动机，因为我们走进客户会议，所有东西都用不同的术语来指代，即使它们具有相同的结构。所以我们认为，如果我们能有一套定义、一套图表和代码来向我们的客户解释这些东西，那将会非常有用。而且，我们已经到了模型能够处理我们看到的许多 Agent 式工作流的阶段。这似乎是时候让我们给出一些定义，或者让这些对话更容易。

**Erik:** 对我来说，我看到人们对 Agent 非常兴奋，但也有很多人真的不知道 Agent 在实践中意味着什么，所以他们试图将 Agent 用于他们遇到的任何问题，即使更简单的系统也能工作。所以我认为这是我们应该写这篇文章的原因之一，指导人们如何使用 Agent，以及何时使用 Agent 是合适的。不要“用大炮打蚊子”。

### Agent 的过度炒作和被低估的方面

**Alex:** 这正好引出了我的下一个问题。有很多关于 Agent 潜力的讨论，每个开发者、每个初创公司和企业都在思考如何为他们的公司或产品构建自己的 Agent 版本。但你们开始看到什么在生产中真正有效。所以我们来玩个小游戏。我想知道一件关于 Agent 现在被过度炒作的事情，以及一件被低估的事情，就实现或实际生产中的用途或潜力而言。Erik，我们先从你开始。

**Erik:** 我觉得被低估的是那些能节省人们时间的事情，即使是很小的时间。很多时候，如果你只看表面，会觉得，哦，这只需要我一分钟，即使你能完全自动化它，也只是一分钟。这有什么用？但实际上，这改变了做事的动态，你现在可以比以前多做一百倍。所以我最兴奋的是那些如果更容易就能真正扩大规模的事情。

### 识别 Agent 的有用应用

**Alex:** Barry，你怎么看？

**Barry:** 我不知道这是否一定与炒作有关，但我认为现在很难确定 Agent 真正需要的场景。我认为有一个交叉点是使用 Agent 的最佳位置，那就是一组有价值且复杂的任务，但错误成本或监控成本可能相对较低。除非我们真正研究现有的流程，否则这组任务并不是非常清晰和明显的。我认为编码和搜索是 Agent 非常有用的两个典型例子。以搜索为例，对吧？这是一项非常有价值的任务。很难进行深入的迭代搜索，但你总是可以牺牲一些精度来换取召回率，然后获取更多一点的文档或信息，然后过滤掉。所以我们在 Agent 式搜索中看到了很多成功。

### 编码 Agent：潜力和挑战

**Alex:** 目前的编码 Agent 是什么样的？

**Erik:** 编码 Agent 非常令人兴奋，因为它们是可验证的，至少部分可验证。代码有一个很好的特性，你可以为它编写测试，然后你编辑代码，测试要么通过，要么不通过。现在，这假设你有良好的单元测试，我认为世界上每个工程师都会说，我们没有。

**Alex:** 是的。

**Erik:** 但至少它比很多东西都好。对于许多其他领域，没有等效的方法来做到这一点。所以这至少给了编码 Agent 一种方法，让它在每次循环时都能获得更多信号。所以，如果每次它都再次运行测试，它会看到错误或输出是什么，这让我认为，模型可以通过获得这种反馈来收敛到正确的答案。如果你没有某种机制在迭代时获得反馈，你就没有注入任何更多的信号，你只会得到噪音。因此，如果没有类似的东西，Agent 就没有理由收敛到正确的答案。

**Alex:** 我明白了。那么，目前在编码方面提高 Agent 性能的最大障碍是什么？

**Erik:** 对于编码，在过去的一年里，我们在 SWE-bench 上看到，结果从非常非常低上升到，我认为现在超过了 50%，这真的很了不起。所以模型在编写代码来解决这些问题方面变得非常出色。我觉得我这里有一个稍微有争议的观点，我认为下一个限制因素将回到验证。对于那些我们确实有完美的单元测试的情况，这开始起作用了，但对于现实世界的情况，我们通常没有完美的单元测试。所以这就是我现在正在思考的，找到我们可以验证的方法，我们可以为真正关心的事情添加测试，以便模型本身可以测试这一点，并在返回给人类之前知道它是对还是错。

**Alex:** 我明白了。确保我们可以在流程本身中嵌入某种反馈循环。

**Erik:** 完全正确。是对还是错。

### 2025 年 Agent 的未来

**Alex:** 2025 年 Agent 的未来会是什么样子？Barry，我们先从你开始。

**Barry:** 是的，我认为这是一个非常困难的问题。这可能不是一个实际的事情，但我一直很感兴趣的一件事是多 Agent 环境会是什么样子。我想我已经给 Erik 看过这个了，我建立了一个环境，一群 Claude 可以启动其他的 Claude，并一起玩狼人杀游戏。这是一个完全……

**Alex:** 狼人杀是什么？

**Barry:** 狼人杀是一个社交推理游戏，所有玩家都试图弄清楚彼此的角色是什么。它与 Mafia 非常相似，它完全是基于文本的，这非常适合 Claude 参与。

**Alex:** 我明白了。所以我们有 Claude，多个不同的 Claude 在这个游戏中扮演不同的角色，所有 Claude 都在互相交流。

**Barry:** 是的，完全正确。然后你会看到很多有趣的互动，你以前从未见过的，这是我非常兴奋的事情，因为就像我们从单个 LLM 到多 LLM 一样，我认为到今年年底，我们可能会看到我们从 Agent 到多 Agent。在这个领域有一些有趣的研究问题需要解决。

**Alex:** 在 Agent 如何相互交互方面，当你协调执行不同任务的 Agent 时，这种涌现行为是什么样的？

**Barry:** 完全正确。以及这是否真的有用，或者比拥有更多资源的单个 Agent 更好。

**Alex:** 我们现在是否看到任何在生产中实际工作的多 Agent 方法？

**Barry:** 我觉得在生产中，我们甚至还没有看到很多成功的单 Agent。

**Alex:** 有趣。

**Barry:** 但是，这是具有改进功能的下一代模型的成功 Agent 的潜在扩展。所以这不是建议每个人都去探索投票 Agent 环境。这只是，我认为，为了理解模型的行为，这为我们提供了一种更好的方式来理解模型行为。

**Alex:** 我明白了。好的，Erik，2025 年 Agent 的未来会是什么样子？

**Erik:** 我觉得在 2025 年，我们将看到许多企业采用 Agent，开始自动化许多重复性任务，并真正扩展许多人们以前想做更多但成本太高的事情。你现在可以用这些东西做 10 倍或 100 倍的事情。我想象的是，每个 pull request 都会触发一个编码 Agent 来更新你的所有文档。像这样的事情以前是成本过高的。但是一旦你认为 Agent 几乎是免费的，你就可以开始做这些事情，到处添加这些“花里胡哨”的功能。我认为也许还不会发生的事情，回到什么是过度炒作？我觉得针对消费者的 Agent 现在相当被过度炒作。

**Alex:** 好的，开始了。热门话题。

**Erik:** 因为我认为，我们谈到了可验证性。我认为对于很多消费者任务来说，完全指定你的偏好和任务是什么，几乎和你自己做一样费力，而且验证成本很高。所以试图让一个 Agent 完全为你预订假期，描述你到底想要什么样的假期和你的偏好，几乎和你自己去预订一样困难。而且风险很高。你不希望 Agent 在你没有先接受的情况下就去预订机票。

**Alex:** 这里是不是也存在一个上下文的问题，模型是否能够推断出关于某人的信息，而不必明确地去询问和了解随着时间的推移的偏好？

**Erik:** 是的，所以我认为这些事情会实现的，但首先你需要建立这种上下文，以便模型已经知道你的偏好。我认为这需要时间。

**Alex:**我明白。

**Erik:** 我们需要一些垫脚石才能完成更大的任务，例如计划整个假期。
**Alex:** 我明白。

### 给开发者的建议

**Alex:** 最后一个问题，对于正在探索这个领域的开发者，你有什么建议可以给他们，无论是开始构建还是从一般的未来保障的角度来考虑？

**Erik:** 我觉得我最好的建议是，确保你有一种方法来衡量你的结果。因为我看到很多人会在真空中构建，没有任何方法可以获得关于他们的构建是否有效的反馈。你最终可能会构建很多东西，却没有意识到它不起作用，或者也许更简单的东西实际上也能做得一样好。

**Barry:** 是的，非常相似，从尽可能简单的地方开始，并在你构建更多复杂性时保持可衡量的结果。有一件事让我印象深刻，我与一些非常有创意的初创公司合作，他们可以在一个 LLM 调用中完成所有事情，围绕代码的编排（即使模型变得更好，这种编排也会持续存在）是他们的优势。当我看到其中一个时，我总是很高兴，因为我认为他们可以从未来的能力改进中获益。是的，我认为实际上，我们不知道什么用例对 Agent 来说是最好的，情况会发生变化，但现在可能是开始培养一些 Agent 思维的好时机，只是为了更好地理解这种能力。

**Erik:** 是的，我想强调你说的，为模型变得更好而兴奋。我认为如果你看看你的初创公司或你的产品，然后想，哦，天哪，如果模型变得更聪明，我们所有的护城河都会消失。这意味着你构建了错误的东西。相反，你应该构建一些东西，以便随着模型变得更聪明，你的产品变得越来越好。

**Alex:** 对。这是很好的建议。Erik，Barry，谢谢你们。这是《构建有效的 Agent》。谢谢。

**Erik & Barry:** 谢谢。
