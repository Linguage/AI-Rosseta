# 欢迎来到体验时代

- 作者：David Silver, Richard S. Sutton\*
- 原文连接：[The Era of Experience](https://storage.googleapis.com/deepmind-media/Era-of-Experience%20/The%20Era%20of%20Experience%20Paper.pdf)

## 摘要

我们正站在人工智能新时代的门槛上，这个时代有望达到前所未有的能力水平。新一代智能体将主要通过从经验中学习来获得超人的能力。本文探讨了将定义这个即将到来的时代的关键特征。

## 人类数据时代

人工智能（AI）近年来取得了显著进展，通过训练大量人类生成的数据，并利用专家人类的例子和偏好进行微调。大型语言模型（LLMs）就是一个典型的例子，它们已经达到了广泛的通用性水平。单个LLM现在可以执行从写诗和解决物理问题到诊断医疗问题和总结法律文件等各种任务。

然而，虽然模仿人类足以在一定程度上重现许多人类的能力，但仅靠这种方法并没有，也可能无法在许多重要主题和任务上实现超人智能。在数学、编程和科学等关键领域，从人类数据中提取的知识正在迅速接近极限。大多数高质量的数据来源——那些能够真正提高强大智能体表现的数据——要么已经被消耗殆尽，要么即将被消耗殆尽。仅靠人类数据的监督学习驱动的进步速度正在明显放缓，这预示着需要一种新的方法。此外，有价值的新见解，如新定理、新技术或科学突破，都超出了当前人类理解的范围，无法通过现有的人类数据捕捉。

# 体验时代

要取得更大的进展，需要一种新的数据来源。这种数据必须以一种智能体变得更强大时不断改进的方式生成；任何静态的合成数据生成过程都将很快被超越。这可以通过让智能体从自己的经验中持续学习来实现，即由智能体与其环境互动生成的数据。人工智能正处于一个新时期的开端，在这个时期，经验将成为进步的主要媒介，并最终超越当今系统中使用的庞大的人类数据规模。

这种转变可能已经开始，即使对于那些体现以人为本的人工智能的大型语言模型也是如此。一个例子是数学能力。AlphaProof [20] 最近成为第一个在国际数学奥林匹克竞赛中获得奖牌的程序，超越了以人为本的方法 [27, 19] 的表现。AlphaProof最初接触了大约10万个由人类数学家多年创建的正式证明，随后其强化学习（RL）算法1通过与形式证明系统的持续互动生成了1亿多个证明。这种对互动经验的关注使AlphaProof能够探索超出预先存在的正式证明范围的数学可能性，从而发现新颖和具有挑战性的问题的解决方案。非正式数学也通过用自我生成的数据取代专家生成的数据取得了成功；例如，DeepSeek最近的工作“强调了强化学习的力量和美妙之处：我们没有明确地教模型如何解决问题，而是简单地为它提供了正确的激励，它就能自主地发展出高级的问题解决策略。”[10]

我们的观点是，一旦体验式学习的全部潜力得到发挥，就会出现令人难以置信的新能力。体验时代可能会以以下智能体和环境为特征，除了从大量的体验数据中学习外，还将在以下几个方面突破以人为本的人工智能系统的局限性：

- 智能体将生活在体验流中，而不是短暂的互动片段。
- 它们的行动和观察将丰富地扎根于环境中，而不仅仅是通过人类对话进行互动。
- 它们的奖励将扎根于它们对环境的体验，而不是来自人类的预先判断。
- 它们将计划和/或推理经验，而不是仅仅用人类的术语进行推理。

我们认为，今天的技术，通过适当选择的算法，已经提供了足够强大的基础来实现这些突破。此外，人工智能社区对这一议程的追求将刺激在这些方向上的新创新，从而迅速推动人工智能朝着真正超人的智能体发展。

### 流

体验式智能体可以在一生中不断学习。在人类数据时代，基于语言的人工智能主要关注短期的互动情节：例如，用户提出一个问题，智能体（可能在经过几个思考步骤或工具使用动作之后）做出回应。通常，很少或没有信息从一个情节传递到下一个情节，从而排除了任何随时间的适应性。此外，智能体只追求当前情节中的结果，例如直接回答用户的问题。相比之下，人类（和其他动物）存在于一个持续多年的行动和观察流中。信息在整个流中传递，他们的行为会根据过去的经验进行调整，以自我纠正和改进。此外，目标可以用延伸到未来很长时间的行动和观察来指定。例如，人类可能会选择行动来实现长期目标，如改善他们的健康、学习一门语言或取得科学突破。

强大的智能体应该有自己的体验流，像人类一样，在很长的时间尺度上发展。这将使智能体能够采取行动来实现未来的目标，并随着时间的推移不断适应新的行为模式。例如，连接到用户可穿戴设备的健康和保健智能体可以监测几个月的睡眠模式、活动水平和饮食习惯。然后，它可以提供个性化的建议、鼓励，并根据长期趋势和用户的具体健康目标调整其指导。同样，个性化的教育智能体可以跟踪用户在学习一门新语言方面的进展，识别知识差距，适应他们的学习风格，并在几个月甚至几年的时间内调整其教学方法。此外，科学智能体可以追求雄心勃勃的目标，如发现一种新材料或减少二氧化碳。这样的智能体可以分析长期以来的真实世界观察，开发和运行模拟，并提出真实世界的实验或干预措施。

在每种情况下，智能体都会采取一系列步骤，以便最大限度地提高长期成功的概率，达到既定目标。单个步骤可能不会提供任何直接的好处，或者在短期内甚至可能是有害的，但仍然可以在总体上对长期成功做出贡献。这与当前的人工智能系统形成了鲜明对比，当前的人工智能系统为请求提供即时响应，而没有任何能力衡量或优化其行为对环境的未来后果。

### 行动和观察

体验时代的智能体将在现实世界中自主行动。人类数据时代的LLMs主要关注人类特权的行动和观察，这些行动和观察将文本输出给用户，并将用户的文本输入到智能体中。这与自然智能截然不同，在自然智能中，动物通过运动控制和传感器与其环境互动。虽然动物，尤其是人类，可能会与其他动物交流，但这与运动感觉控制通过相同的界面发生，而不是通过特权通道发生。

长期以来，人们已经认识到LLMs也可以在数字世界中调用行动，例如通过调用API（例如，参见 [43]）。最初，这些能力主要来自人类对工具使用的例子，而不是来自智能体的经验。然而，编码和工具使用能力越来越多地建立在执行反馈 [17, 7, 12] 的基础上，智能体实际上运行代码并观察发生了什么。最近，新一波原型智能体已经开始以更普遍的方式与计算机互动，通过使用人类操作计算机时使用的相同界面 [3, 15, 24]。这些变化预示着从完全人类特权的通信到更自主的互动的转变，智能体能够在世界上独立行动。此类智能体将能够积极探索世界，适应不断变化的环境，并发现人类可能永远不会想到的策略。

这些更丰富的互动将提供一种自主理解和控制数字世界的方法。智能体可以使用“人类友好的”行动和观察，例如用户界面，这些界面自然地促进与用户的沟通和协作。智能体也可以采取“机器友好的”行动，即执行代码和调用API，从而使智能体能够自主地为其目标服务。在体验时代，智能体还将通过数字界面与现实世界互动。例如，科学智能体可以监控环境传感器，远程操作望远镜，或控制实验室中的机械臂以自主进行实验。

### 奖励

如果体验式智能体可以从外部事件和信号中学习，而不仅仅是从人类的偏好中学习呢？

以人为中心的LLMs通常会根据人类的预先判断来优化奖励：专家观察智能体的行动，并决定它是否是一个好的行动，或者在多个备选智能体行动中选择最好的智能体行动。例如，专家可能会判断健康智能体的建议、教育助手的教学或科学智能体建议的实验。这些奖励或偏好是由人类在没有后果的情况下确定的，而不是衡量这些行动对环境的影响，这意味着它们并没有直接植根于世界的现实中。以这种方式依赖人类的预先判断通常会导致智能体表现的不可逾越的上限：智能体无法发现人类评估者低估的更好策略。为了发现远远超出现有人类知识的新想法，有必要使用基于现实的奖励：来自环境本身的信号。例如，健康助手可以将用户的健康目标转化为基于诸如他们的静息心率、睡眠时长和活动水平等信号的奖励，而教育助手可以使用考试成绩来为语言学习提供基于现实的奖励。同样，一个以减少全球变暖为目标的科学智能体可能会使用基于二氧化碳水平的经验观察的奖励，而发现更坚固材料的目标可能会基于材料模拟器中的测量值组合，例如抗拉强度或杨氏模量。

基于现实的奖励可能来自智能体环境中的人类2。例如，人类用户可以报告他们是否觉得蛋糕美味、运动后有多疲劳或头痛的程度，从而使助手智能体能够提供更好的食谱，改进其健身建议或改进其推荐的药物。这些奖励衡量了智能体的行动在其环境中的后果，并且最终应该比人类专家预先判断提议的蛋糕食谱、运动计划或治疗方案能够提供更好的帮助。

如果奖励不是来自人类数据，那么它们来自哪里呢？一旦智能体通过丰富的行动和观察空间（见上文）连接到世界，将不会缺少基于现实的信号来为奖励提供基础。事实上，世界充斥着诸如成本、错误率、饥饿感、生产力、健康指标、气候指标、利润、销售额、考试成绩、成功、访问量、产量、股票、点赞数、收入、快乐/痛苦、经济指标、准确性、功率、距离、速度、效率或能源消耗等量。此外，还有无数其他信号来自特定事件的发生，或者来自原始观察和行动序列中派生的特征。

原则上，人们可以创建各种不同的智能体，每个智能体都将一个基于现实的信号优化作为其奖励。有一种观点认为，即使是单个这样的奖励信号，如果以非常有效的方式进行优化，也可能足以诱导出广泛的能力智能 [34] 3。这是因为在复杂的环境中实现一个简单的目标可能通常需要掌握各种技能。

然而，追求单一奖励信号表面上似乎并不符合通用人工智能的要求，即可以可靠地引导其朝着任意用户期望的行为发展。那么，自主优化基于现实的非人类奖励信号是否与现代人工智能系统的要求背道而驰？我们认为不一定是这样，通过勾勒出一个可能满足这些要求的方法；其他方法也可能是可行的。

这个想法是根据用户引导的方式，灵活地调整基于现实信号的奖励。例如，奖励函数可以由一个神经网络定义，该神经网络将智能体与用户和环境的交互作为输入，并输出一个标量奖励。这允许奖励以取决于用户目标的方式选择或组合来自环境的信号。例如，用户可能会指定一个广泛的目标，例如“改善我的健康状况”，并且奖励函数可能会返回用户心率、睡眠时长和步数的函数。或者，用户可能会指定一个“帮助我学习西班牙语”的目标，并且奖励函数可能会返回用户的西班牙语考试成绩。

此外，用户可以在学习过程中提供反馈，例如他们的满意度，这可以用于微调奖励函数。然后，奖励函数可以随时间调整，以改进其选择或组合信号的方式，并识别和纠正任何偏差。这也可以理解为一个双层优化过程，它优化用户反馈作为顶层目标，并优化来自环境的基于现实的信号作为底层。4 通过这种方式，少量的人类数据可以促进大量的自主学习。

## 计划和推理

体验时代是否会改变智能体计划和推理的方式？最近，在使用能够通过语言进行推理或“思考”的LLMs [23, 14, 10] 方面取得了重大进展，通过在输出响应之前遵循一个思维链 [16]。从概念上讲，LLMs可以充当通用计算机 [30]：LLM可以在其自身的上下文中附加标记，从而使其能够在输出最终结果之前执行任意算法。

在人类数据时代，这些推理方法被明确设计为模仿人类的思维过程。例如，LLMs已被提示发出类似于人类的思维链 [16]，模仿人类思维的痕迹 [42]，或加强与人类示例相匹配的思维步骤 [18]。推理过程可能会被进一步微调，以产生与人类专家确定的正确答案相匹配的思维痕迹 [44]。

然而，人类语言极不可能提供通用计算机的最佳实例。肯定存在更有效的思维机制，使用非人类语言，例如可以利用符号、分布式、连续或可微的计算。原则上，自我学习系统可以通过从经验中学习如何思考来发现或改进这些方法。例如，AlphaProof学习以与人类数学家完全不同的方式正式证明复杂的定理 [20]。

此外，通用计算机的原理仅解决了智能体的内部计算；它没有将其连接到外部世界的现实。接受过模仿人类思想甚至与人类专家答案相匹配的训练的智能体，可能会继承嵌入在该数据中的错误的思维方法，例如错误的假设或固有的偏见。例如，如果一个智能体接受过使用5000年前的人类思想和专家答案进行推理的训练，它可能会用万物有灵论来推理物理问题；1000年前它可能会用有神论的术语进行推理；300年前它可能会用牛顿力学的术语进行推理；而50年前它可能会用量子力学的术语进行推理。超越每一种思维方法都需要与现实世界互动：提出假设、进行实验、观察结果并相应地更新原则。同样，智能体必须基于真实世界的数据，才能推翻错误的思维方法。这种基于现实为智能体提供了一个反馈循环，使其能够针对现实检验其继承的假设，并发现不受当前主要人类思维模式限制的新原则。如果没有这种基于现实，智能体无论多么复杂，都将成为现有人类知识的“回音室”。为了超越这一点，智能体必须积极参与世界，收集观察数据，并使用这些数据迭代地改进其理解，从而在许多方面反映了推动人类科学进步的过程。

将思维直接扎根于外部世界的一种可能方法是构建一个世界模型 [37]，该模型预测智能体行动对世界的影响，包括预测奖励。例如，健康助手可能会考虑推荐当地的健身房或健康播客。智能体的世界模型可能会预测用户的心率或睡眠模式在采取此行动后会发生怎样的变化，以及预测与用户的未来对话。这允许智能体直接根据其自身的行动及其对世界的因果关系进行计划 [36, 29]。随着智能体在其整个体验流中继续与世界互动，其动态模型会不断更新，以纠正其预测中的任何错误。给定一个世界模型，智能体可以应用可扩展的计划方法来提高智能体的预测性能。

计划和推理方法不是互斥的：智能体可以在计划期间应用内部LLM计算来选择每个行动，或者模拟和评估这些行动的后果。

### 为什么是现在？

从经验中学习并不是什么新鲜事。强化学习系统以前已经掌握了许多复杂的任务，这些任务是在具有明确奖励信号的模拟器中表示的（参见图1中的“模拟时代”）。例如，强化学习方法通过在诸如双陆棋 [39]、围棋 [31]、国际象棋 [32]、扑克 [22, 6] 和策略棋 [26] 等棋盘游戏；诸如Atari [21]、星际争霸II [40]、Dota 2 [4] 和 Gran Turismo [41] 等视频游戏；诸如魔方 [1] 等灵巧操作任务；以及诸如数据中心冷却 [13] 等资源管理任务的自我对弈中等于或超过了人类的表现。此外，诸如AlphaZero [33] 等强大的强化学习智能体在神经网络的大小、交互体验的数量和思考时间的持续时间内表现出令人印象深刻且可能无限的可扩展性。然而，基于这种模式的智能体并没有跨越模拟（具有奇异的、精确定义的奖励的封闭问题）到现实（具有看似定义不明确的多种奖励的开放式问题）之间的差距。

![](https://cdn-mineru.openxlab.org.cn/extract/1e7f9359-ece3-4711-ac39-eb36e44905bf/eda9e0260e258e202900d724910a60e7f19e4b39f7a68f56b526fdde29970edd.jpg)
图1：主要人工智能范式的草图年表。y轴表示该领域总工作量和计算量中专注于强化学习的比例。

人类数据时代提供了一个有吸引力的解决方案。大量的人类数据语料库包含适用于各种任务的自然语言示例。与模拟时代的更狭隘的成功相比，在此数据上训练的智能体实现了一系列广泛的能力。因此，体验式强化学习的方法在很大程度上被抛弃，转而支持更通用的智能体，从而导致了以人为中心的人工智能的广泛转变。

然而，在这种转变中失去了一些东西：智能体自我发现知识的能力。例如，AlphaZero发现了国际象棋和围棋的全新策略，改变了人类玩这些游戏的方式 [28, 45]。体验时代将使这种能力与人类数据时代实现的任务通用性水平相协调。如上所述，当智能体能够在真实世界的体验流中自主地行动和观察 [11]，并且奖励可以灵活地连接到大量基于现实的真实世界信号中的任何一个时，这将成为可能。与复杂的真实世界行动空间 [3, 15, 24] 交互的自主智能体的出现，以及可以解决丰富推理空间中开放式问题的强大强化学习方法 [20, 10]，表明向体验时代的转变迫在眉睫。

## 强化学习方法

强化学习（RL）有着悠久的历史，它深深植根于自主学习，即智能体通过与环境的直接互动为自己学习。早期的强化学习研究产生了一套强大的概念和算法。例如，时间差分学习 [35] 使智能体能够估计未来的奖励，从而带来了诸如双陆棋 [39] 中超人的表现之类的突破。由乐观或好奇心驱动的探索技术被开发出来，以帮助智能体发现创造性的新行为并避免陷入次优的例程 [2]。诸如Dyna算法之类的方法使智能体能够构建和学习其世界的模型，从而使它们能够计划和推理未来的行动 [36, 29]。诸如选项和间/内选项学习之类的概念促进了时间抽象，使智能体能够推理更长的时间跨度，并将复杂的任务分解为可管理的子目标 [38]。

然而，以人为中心的LLMs的兴起将重点从自主学习转移到利用人类知识上。诸如RLHF（来自人类反馈的强化学习）[9, 25] 之类的技术以及使语言模型与人类推理对齐的方法 [44] 被证明是非常有效的，从而推动了人工智能能力的快速发展。这些方法虽然强大，但经常绕过核心强化学习概念：RLHF通过调用人类专家代替机器估计值来回避了对价值函数的需求，来自人类数据的强大先验减少了对探索的依赖，并且以人为中心的术语进行推理减少了对世界模型和时间抽象的需求。

然而，有人可能会说，这种范式的转变把脏水和孩子一起倒掉了。虽然以人为中心的强化学习已经实现了前所未有的广泛行为，但它也对智能体的表现施加了新的上限：智能体无法超越现有的人类知识。此外，人类数据时代主要关注为不基于现实的人类互动短事件而设计的强化学习方法，并且不适合基于现实的自主互动的长时间流。

体验时代提供了一个重新审视和改进经典强化学习概念的机会。这个时代将带来思考奖励函数的新方法，这些奖励函数可以灵活地基于观察数据。它将重新审视价值函数以及从具有尚未完成的序列的长流中估计它们的方法。它将带来有原则但实用的真实世界探索方法，这些方法可以发现与人类先验完全不同的新行为。将开发出新的世界模型方法，这些方法可以捕获基于现实的互动的复杂性。用于时间抽象的新方法将使智能体能够在越来越长的时间范围内根据经验进行推理。通过建立在强化学习的基础上并将强化学习的核心原则适应于这个新时代的挑战，我们可以释放自主学习的全部潜力，并为真正超人的智能铺平道路。

# 后果

人工智能智能体通过与世界的互动来学习的体验时代的到来，预示着一个与我们以前见过的任何事物都截然不同的未来。这种新模式虽然提供了巨大的潜力，但也提出了重要的风险和挑战，需要仔细考虑，包括但不限于以下几点。

从积极的方面来看，体验式学习将释放前所未有的能力。在日常生活中，个性化助手将利用持续的体验流来适应个人在健康、教育或职业方面的长期需求。也许最具有变革性的是科学发现的加速。人工智能智能体将自主设计和进行材料科学、医学或硬件设计等领域的实验。通过不断地从自己的实验结果中学习，这些智能体可以迅速探索知识的新领域，从而以前所未有的速度开发出新的材料、药物和技术。

然而，这个新时代也带来了重大而新颖的挑战。虽然人类能力的自动化有望提高生产力，但这些改进也可能导致失业。智能体甚至可能能够表现出以前被认为是人类独有领域的能力，例如长期解决问题、创新以及对现实世界后果的深刻理解。

此外，虽然存在围绕滥用任何人工智能的一般担忧，但能够自主地在更长时间内与世界互动以实现长期目标的智能体可能会带来更高的风险。默认情况下，这为人类干预和调解智能体的行为提供了更少的机会，因此需要高度的信任和责任。摆脱人类数据和人类思维模式也可能使未来的AI系统更难以解释。

然而，虽然承认体验式学习会增加某些安全风险，并且肯定需要进一步的研究以确保向体验时代的平稳过渡，但我们也应该认识到，它也可能提供一些重要的安全益处。

首先，体验式智能体知道它所处的环境，并且其行为可以随着时间的推移适应环境的变化。任何预编程系统，包括固定的AI系统，都可能不知道其环境上下文，并且可能无法适应其部署到的不断变化的世界。例如，关键的硬件可能会发生故障，疫情可能会导致快速的社会变革，或者新的科学发现可能会引发快速的技术发展。相比之下，体验式智能体可以观察并学会规避故障硬件，适应快速的社会变革，或拥抱和建立在新的科学技术之上。也许更重要的是，智能体可以识别出何时其行为正在引发人类的担忧、不满或痛苦，并适应性地修改其行为以避免这些负面后果。

其次，智能体的奖励函数本身可以通过经验进行调整，例如使用前面描述的双层优化（参见“奖励”部分）。重要的是，这意味着可以通过反复试验来逐步纠正未对齐的奖励函数。例如，与其盲目地优化诸如最大化纸夹数量 [5] 之类的信号，不如在纸夹生产消耗地球上的所有资源之前，根据人类的担忧迹象来修改奖励函数。这类似于人类互相设定目标的方式，然后在观察到人们玩弄系统、忽视长期福祉或造成不希望的负面后果时调整这些目标；虽然也像人类的目标设定一样，但不能保证完美的对齐。

最后，依赖物理经验的进步本质上受到在现实世界中执行行动并观察其后果所需的时间的限制。例如，即使有AI辅助设计，新药的开发仍然需要无法一夜之间完成的真实世界试验。这可能会对潜在的AI自我改进速度提供自然制动。

# 结论

体验时代标志着人工智能发展的一个关键时刻。智能体将在今天坚实的基础之上，但超越人类数据衍生的局限性，越来越多地从自己与世界的互动中学习。智能体将通过丰富的观察和行动自主地与环境互动。他们将在终生体验流中继续适应。他们的目标将可以直接用于任何基于现实的信号的组合。此外，智能体将利用强大的非人类推理，并构建基于智能体行动对其环境影响的计划。最终，体验数据将超越人类生成数据的规模和质量。这种范式转变，伴随着强化学习算法的进步，将在许多领域释放出超越任何人类所拥有的新能力。

# 致谢

作者感谢Thomas Degris、Rohin Shah、Tom Schaul和Hado van Hasselt的有益评论和讨论。

# 参考文献

- [1] I. Akkaya, M. Andrychowicz, M. Chociej, M. Litwin, B. McGrew, A. Petron, A. Paino, M. Plappert, G. Powell, R. Ribas, J. Schneider, N. Tezak, J. Tworek, P. Welinder, L. Weng, Q. Yuan, W. Zaremba, 和 L. Zhang. Solving Rubik’s cube with a robot hand, 2019. 
- [ ] [2] S. Amin, M. Gomrokchi, H. Satija, H. van Hoof, 和 D. Precup. A survey of exploration methods in reinforcement learning, 2021.
- [ ] [3] Anthropic. Introducing computer use, a new Claude 3.5 Sonnet, and Claude 3.5 Haiku. https://www. anthropic.com/news/3-5-models-and-computer-use, 2024. 
- [ ] [4] C. Berner, G. Brockman, B. Chan, V. Cheung, P. Debiak, C. Dennison, D. Farhi, Q. Fischer, S. Hashme, C. Hesse, R. J´ozefowicz, S. Gray, C. Olsson, J. Pachocki, M. Petrov, H. P. d. O. Pinto, J. Raiman, T. Salimans, J. Schlatter, J. Schneider, S. Sidor, I. Sutskever, J. Tang, F. Wolski, 和 S. Zhang. Dota 2 with large scale deep reinforcement learning, 2019. 
- [ ] [5] N. Bostrom. Ethical issues in advanced artificial intelligence. https://nickbostrom.com/ethics/ai, 2003.
- [6] N. Brown 和 T. Sandholm. Superhuman AI for heads-up no-limit poker: Libratus beats top professionals. Science, 359(6374):418–424, 2018.
- [ ] [7] X. Chen, M. Lin, N. Sch¨arli, 和 D. Zhou. Teaching large language models to self-debug, 2023. 
- [ ] [8] N. Chentanez, A. Barto, 和 S. Singh. Intrinsically motivated reinforcement learning. In L. Saul, Y. Weiss, 和 L. Bottou, 编辑, Advances in Neural Information Processing Systems, volume 17. MIT Press, 2004. 
- [ ] [9] P. F. Christiano, J. Leike, T. Brown, M. Martic, S. Legg, 和 D. Amodei. Deep reinforcement learning from human preferences. In I. Guyon, U. V. Luxburg, S. Bengio, H. Wallach, R. Fergus, S. Vishwanathan, 和 R. Garnett, 编辑, Advances in Neural Information Processing Systems, volume 30. Curran Associates, Inc., 2017.
- [10] DeepSeek AI. DeepSeek-R1: Incentivizing reasoning capability in LLMs via reinforcement learning. arXiv preprint arXiv:2501.12948, 2025.
- [11] M. Elsayed, G. Vasan, 和 A. R. Mahmood. Streaming deep reinforcement learning finally works, 2024.
- [12] J. Gehring, K. Zheng, J. Copet, V. Mella, Q. Carbonneaux, T. Cohen, 和 G. Synnaeve. Rlef: Grounding code llms in execution feedback with reinforcement learning, 2025.
- [13] Google DeepMind. Deepmind AI reduces google data centre cooling bill by $40\%$ . https://deepmind.google/discover/blog/ deepmind-ai-reduces-google-data-centre-cooling-bill-by-40/, 2016.
- [14] Google DeepMind. Gemini: Flash thinking. https://deepmind.google/technologies/gemini/ flash-thinking/, 2024.
- [15] Google DeepMind. Project Mariner. https://deepmind.google/technologies/ project-mariner, 2024.
- [16] T. Kojima, S. S. Gu, M. Reid, Y. Matsuo, 和 Y. Iwasawa. Large language models are zero-shot reasoners. In S. Koyejo, S. Mohamed, A. Agarwal, D. Belgrave, K. Cho, 和 A. Oh, 编辑, Advances in Neural Information Processing Systems, volume 35, pages 22199–22213. Curran Associates, Inc., 2022.
- [17] H. Le, Y. Wang, A. D. Gotmare, S. Savarese, 和 S. C. H. Hoi. CodeRL: Mastering code generation through pretrained models and deep reinforcement learning, 2022.
- [18] H. Lightman, V. Kosaraju, Y. Burda, H. Edwards, B. Baker, T. Lee, J. Leike, J. Schulman, I. Sutskever, 和 K. Cobbe. Let’s verify step by step, 2023.
- [19] H. Mahdavi, A. Hashemi, M. Daliri, P. Mohammadipour, A. Farhadi, S. Malek, Y. Yazdanifard, A. Khasahmadi, 和 V. Honavar. Brains vs. bytes: Evaluating llm proficiency in olympiad mathematics, 2025.
- [20] H. Masoom, A. Huang, M. Z. Horv´ath, T. Zahavy, V. Veeriah, E. Wieser, J. Yung, L. Yu, Y. Schroecker, J. Schrittwieser, O. Bertolli, B. Ibarz, E. Lockhart, E. Hughes, M. Rowland, G. Margand, A. Davies, D. Zheng, I. Beloshapka, I. von Glehn, Y. Li, F. Pedregosa, A. Velingker, G. ˇZuzˇic´, O. Nash, B. Mehta, P. Lezeau, S. Mercuri, L. Wu, C. Soenne, T. Murrills, L. Massacci, A. Yang, A. Mandhane, T. Eccles, E. Ayg¨un, Z. Gong, R. Evans, S. Mokr´a, A. Barekatain, W. Shang, H. Openshaw, F. Gimeno, D. Silver, 和 P. Kohli. AI achieves silver-medal standard solving International Mathematical Olympiad problems. https://deepmind.google/discover/ blog/ai-solves-imo-problems-at-silver-medal-level/, 2024.
- [21] V. Mnih, K. Kavukcuoglu, D. Silver, A. A. Rusu, J. Veness, M. G. Bellemare, A. Graves, M. Riedmiller, A. K. Fidjeland, G. Ostrovski, S. Petersen, C. Beattie, A. Sadik, I. Antonoglou, H. King, D. Kumaran, D. Wierstra, S. Legg, 和 D. Hassabis. Human-level control through deep reinforcement learning. Nature, 518(7540):529–533, 2015.
- [22] M. Moravˇc´ık, M. Schmid, N. Burch, V. Lisy\`, D. Morrill, N. Bard, T. Davis, K. Waugh, M. Johanson, 和 M. Bowling. Deepstack: Expert-level artificial intelligence in heads-up no-limit poker. Science, 356(6337):508–513, 2017.
- [23] OpenAI. Openai o1 mini: Advancing cost-efficient reasoning. https://openai.com/index/ openai-o1-mini-advancing-cost-efficient-reasoning/, 2024.
- [24] OpenAI. Introducing Operator. https://openai.com/index/introducing-operator, 2025.
- [25] L. Ouyang, J. Wu, X. Jiang, D. Almeida, C. L. Wainwright, P. Mishkin, C. Zhang, S. Agarwal, K. Slama, A. Ray, J. Schulman, J. Hilton, F. Kelton, L. Miller, M. Simens, A. Askell, P. Welinder, P. Christiano, J. Leike, 和 R. Lowe. Training language models to follow instructions with human feedback, 2022.
- [26] J. Perolat, B. D. Vylder, D. Hennes, E. Tarassov, F. Strub, V. de Boer, P. Muller, J. T. Connor, N. Burch, T. Anthony, S. McAleer, R. Elie, S. H. Cen, Z. Wang, A. Gruslys, A. Malysheva, M. Khan, S. Ozair, F. Timbers, T. Pohlen, T. Eccles, M. Rowland, M. Lanctot, J.-B. Lespiau, B. Piot, S. Omidshafiei, E. Lockhart, L. Sifre, N. Beauguerlange, R. Munos, D. Silver, S. Singh, D. Hassabis, 和 K. Tuyls. Mastering the game of Stratego with model-free multiagent reinforcement learning. Science, 378(6623):990–996, 2022.
- [27] I. Petrov, J. Dekoninck, L. Baltadzhiev, M. Drencheva, K. Minchev, M. Balunovic´, N. Jovanovi´c, 和 M. Vechev. Proof or bluff? evaluating llms on 2025 usa math olympiad, 2025.
- [28] M. Sadler 和 N. Regan. Game Changer. New in Chess, 2019.
- [29] J. Schrittwieser, I. Antonoglou, T. Hubert, K. Simonyan, L. Sifre, S. Schmitt, A. Guez, E. Lockhart, D. Hassabis, T. Graepel, T. P. Lillicrap, 和 D. Silver. Mastering Atari, Go, chess and shogi by planning with a learned model. Nature, 588:604 – 609, 2019.
- [30] D. Schurmanns. Memory augmented large language models are computationally universal. arXiv preprint arXiv:2501.12948, 2023.
- [31] D. Silver, A. Huang, C. J. Maddison, A. Guez, L. Sifre, G. Van Den Driessche, J. Schrittwieser, I. Antonoglou, V. Panneershelvam, M. Lanctot, S. Dieleman, D. Grewe, J. Nham, N. Kalchbrenner, I. Sutskever, T. Lillicrap, M. Leach, K. Kavukcuoglu, T. Graepel, 和 D. Hassabis. Mastering the game of Go with deep neural networks and tree search. Nature, 529(7587):484–489, 2016.
- [32] D. Silver, T. Hubert, J. Schrittwieser, I. Antonoglou, M. Lai, A. Guez, M. Lanctot, L. Sifre, D. Kumaran, T. Graepel, T. Lillicrap, K. Simonyan, 和 D. Hassabis. A general reinforcement learning algorithm that masters chess, shogi, and Go through self-play. Science, 362(6419):1140–1144, 2018.
- [33] D. Silver, J. Schrittwieser, K. Simonyan, I. Antonoglou, A. Huang, A. Guez, T. Hubert, L. Baker, M. Lai, A. Bolton, Y. Chen, T. Lillicrap, F. Hui, L. Sifre, G. van den Driessche, T. Grapel, 和 D. Hassabis. Mastering the game of go without human knowledge. Nature, 550(7676):354–359, 2017.
- [34] D. Silver, S. Singh, D. Precup, 和 R. S. Sutton. Reward is enough. Artificial Intelligence, 299:103535, 2021.
- [35] R. S. Sutton. Learning to predict by the methods of temporal differences. Machine Learning, 3:9–44, 1988.
- [36] R. S. Sutton. Integrated architectures for learning, planning, and reacting based on approximating dynamic programming. In Proceedings of the Seventh International Conference on Machine Learning, pages 216–224. Morgan Kaufmann, 1990.
- [37] R. S. Sutton 和 A. G. Barto. Reinforcement Learning: An Introduction. The MIT Press, second edition, 2018.
- [38] R. S. Sutton, D. Precup, 和 S. Singh. Between mdps and semi-mdps: A framework for temporal abstraction in reinforcement learning. Artificial Intelligence, 112(1-2):181–211, 1999.
- [39] G. Tesauro. TD-Gammon, a self-teaching backgammon program, achieves master-level play. Neural Computation, 6(2):215–219, 1994.
- [40] O. Vinyals, I. Babuschkin, W. M. Czarnecki, M. Mathieu, A. Dudzik, J. Chung, D. Choi, R. Powell, T. Ewalds, P. Georgiev, J. Oh, D. Horgan, M. Kroiss, I. Danihelka, A. Huang, L. Sifre, T. Cai, J. P. Agapiou, M. Jaderberg, A. S. Vezhnevets, R. Leblond, T. Pohlen, V. Dalibard, D. Budden, Y. Sulsky, J. Molloy, T. L. Paine, C. Gulcehre, Z. Wang, T. Pfaff, Y. Wu, R. Ring, D. Yogatama, D. Wu¨ nsch, K. McKinney, O. Smith, T. Schaul, T. P. Lillicrap, K. Kavukcuoglu, D. Hassabis, C. Apps, 和 D. Silver. Grandmaster level in StarCraft II using multi-agent reinforcement learning. Nature, 575:350 – 354, 2019.
- [41] P. R. Wurman, S. Barrett, K. Kawamoto, J. MacGlashan, K. Subramanian, T. J. Walsh, R. Capobianco, A. Devlic, F. Eckert, F. Fuchs, L. Gilpin, P. Khandelwal, V. Kompella, H. Lin, P. MacAlpine, D. Oller, T. Seno, C. Sherstan, M. D. Thomure, H. Aghabozorgi, L. Barrett, R. Douglas, D. Whitehead, P. D¨urr, P. Stone, M. Spranger, 和 H. Kitano. Outracing champion Gran Turismo drivers with deep reinforcement learning. Nature, 602(7896):223–228, 2022.
- [42] M. S. Yang, D. Schuurmans, P. Abbeel, 和 O. Nachum. Chain of thought imitation with procedure cloning. In S. Koyejo, S. Mohamed, A. Agarwal, D. Belgrave, K. Cho, 和 A. Oh, 编辑, Advances in Neural Information Processing Systems, volume 35, pages 36366–36381. Curran Associates, Inc., 2022.
- [43] S. Yao, J. Zhao, D. Yu, N. Du, I. Shafran, K. Narasimhan, 和 Y. Cao. React: Synergizing reasoning and acting in large language models. In 11th International Conference on Learning Representations, 2023.
- [44] E. Zelikman, J. M. Mu, N. D. Goodman, 和 G. Poesia. Star: Bootstrapping reasoning with reasoning. Advances in Neural Information Processing Systems, 35:24170–24184, 2022.
- [45] Y. Zhou. Rethinking Opening Strategy: AlphaGo’s Impact on Pro Play. CreateSpace Independent, 2018.

---

