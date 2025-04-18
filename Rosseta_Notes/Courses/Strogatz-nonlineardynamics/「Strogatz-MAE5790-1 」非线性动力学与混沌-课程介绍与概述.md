

## 内容简介
- 视频链接：[MAE5790-1 Course introduction and overview](https://www.youtube.com/watch?v=ycJEoqmQvwg&list=PLbN57C5Zdl6j_qJA-pARJnKsmROzPnO9V)
- 视频号链接：[Cornell MAE](https://www.youtube.com/@cornellmae1636)
- 作者：[个人网站](https://www.stevenstrogatz.com/)

### 导言

本篇内容整理自康奈尔大学 MAE5790《非线性动力学与混沌》课程的首次讲座，由 Steven Strogatz 教授主讲。作为课程的开篇，本次讲座旨在为学习者提供一个全面的引导，内容涵盖了课程的基本管理信息、学习要求、核心概念的引入以及学科发展的宏观视角。

讲座首先介绍了课程的组织安排，包括教材选用、评分方式、沟通渠道（Piazza 平台）以及对作业完成方式和学术诚信的特别说明。随后，Strogatz 教授概述了学习本课程所需的先修知识，并强调了课程独特的学习风格——侧重于几何直觉、可视化思维，而非传统的繁复计算与证明。

讲座的核心部分在于对非线性动力学与混沌领域的历史脉络进行了梳理，从牛顿对三体问题的探索，经庞加莱的几何革命，到洛伦兹对混沌的再发现，直至费根鲍姆的普适性理论和学科的现代发展，勾勒出一幅学科演进的全景图。紧接着，教授阐述了研究动力系统的逻辑框架，引入相空间、相图等核心概念，并通过一个“二维网格”的视角将不同类型、不同维度的动力系统进行归类，明确了本课程的研习路径（从一维到三维非线性系统）。

最后，讲座初步探讨了一维非线性系统，以 $\dot{x} = \sin(x)$ 和 Logistic 方程为例，具体演示了如何运用图形化的相线分析方法来理解系统的不动点、稳定性及其长期行为，为后续更深入的学习奠定了基础。

### 内容纲要

```
MAE5790 课程介绍与概述
├── 课程介绍与管理
│   ├── 讲师与联系方式 (Steve Strogatz, 办公时间)
│   ├── 助教 (待定)
│   ├── 教材 (Strogatz 著, 提及盗版问题)
│   ├── 课程网站 (Piazza, 用于交流与发布信息)
│   ├── 授课形式 (课堂讲授, VideoNote 录像)
│   └── 评分与作业
│       ├── 组成 (作业, 期中, 期末 Take-home)
│       └── 作业政策 (允许参考/合作, 但需独立完成并注明来源)
├── 课程内容与要求
│   ├── 先修知识 (微积分曲线绘制, 线性代数, 高等微积分基础, 计算机求解 ODE)
│   ├── 有益背景 (科学基础)
│   ├── 课程水平与风格 (研究生/高年级本科生, 强调几何/直觉思维)
│   └── 课程结构简述 (1D -> 2D -> 3D 系统)
├── 非线性动力学与混沌的历史概述
│   ├── 起点: 牛顿 (1666, 微积分, 二体问题, 三体问题困境)
│   ├── 庞加莱 (约1890, 几何方法, 相空间, 混沌初现, 影响有限)
│   ├── 非线性振子时代 (1920s-1950s, 工程应用)
│   ├── 计算机与洛伦兹 (1960s, Lorenz 系统, 敏感依赖性, 再发现混沌)
│   ├── 数学进展 (1960s, Smale, KAM 理论)
│   ├── 混沌理论兴盛 (1970s)
│   │   ├── 罗伯特·梅 (迭代映射, Logistic 映射, Nature 论文)
│   │   ├── 曼德勃罗 (分形)
│   │   ├── 温弗里 (生物节律)
│   │   ├── 鲁厄尔 & 塔肯斯 (与湍流联系)
│   │   └── 约克 (命名 "Chaos")
│   ├── 费根鲍姆 (约1978, 普适性, 重整化群)
│   ├── 普及与应用 (1980s, 科普书籍, 流行文化, 实验证实)
│   ├── 后续发展 (1990s至今, 顶峰已过, 转向复杂系统/网络理论)
│   └── 问答环节
│       ├── Q: 太空竞赛与庞加莱工作? (A: 轨道规划者知晓, 低成本任务应用)
│       └── Q: 曼德勃罗受混沌启发? (A: 平行发展, 与分形联系)
├── 动力学的逻辑结构与方法
│   ├── 研究对象 (微分方程系统 $\dot{\mathbf{x}} = \mathbf{f}(\mathbf{x})$, 自治系统)
│   ├── 线性 vs 非线性 (定义, 例子: 简谐振子 vs 摆)
│   ├── 高阶方程转系统
│   ├── 几何方法 (庞加莱思想)
│   │   ├── 解作为相空间轨迹
│   │   ├── 相图 (Phase Portrait)
│   │   └── 目标: 不求解而理解行为
│   └── 动力学世界观 ("Big Grid")
│       ├── 分类依据 (线性/非线性 vs 维度 N)
│       ├── 放置实例 (物理, 数学, 生物系统)
│       ├── 课程路径 (1D -> 2D -> 3D 非线性)
│       └── 混沌出现位置 (N>=3)
└── 一维系统 (1D Systems: $\dot{x} = f(x)$)
    ├── 几何视角 (线上流动)
    ├── 分析方法 (绘制 $\dot{x}$ vs $x$ 图)
    │   ├── 流动方向 ($\dot{x}>0$ 右移, $\dot{x}<0$ 左移)
    │   └── 不动点 ($\dot{x}=0$, Fixed Points, $x^*$)
    ├── 不动点稳定性
    │   ├── 稳定 (Stable, 吸引, 实心圆)
    │   └── 不稳定 (Unstable, 排斥, 空心圆)
    ├── 示例 1: $\dot{x} = \sin(x)$
    │   ├── 对比解析解的复杂性
    │   └── 几何分析 (图像, 不动点, 稳定性, 长期行为, 定性 $x(t)$ 图像)
    └── 示例 2: Logistic 方程 ($\dot{x} = rx(1-x/K)$)
        ├── 生物学背景 (单位个体增长率, 环境容纳量)
        └── 几何分析 (抛物线图像, 不动点 0 与 K, 稳定性分析, 结论: 趋向 K)
```

---

## 课程介绍与概述 (MAE5790 - 非线性动力学与混沌)

大家好，欢迎来到 MAE5790 课程：非线性动力学与混沌。

你们可以叫我 Steve，很多研究生都这么叫，我自己的研究生也这么叫。或者你可以说 Professor 或 Professor Strogatz，怎么舒服怎么来。我的办公时间是周一 1:30 到 3:30，在数学系的 Malott Hall，533A 房间。

关于助教，我们还在安排中，确定后会通知大家。

教材是我多年前写的一本书。大家去校园书店看了吗？还在卖是吧？好的，所以如果你想要一本，应该能买到。网络上也有免费的盗版，我不推荐你们这样做，但这取决于你们自己。

还有什么呢？哦，网站。这学期我们用 Piazza。可能有些人已经收到了我或者 Piazza 发来的邮件了，对吧？如果没有，你应该自己去注册一下这门课。我已经把网址列在了讲义上，我们基本上就在那里活动了。如果你有邮件问题，最好发在那里，而不是直接写给我，因为其他学生可能会回答你，或者如果你知道答案，也可以帮助其他学生。所有的作业和其他信息都会在那里发布。

我们的朋友 VideoNote 正在给我们录像，至少是在录我。这意味着如果你们错过了课程，或者只是想回顾一下某个令人困惑的点，之后可以观看讲座录像。我想录像大概会在讲座结束后一两天内发布，并且带有很多很棒的功能，比如关键主题会被标记出来，你可以搜索它们，所以这些录像非常宝贵和方便。

我们这门课是有评分的。有作业，有期中考试，还有期末考试。期中考试将在课堂上进行，我看教室这么拥挤，考试条件会有点艰苦，但我不知道，我们尽力而为吧。期末考试将是带回家的形式（Take-home）。我会在学期最后一天之前布置，你们将有一周的时间来完成。这并不意味着需要一周的工作量，可能只需要大概 10 个小时的工作量，但你们会有一周的时间。我不希望有巨大的时间压力。总之，关于期末考试的细节我们稍后再谈，但基本上除了不能和别人合作之外，什么都可以做。你可以用网络，用电脑，查书，任何你想用的都可以。

作业我会在周四布置，下周四到期。现在，作业带来了一点小问题，因为这本书的答案手册在互联网上到处都是。这使得我很难因为你们做了作业就给你们学分，因为过去我发现有学生从网上抄答案。所以，与其把这变成一个学术诚信问题，我想说的是，你们被允许这样做，因为反正有些人会这么做，我也不想去强制执行关于这方面的诚信政策。所以，如果你觉得从其他来源（包括你最好的朋友或互联网）抄作业对你有帮助，那就去做吧，这是允许的。但我认为这是一种很糟糕的学习方式，而学习大概是你们来这里的目的。所以我建议你们自己做，或者和朋友一起做，然后自己写下答案。

正如我在这里关于学术诚信部分所说的，对于考试，规矩照旧，你不能抄袭或与人合作。但是，对于作业，你可以这样做。但我希望你们独立完成答案的书写。我的想法是，即使你在抄袭，用你自己的手写出来或者打出来，也可能多少有些好处。就是说，不要交答案手册的复印件，那也太离谱了。另外，如果你确实从别人那里抄了，或者你有合作者，请诚实地说明他们是谁。正如我一直说的，这样做没有惩罚，所以说实话就行。就像你写学术论文一样，如果你引用了某些内容，你会注明参考文献，否则就是剽窃。所以，养成注明帮助者的习惯。如果你不这样做，那才真的是学术诚信违规，我将不得不追究此事。我们不希望发生那种情况。

到目前为止有什么问题吗？

## 课程内容与要求

课程的主题嘛，我稍后会更详细地讨论，但粗略地说，我们从...嗯，你们可以在讲义上看到，我们会贯穿整本教材。

现在让我试着给你们更多关于先修知识要求的信息。我认为，绝对不可或缺的是微积分。你必须擅长曲线绘制。也就是说，当我给出一个曲线，$f(x)$，里面可能还带有参数，你应该能够轻松地用手画出那条曲线，而不是用图形计算器。你应该能够画出一个参数变化时的函数族曲线。你需要对微积分的这部分感到自如。

在某些时候，我们需要一些关于特征值和特征向量的线性代数知识。你可能需要一点点高等微积分知识，知道什么是雅可比矩阵。你当然需要知道如何求偏导数，一点点多元泰勒级数，但不多。大概就这些了。有一次我们会用到傅里叶分析，但我不会假设你们懂，到时候会讲解。

如果你有良好的科学背景，这将非常有帮助。所以，如果你懂大一物理，一点生物学，一些化学，你懂的科学越多越好。工程学背景也会有帮助，但这并非严格要求。我的意思是，这是一个背景广泛多样的班级，所以我需要用到的任何科学知识，我都会尽量概述。

课程的水平，主要是面向一年级研究生，也有很多优秀的本科生问是否可以选这门课，是的，可以。传统上，大二学生会觉得有点难，但如果你非常努力，也能做到。这是一门出人意料地有技巧性的课程。它看起来会很简单，但里面有很多微妙之处。所以你确实需要注意，思考的方式会和你习惯的不同。它不会像一门有很多计算或证明的数学课。它会涉及大量的可视化、几何思维和直觉。所以如果你喜欢这些，你会爱上这门课。但是，我想它会和你习惯的课程感觉不同。

哦，还有，我们会经常使用计算机。你应该能够自如地使用像 Maple、Matlab 或 Mathematica 这样的程序来求解微分方程，或者如果你不用这些，你可以自己写代码，可以用 Python。我不在乎你怎么做，但是，有时候你得用计算机来求解非线性微分方程。所以你应该预料到会做这些。网上也有一些你可以使用的东西，有一些小程序会很有帮助，我会推荐给你们。

好了，我想我准备好开始了，除非还有其他任何问题？都清楚了吗？没有问题。我喜欢互动式的课堂，所以任何时候都可以随时提问或评论。

## 非线性动力学与混沌的历史概述

让我先给你们两个关于这个学科的概述，然后我们会进入如何计算或可视化某些具体内容的细节。首先，让我们从历史开始。这个学科是关于什么的？它是如何演变的？

好的，这是历史概述。当然，这是一个非常简略的概述，我不会给出全面的论述，但这些是重点。

我认为开端是 1666 年。艾萨克·牛顿那时 24 岁。他在 1666 年成果丰硕，或多或少地发明了微积分，弄清了光学定律，发现了万有引力。对他来说是丰收的一年。他还有其他成果，但总之，就我们而言——说他发明了常微分方程其实不太准确，但他在这方面的进展远超同时代的任何人——在人类历史上首次解释了行星的轨道。开普勒已经根据第谷·布拉赫的数据计算出行星沿椭圆运动，并且还有他另外两条行星运动定律。牛顿可以从万有引力、加上微积分、再加上他的三大运动定律来解释所有这些。这就是动力学的开端。

但有趣的是，那时他解决的是我们所说的二体问题，也就是一个行星被太阳（或者地球或其他行星被太阳）的引力吸引。他由此能够解释椭圆轨道。但是，为了做到这一点，他不得不忽略太阳系中所有其他的行星，或者宇宙中所有其他物体。这就是为什么我们称之为二体问题——只有太阳和一个行星。但如果存在更多的天体呢？当然是有的，比如月球或其他行星。那就变成了三体问题或 N 体问题。牛顿解决不了。他实际上写信给他的一个朋友说，没有任何问题像三体问题那样让他头疼，尽管他称之为“月球问题”，但指的就是三体问题。所以他没有解决，其他人也没有。但人们为此努力了数百年。

所以我快进到 19 世纪末期，大约是 1890 年左右。那时仍然没有人解决三体问题。所有人都尝试过，欧拉、所有伟大的数学家，高斯。最终，庞加莱解释了问题所在。事实上，你根本无法真正“解决”三体问题。庞加莱引入了一种几何方法，相对于基于解析微积分的方法。

**问：** （听不清，似乎是问庞加莱是否证明了三体问题不可解）
**答：** 庞加莱或多或少地证明了你无法用寻找封闭形式解析表达式的传统意义来解决三体问题。也就是说，他揭示了——我不知道这是否算得上一个严格的证明，但可以商榷——但他确实以一种其他人未曾认识到的根本方式认识到了困难所在。如今我们会说，他的论证确实可以构造成一个证明。所以，是的，我会这么说。

但无论如何，通过他使用几何和可视化来补充（而非替代）微积分的工作，他看到了我们现在称之为“混沌”的东西。所以，他基于一个我们称之为“相空间”（Phase Space）的概念来进行几何研究。我希望稍后在讲座中向大家展示一些关于相空间的内容。但他的工作让我们得以一窥混沌。

人们喜欢说庞加莱发现了混沌。现在你可能想知道混沌的定义是什么，我们将在课程后期详细讨论。但现在，你应该把关键要素理解为：这是一种发生在确定性系统（Deterministic Systems）中的现象。确定性意味着系统由没有随机性的规则所支配，其中没有任何随机（stochastic）成分。它们是当前状态决定未来状态的系统。在这些确定性系统中，你有时会遇到非周期的（Aperiodic）、看似不可预测的（Seemingly Unpredictable）行为。

所以，在一个确定性系统中，“非周期”意味着它不重复，它不是简单的重复运动，也不是那种最终稳定到平衡状态的运动。它是某种既不重复也不稳定的东西，然而系统却是确定性的。它具有那种看起来有点随机的特性，也就是说，从长远来看，似乎很难预测它会做什么。它还具有这样一个特性，我们稍后会称之为对初始条件的敏感依赖性（Sensitive Dependence on Initial Conditions）。这是一个关键要素。

对初始条件的敏感依赖性意味着，如果你比较系统从某个初始条件开始的行为，然后想象稍微改变一下初始条件，只改变一点点，行为在一段时间内会保持大致相同，但随后非常迅速地——实际上是指数级快速地——两个解会分离开来。这就是我所说的敏感依赖性：微小的误差或微小的不确定性会被指数级快速放大。这使得长期预测变得不可能。但不要把它想成是随机性，因为在误差变得太大之前，短期预测仍然是可能的。

总之，这是庞加莱在他的工作中能看到的东西。你可能会认为这就是混沌热潮的开始，但事实并非如此。因为没有人真正理解庞加莱做了什么。还有一个有趣的事情是，他非常不擅长画画。事实上，他上大学的入学考试中，机械制图部分得了零分。他在绘画方面简直一塌糊涂。因此，在他的书和论文中，他倾向于不画出他所思考的东西的图片，尽管他非常擅长视觉化思考。所以他描述了某种形状，那是他所发现的混沌的本质，但他没有画图。我真的认为这妨碍了对这个学科的理解，没有人真正知道他在说什么。

另一个阻碍因素是，如果你记得，这是 19 世纪末，开始进入 20 世纪初。经典力学已经不是研究热点了。对吧？20 世纪初的热点是什么？量子力学刚刚起步，对吧？马克斯·普朗克，光电效应，还有相对论正在被创立。所以物理学的全部注意力已经不在三体问题上了。人们对那个问题已经厌倦了 200 年了。因此，庞加莱的工作基本上没什么反响，除了一些数学家注意到了它。但无论如何，这就是 19 世纪末的情况。

与此同时，大约从 1920 年代到 1950 年代，可以说是物理学和工程学中非线性振子（Nonlinear Oscillators）的伟大时代。例如，像收音机这样的东西被发明出来，它们基于真空管技术，而真空管是现在我们使用的半导体晶体管的前身。不过，收音机使用了这种有趣的真空管，它就是一个非线性振子。你也可以把雷达、用于通信的锁相环、激光器都看作是依赖非线性动力学才能工作的例子。所以如果你读这个时代的关于非线性动力学的书，会发现全是关于非线性振荡的，没有人谈论混沌，因为正如我说的，那基本上被遗忘了。

与此同时，大约在 1950 年，我们今天所知的计算机被发明出来了，部分是受到第二次世界大战以及冷战的刺激。高速可编程计算机出现了。这给动力学研究提供了一个强大的新工具，用于思考和可视化事物。

在 1960 年代，它被非常有力地使用，特别是由这门课的英雄之一，埃德·洛伦兹（Ed Lorenz）使用。他是麻省理工学院的气象学家和数学家。我们将在课程快结束时听到他的工作。他尤其以其在一个关于大气对流模型的混沌系统上的工作而闻名。他对天气预报感兴趣，这引导他建立了一个非常简化的关于大气中对流环流的流体动力学模型。他发现这个模型展现了那种不可预测的行为。他也没有使用“混沌”这个词，但他确实在 1963 年写了一篇非常重要的论文，我们将仔细研读，题目叫做《确定性非周期流》（Deterministic Nonperiodic Flow）之类的。这是一篇绝对优美且易读的论文，本应开启混沌革命。但他同样被忽视了，部分原因是因为他的工作发表在一个物理学家和数学家不读的期刊上——《大气科学杂志》（Journal of the Atmospheric Sciences），另一部分原因是因为他在流体动力学领域的同事说：“这是个荒谬的模型，这不是一个正确的大气模型，所以这什么也说明不了。”因此，没有人真正理解他所取得的巨大突破。

直到 20 世纪 70 年代中期，这才是混沌理论的繁荣时期。大约在 1975 年左右。哦，实际上，我应该再说一件 60 年代的事，那就是还有一位名叫斯蒂芬·斯梅尔（Stephen Smale）的数学家以及另外三位总是以缩写 KAM（Kolmogorov, Arnold, Moser）出现的数学家的工作。这是纯数学家们非常深刻的工作，基本上是沿着庞加莱开创并一直在纯数学领域延续下来的思路进行的，但世界其他地方，当然包括物理学家，并不知道这些。这是非常深刻和有趣的工作，如果你去上纯数学的混沌课程，会全是关于这类主题，而我描述的其他内容会少得多。我们不会过多讨论那些，但如果你想学，可以去上像 Math 6170 这样的课，可以学到这些东西。

总之，到了 1970 年代，一切都开始发生了。一位名叫鲍勃·梅（Bob May）的种群生物学家注意到了迭代映射（Iterated Mappings）中的混沌，就是这种形式的简单动力系统：$x_{n+1} = f(x_n)$。这里时间是离散的字母 n，就像 n=1, 2, 3, 4 那样。这些是简化的种群模型。你可以把它想象成一个你可以在计算器上编程的函数，输入一个数字，按下那个函数键，得到一个新数字，再应用那个函数，一直这样做。你可能在计算器上玩过这类游戏，比如反复按余弦键或平方根键。这些就是迭代映射。这可能是我们将要研究的继洛伦兹系统之后最简单的混沌模型。

梅还在 1976 年写了一篇论文，题目大概是《具有非常复杂动力学的简单动力系统》（Simple Dynamical Systems with Very Complicated Dynamics）或者《具有非常复杂动力学的简单非线性系统》（Simple Nonlinear Systems with Very Complicated Dynamics），发表在《自然》（Nature）杂志上，所有人都看到了。这让许多人意识到有一个完整的学科等待被研究。实际上，梅发出了他所谓的“福音式呼吁”（Evangelical Plea），认为我们应该停止只向大学生和研究生教授线性数学，应该向他们展示一旦允许系统是非线性的，一切规则都可能被打破，你可以发现各种各样的事情，是时候停止“撒谎”（指只教线性知识），开始在课堂上教授这些了。所以我们现在就在这里，试图这样做。总之，梅确实有力地阐述了这一点。特别地，他研究了我们称之为种群生物学中的 Logistic 方程（Logistic Equation），这是混沌最简单的模型之一，如今我们对其了解很多。

与此同时，还有本华·曼德勃罗（Benoit Mandelbrot），他对一切都有自己独特的看法，大致上开创了分形（Fractals）这门学科，后来发现分形与混沌密切相关。我们将在学期后面看到这种联系。所以那是在 70 年代开始发生的。

一位名叫阿特·温弗里（Art Winfree）的生物学家——康奈尔大学工程物理专业的本科毕业生——从数学的角度研究生物节律（Biological Rhythms）。也就是生物学中的非线性振子。他是我的导师，所以我对他和他的纪念有着特殊的感情。但他确实做了极其重要且有影响力的工作，将数学，特别是拓扑学引入了生物学。

最后，还有鲁厄尔（Ruelle）和塔肯斯（Takens）的工作，他们是纯数学家，但他们提出了一个想法：人们在像洛伦兹系统或这些迭代映射中看到的混沌，可能与经典力学中最大的未解之谜——湍流（Turbulence）问题有关。也就是说，纳维-斯托克斯方程（Navier-Stokes equations）或真实流体系统中的湍流到底是怎么回事？问题是，我们从混沌中学到的东西能否揭示这个古老的湍流问题？湍流只是混沌的另一个名字吗？还是它们不同？它们之间有什么关系？鲁厄尔和塔肯斯对此提出了一些非常有启发性的想法，激励了许多人。所有这些事情都促使混沌成为一个研究领域。大约在那个时候，马里兰大学的数学家吉姆·约克（Jim Yorke）给这个学科命了名。

总之，在 70 年代，它成了一个大事件。我认为整个事件的高潮大约在 1978 年。当时一位名叫米切尔·费根鲍姆（Mitchell Feigenbaum）的年轻物理学家发现了一个真正惊人的联系，介于 Logistic 映射和其他迭代映射的研究工作之间，他发现了…嗯，他发现了所有这些与当时主要在康奈尔大学进行的关于相变（Phase Transitions）的工作之间的联系，比如通过化学系的 Ben Widom 教授或物理系的 Ken Wilson（他后来因其在物理学中重整化群方面的工作获得了诺贝尔奖）的工作。所以这种联系是介于相变与混沌之间的。

费根鲍姆注意到的是后来被称为通往混沌的普适路径（Universal Route to Chaos）。也就是说，完全不同的物理、生物或化学系统可以以相同的方式（定量地）进入混沌状态。存在着关于从有序进入混沌过程的数学定律。费根鲍姆发现了这些定律，并发现，正如我说的，它们是普适的。它们在那些在科学层面上毫无共同之处的系统中以相同的方式发生。这真的很难理解，也难以置信，但他通过与统计物理学中相变的联系解释了这一点。这也是我们这门课以及整个混沌理论学科的一个高潮，我们将在学期后期研究这个问题。费根鲍姆在他的分析中使用的关键点是，正如我说的，重整化群（Renormalization Group）。我不假设你们上过研究生的统计力学课程，所以我将给你们一个简化版的重整化，并试图解释费根鲍姆做了什么。

到了 1980 年代…让我想想，我应该考虑一下你们大概是什么时候出生的，因为那对你们来说是一个很自然的时间点去关注。我想大概是 1990 年代，对吗？是的。我们还没到那里。好的，所以 1980 年代，这是混沌和非线性动力学变得时髦（fashionable）的时代。事实上，它们在此时非常热门（hot）。这是世界开始意识到它们的时候。分形也是如此。所以，火，火，火。然后，你知道，像一个高潮是詹姆斯·格莱克（James Gleick）关于混沌的书，名为《混沌：开创新科学》（Chaos: Making a New Science），在 1987 年出版，后来被翻译成 25 种语言，销量数百万册。每个人都在听说混沌。你可以买到印有分形的 T 恤、屏保、咖啡杯。斯蒂芬·斯皮尔伯格在 90 年代初拍了《侏罗纪公园》（Jurassic Park），其中的英雄之一是一位混沌理论家，他说：“我认为如果你们把这些恐龙放在这个公园里可能会有麻烦，也许你无法…也许很难预测会发生什么。”你们看过那部电影，对吧？他试图在劳拉·邓恩（Laura Dern）的手上解释蝴蝶效应，杰夫·戈德布拉姆（Jeff Goldblum）演的。对，戈德布拉姆。总之，是的，那是在 90 年代初，但《侏罗纪公园》的小说我想是稍早一点写的。

总之，流行文化开始意识到它。与此同时，有各种各样的实验证实了这些理论思想。在我们在理论部分之后，我会在各种物理和生物系统中描述这些实验。

然后，好吧，接下来发生了什么？然后你们出生了，那是 1990 年代。我想说，到那时，混沌理论基本上已经达到了顶峰。有一些关于混沌的工程应用的工作，比如利用混沌来加密私人通信。也就是说，混沌有什么用？它仅仅是个麻烦，还是我们能利用它？我们能以某种方式利用它吗？这成了一个问题。

但这个学科确实开始转向更复杂的事物。也就是说，不再是只有少数几个变量的系统——这才是混沌理论真正关注的，即只有三四个少量变量的系统中的复杂行为——兴趣开始转向现在所谓的复杂系统（Complex Systems），这些系统有数百万或数十亿个变量。因此，这成为了 90 年代以及进入 21 世纪至今的热门学科。复杂系统是当前研究的热点。还有网络理论（Network Theory）。

所以我想说，这大概是我们如今主要感兴趣的。混沌…如果你只精通混沌而没有其他专长，可能很难在大学获得终身教职。在数学系或许还可以，但从科学角度看，这个领域已经向前发展了。

这就是整个故事的一个非常快速的概述。

在我继续之前，你们想问什么或评论什么吗？

**问：** 在太空竞赛开始时，有人利用了庞加莱关于三体问题的工作吗？
**答：** 问题是：太空竞赛开始时，有人用庞加莱的三体问题工作吗？是的，事实证明，有一些…那些考虑很多关于卫星或飞船轨道（Trajectories）的规划者，他们当然知道庞加莱的工作以及后续的工作。我不知道他们是否需要它来完成像登月任务这样的事情，但混沌的思想确实以一些令人惊讶的方式被使用了…来执行非常低成本的任务。比如，实际上有一个著名的案例，我记不清是卫星还是什么飞行器，它遇到了麻烦，轨道工程师需要找到一种方法让它返回地球，但它上面实际上没有任何…只有一个非常弱的火箭。我的意思是，它只有一些小的姿态修正火箭，不足以用标准方式把它一直带回地球。但是利用混沌理论，实际上可以规划出一条几乎不需要能量的路线，你可以有点像…在太阳系中“冲浪”，并利用敏感依赖性，以一种实际上帮助你将这个受损的卫星用几乎没有燃料的方式带回来的方式。这真是太神奇了。这对那些更传统的轨道工程师来说是一个巨大的惊喜，他们认为你需要强大的火箭来引导你穿越太阳系。实际上，如果你知道怎么做，你可以沿着太阳系的引力及其混沌轨道“巡航”。这真是太神奇了。我在我的教学公司（The Teaching Company）课程中详细讲述了这个故事，如果你想看那些视频的话。

**问：** 曼德勃罗是受到混沌的启发吗？
**答：** 问题是：曼德勃罗是否受到混沌的启发？我认为他的工作是一个并行的流派。他知道混沌理论，但我不会说他是受其启发的。他思考了很多现实世界的问题，关于股票市场的行为，或者语言，云和星系的形状。他对自然界，自然的几何形状非常感兴趣。他确实做了现在称为曼德勃罗集（Mandelbrot set）的东西，这与迭代映射密切相关。所以他接近于研究混沌，但这并不是他的主要兴趣。只是碰巧我们在研究混沌时遇到的一些几何形状是分形，这就是主要的联系。

好了，让我把历史部分放在这里。现在试着谈谈我们正在做的逻辑方面，也就是所有这些背后的数学是什么。

## 动力学的逻辑结构与方法

我想在结束这部分时向你们展示一张大图，它将指导我们整个学期。所以当你们心中有了这张图之后，你们就会知道我们处于什么位置。

好的，动力学的逻辑结构。我在这里使用“动力学”（Dynamics）来指代整个学科，任何随时间变化的东西，我都认为是动力学的一部分，而不是你可能持有的狭隘观点，认为它必须与 $F=ma$ 之类的东西有关。它比 $F=ma$ 要大得多。

我们在这里真正研究的是微分方程。我们通常会写成这样：$\dot{\mathbf{x}} = \mathbf{f}(\mathbf{x})$。这里的记号是，点表示时间导数，带下划线的 $\mathbf{x}$ 表示一个向量。这是 $\mathbb{R}^n$ 中的某个元素。也就是说，如果你想用坐标写出来，它是 $(x_1, \dots, x_n)$。这是我的 $\mathbf{x}$。这个空间 $\mathbb{R}^n$，我们通常称之为相空间（Phase Space），有时我们可能称之为状态空间（State Space）。$\mathbf{f}$ 是某个给定的函数，通常是非线性函数。

如果我们用分量形式写出来，我们有：
$\dot{x}_1 = f_1(x_1, \dots, x_n)$
...
$\dot{x}_n = f_n(x_1, \dots, x_n)$

这是一个由 n 个耦合的常微分方程组成的系统，是我们思考的对象。这些 $f_i$ 是给定的函数，取决于我们研究的问题。

我们会说，如果右手边所有的 $x_i$ 都只以一次幂出现，那么系统是线性的（Linear）。我的意思是，没有乘积、幂次或 $x_i$ 的函数。也就是说，非线性项（Nonlinear terms）会是像 $x_1^2$ 这样的幂次，这是非线性项；或者 $x_2 \times x_3$ 是非线性的；或者像 $\sin(x_4)$ 或 $e^{x_5}$ 这样的东西。这些都是非线性项。如果我们想要一个线性系统，我们就不希望有任何这些项，我们只希望有 $x_i$ 本身乘以常数。

**问：** （听不清，似乎是问 rhs 是什么意思）
**答：** rhs，右手边（right hand side）。

你们在线性代数或线性微分方程课程中学过线性系统。

**问：** （听不清，似乎是问是否只关注自治系统）
**答：** 是的。问题是我们是否只对自治系统（Autonomous systems）感兴趣？记住，如果右手边不依赖于时间——正如我写的，它只依赖于 $x$ 变量，而不依赖于时间 $t$——那么就称为自治系统。我在这门课中将几乎完全坚持使用自治系统。有时候我们遇到带有外力（external forcing）的问题，这时在右手边引入时间 $t$ 是很自然的，但大多数情况下我们不会处理这些。在少数我们确实遇到的情况下，你仍然可以通过引入另一个变量将它们变成自治系统。你总可以说 $\dot{t} = 1$，然后你只需将状态空间视为 $(x_1, \dots, x_n, t)$，然后它就又变成了一个自治系统。我们喜欢这样做的原因是…我猜我应该在讲到这一点时澄清一下，但自治系统是我们进行几何研究的好地方。也就是说，我们希望将相空间想象成里面有箭头的向量场（Vector fields），而这些向量场不应该变化，以便我们的几何图像保持固定。如果你允许显式的对时间的依赖，向量会随时间摆动，这会弄乱几何图像。所以我倾向于不考虑非自治系统（Non-autonomous systems）。这在这个学科中是相当惯常的做法。

好吧。让我给你们…哦，顺便说一下，如果…嗯，任何不是线性的系统都称为非线性的（Nonlinear）。

让我们做几个快速的例子。一个经典的是简谐振子（Simple Harmonic Oscillator）。你们可能习惯写成类似 $m\ddot{x} + kx = 0$ 这样的形式。马上你就会注意到，这并不完全符合我们的框架，因为我说过我们只写一阶方程组，而这里有一个二阶导数 $\ddot{x}$。但我们可以通过一个小技巧把它转换到我们的框架中。为了把它写成 $\dot{\mathbf{x}} = \mathbf{f}(\mathbf{x})$ 的形式，我们引入一些新变量。让 $x_1 = x$，并且我们定义 $x_2 = \dot{x}$。有了这个选择，那么请注意 $\dot{x}_1$ 就等于 $x_2$，因为它们都等于 $\dot{x}$。而 $\dot{x}_2$ 就是 $\ddot{x}$，根据这个公式，它等于 $-kx_1/m$。

所以，这现在是一个我们说过将一直考虑的类型的系统：两个耦合的一阶方程。注意它是线性的，因为 $x_1$ 和 $x_2$ 只以一次幂出现。所以我们会认为这是一个线性二阶系统。

相比之下，像摆（Pendulum）这样的东西，忽略常数，你知道摆可以写成 $\ddot{x} + \sin(x) = 0$。使用我们刚才对 $x_1$ 和 $x_2$ 用的相同技巧，这个方程对应于 $\dot{x}_1 = x_2$，$\dot{x}_2 = -\sin(x_1)$。这将是非线性的，并且是二阶的，因为有这个非线性项 $\sin(x_1)$。$x_1$ 不仅仅以一次幂出现。你可能在某些课程中学过，要思考摆的问题，可以使用所谓的小角度近似，用 $x$ 代替 $\sin(x)$，但你认识到那只是抛弃了问题的本质。你现在把非线性系统变成了这个线性系统，这对于小角度是可以的，但如果你想理解像摆过顶时会发生什么这样的事情，那就不行了。所以你需要其他机制或方法来看待这个问题，这就是我们将要学习如何做的那类事情。

我们打算怎么做呢？如果你真的研究过摆的解析解，你可能知道它涉及到一种叫做椭圆函数（Elliptic Functions）的东西，现在几乎没人教了，尽管 Richard Rand 仍然教它们。所以你可以在他教的关于哈密顿动力学（Hamiltonian Dynamics）或非线性振动（Nonlinear Vibrations）的课程中了解到它们，我想这两门课他都会讲椭圆函数。但我们采取的不是这种方法。我们不打算使用复杂的特殊函数。相反，我们将使用图像。

这是我们的观点。这就是我提到的庞加莱关于几何是思考非线性系统关键的思想。对我们来说，问题的解——假设我知道 $x_1$ 作为时间的函数和 $x_2$ 作为时间的函数。如果我有一个这样的解，我可以把它看作是一个点沿着一个轨迹（Trajectory）在这个以 $x_1$ 和 $x_2$ 为坐标的空间中移动。也就是说，我们会画一张图，以 $x_1, x_2$ 为轴。然后，你知道，在初始时刻，$x_1$ 和 $x_2$ 在某个位置，这对应于这个 $x_1x_2$ 空间中的一个点。然后随着时间推移，那个点移动到某个其他的点，这意味着如果你把这些点连起来，你就会得到我所说的轨迹。你可以把这看作是那个轨迹的参数方程。

所以，与其从这个意义上思考解，我们将尝试思考这些相空间中的轨迹。这就是庞加莱的伟大思想：关键在于可以将这个构造反过来运行。也就是说，我们可以弄清楚轨迹看起来像什么，从而获得关于解的信息。而且我们可以在不解析地求解方程的情况下做到这一点。这就是我们要用的技巧。我们将使用某种论证来弄清楚轨迹看起来像什么，而无需实际显式地求解它们。

所以我们将尝试找到人们所说的相图（Phase Portrait）。我说的相图是指所有定性上不同的轨迹的图像。我们将尝试在不解析求解微分方程的情况下做到这一点。这就是整个课程的精髓所在。

好了，在我开始做一些数学推导之前的最后一件事是，我说过我想给你们课程的逻辑结构。现在我们有了相空间的概念，以及系统阶数（指我们将其写成系统时方程的数量）的概念，我们就可以做这件事了。让我试着给你们我所认为的动力学世界观，我将把整个宇宙映射到二维平面上，看看一切都适合放在哪里。你应该自己思考一下这张图有什么问题，因为它有很多问题，但尽管它不完美，我认为以这种方式看待事物还是很有帮助和有趣的。

也就是说，让我们给自己留点空间。画一个大的表格，区分线性和非线性系统。然后在顶部根据将控制方程写成系统时方程的数量来分类。我们将有只有一个变量的系统，或者两个，或者三个，或者比三个多但不是太多的系统。所以我说比如 $n>3$，这些是中等规模的系统。然后你可以有巨大的系统，$n \gg 1$，这里我大概想的是数百万或数十亿，或者可能是阿伏伽德罗常数的粒子，你知道，在气体中之类的。然后你还可以考虑连续统（Continuum），其中 $n$ 是无限的，在连续无限的意义上。

让我们来看看我们知道的一些东西，看看它们在这个粗略的分类方式中会落在哪里。我们已经讨论过两个了。简谐振子，用这种方法，会放在 $n=2$ 和线性的格子里。而我们说过，摆会放在 $n=2$ 但非线性的格子里。

像你可能在电子工程或大一物理中学过的 RC 电路，RC 电路会放在那里，它是一阶线性的。有人能想到任何你可能在某处见过的一阶非线性系统吗？有很多。

**问：** （听不清，似乎是提到 Logistic 增长）
**答：** 是的，种群的 Logistic 增长（Logistic Growth）就是一个。是的，一个简单的模型，比如培养皿中细菌的生长。正如你所说，Logistic 增长。还有跳伞者的问题，某人从飞机上跳下来，如果你问他们的速度作为时间的函数是多少，利用空气阻力是非线性阻力这一事实。所以跳伞者动力学（Skydiver Dynamics），速度将由一阶非线性方程控制。

所以你看，这些是你在大学早期教育中学到的东西。

对于连续但线性的，我想到的是像波动方程（Wave Equation），或者实际上麦克斯韦方程组（Maxwell's Equations）在电磁学中，对于电场和磁场是线性的。实际上，薛定谔方程（Schrödinger Equation）也是线性的。你知道，在量子力学中，你可以使用整个向量空间形式体系，希尔伯特空间（Hilbert space）是你的态矢量（bras 和 kets）所在的地方。所以那是一个线性理论。现在你可能想知道我为什么把它放在这个图表上，这明明与偏微分方程有关。这是因为我在想，你知道，如果我想描述由偏微分方程控制的某个东西的状态，我必须告诉你…比如说，如果是量子理论中的波函数，我必须告诉你波函数在连续空间中每一点的值，对吧？为了预测下一时刻的波函数是什么，你需要关于当前所有位置波函数的整个连续无穷多的信息。所以从这个意义上说，你可以认为偏微分方程存在于这一列。

而非线性的则包括像广义相对论（General Relativity），或者湍流问题，或者在生物学中，要理解心脏中最致命的心律失常——心室颤动（Fibrillation），它是由非线性偏微分方程控制的。

还有什么呢？我不知道，你可以…总之，你可以试着填充这个图表。但这是我们课程的计划。我们将从…好吧，首先，通常的主题是什么？我的意思是，这有点像大一物理，上面这些东西。那是大学教育的常规部分。做完这些之后，传统上会跳到很远的地方，去学习这类东西：热方程、波动方程等等。就是你在很多不同学科中学到的线性偏微分方程。所以那些往往是接下来的内容。

但我们将主要从这里开始，然后向这个方向前进：从一阶非线性系统到二阶，然后到三阶，洛伦兹系统就住在那里。所以混沌首次出现在 $n=3$ 这一列的非线性系统中。我们将证明一个定理，或者至少陈述并讨论这个定理，它表明在一维和二维非线性系统中没有混沌。出于拓扑原因，你需要三维或更多维。洛伦兹系统就是这种现象开始发生的一个例子。

还有我之前提到的分形和迭代映射，虽然它们严格来说不属于这里，因为我谈论迭代映射时想到的是离散时间，而不是连续的常微分方程，但就其复杂性而言，它们与洛伦兹系统相当。

所以我们的计划就是从左边开始，系统地贯穿整个学期向右推进。这就是我们的课程。然而，正如我所说，当今科学中最热门的很多东西都涉及网络。它们是非常大的非线性系统。这就是复杂系统的领域，在右下角。这真的是科学的前沿。我的意思是，我们对右下角发生的事情了解不多。我们知道一点点，很多工作正在那里进行。但是，这部分现在已经得到了很好的控制，这就是我们课程的内容。

好了，这就是整个学科的概述。在我们开始做一些实际工作之前，还有什么问题吗？我希望这对你们定位有所帮助。我意识到讨论花了点时间。没问题？好的。

## 一维系统 (1D Systems: $\dot{x} = f(x)$)

让我们现在把这个具体化，在一个例子中讨论相空间。我们刚才讨论的是书中的第一章。现在我们进入第二章。第二章只涉及这些非常简单的形式为 $\dot{x} = f(x)$ 的系统，其中 $x$ 是一个实数，只是一个单一的实数。所以这些是一维系统。称之为一维是因为我想从几何上把它们看作是在一条线上，一条一维线，比如实轴，x 轴上的流动（Flow）。

这里有一个我们如何分析这类系统的例子。假设我们有这个问题：$\dot{x} = \sin(x)$。你可以看到，这是一阶的，但由于正弦函数而是非线性的。现在，如果你在上微分方程课，传统的做法是你会从公式的角度思考。比如你可能会做一些分离变量的事情，得到 $dx / \sin(x) = dt$，然后两边积分。这是一个可分离的微分方程。这边的积分没问题，是 $t$ 加一个常数。但另一边需要一点记忆力。$dx / \sin(x)$…这和…它叫做余割（cosecant）。所以在你的记忆库里搜索，或者用 Wolfram Alpha 或 Mathematica 或 Maple 查一下 $\int \csc(x) dx$。或者，你知道，如果你记性好，你会记得一种写法是 $-\ln(|\csc(x) + \cot(x)|)$。还有其他等价的写法，但这至少是一种。

好的，所以得到了一些难看的函数。然后如果我们有一个初始条件，比如说 $t=0$ 时 $x=x_0$，那么你可以算出常数，你会发现 $t = \ln \left| \frac{\csc(x_0) + \cot(x_0)}{\csc(x) + \cot(x)} \right|$。我这里省略了一些代数步骤。我写这个主要是为了吓唬你们。也就是说，你应该觉得这虽然正确，但并不能提供多少启发。特别是，如何从中解出 $x$ 作为 $t$ 的函数并不那么明显，而这可能是你想要做的。如果你三角函数很厉害，你可以做到。我的意思是，你可以反解这个，但这需要一些工作。

但我的目的是想说，首先，$\sin$ 函数相当简单。如果我给你一个更讨厌的非线性函数，你甚至可能无法完成这个积分。所以我们用这个例子已经有点触及可能性的边缘了。我们能做这个积分，但即使如此，它也不是很有帮助。比如，假设我问你一个简单的问题，比如说 $x_0 = \pi/4$，那么长期行为是什么？也就是说，当 $t \to \infty$ 时，$x(t)$ 的极限是什么？这应该能从那个公式中直接读出来。但我认为，当你看着那个公式时，这并不那么明显。

然而，如果你画一张图，就更容易看清发生了什么。所以我想向你们展示我们将如何思考这个问题，不是通过解析方法，而是画图。我们画出 $\dot{x}$ 对 $x$ 的图像。我们把 $x$ 看作是一个假想粒子的位置。这个粒子被限制在 x 轴上运动，它无法离开那里，它只在这条一维线上移动。在这种解释下，$\dot{x}$ 就是它的速度。而 $\dot{x} = \sin(x)$ 这个微分方程，我们现在把它看作是一个向量场，实际上是 x 轴上的一个速度向量场。也就是说，它给了我们一个规则，表明当你在 $x$ 位置时，你的速度是 $\sin(x)$，这告诉粒子如何移动。

所以如果我画出 $\sin(x)$——这就是曲线绘制部分很重要的原因，你必须知道如何画 $\sin(x)$。好的，你能做到。所以这是 $\sin(x)$，大概是这样。现在这告诉我们什么？在这个拱形下方，$\dot{x}$ 是正的。这意味着粒子会向右移动，对吧？流向是向右的。因为当 $\dot{x}$ 为正时，意味着 $x$ 作为时间的函数是增加的。所以坐在这里的粒子会倾向于增加它的 $x$ 值，因此向右移动。而在这里，粒子看到的是负速度，所以它会向左移动。同样地，你可以填上其他区域。在这里我们会向那个方向移动，这里我们向这个方向移动。

你可能也注意到有些地方 $\dot{x}$ 是零。这些地方很重要。$\dot{x}=0$ 的点，我们称之为不动点（Fixed Points）。我们会用 $x^*$ 这个符号来表示不动点。因为当你在一个不动点时，你没有速度，所以你不会移动，当你受一阶方程（就像我们这里）控制时。也就是说，让我们用圆圈标出那些不动点。让我把这个画得大一点。

好的，我已经圈出了不动点。注意有两种类型的不动点。我们将通过以下方式来表示：对于箭头指向它们的不动点，我将把它们涂实；对于箭头背离它们的不动点，我将让它们保持空心。记住这里是 $x=0$。

现在你可以看到我们那个小问题的答案了。如果我们从这里的 $\pi/4$ 开始，你可以看到粒子会做什么。它只会开始向右移动。事实上，你可以通过查阅这个函数来看它向右移动的速度有多快。最初它的速度是这个数值 $\sin(\pi/4)$，也就是 $\sqrt{2}/2$。让我们实际在这里展示一下。我们可以定性地画出 $x$ 作为时间 $t$ 的函数。注意，我当然没有用任何余割之类的东西，我只是从图上凭感觉画的。我们在 $t=0$ 时在 $\pi/4$。我们最初会以 $\sin(\pi/4)$ 的斜率，也就是 $\sqrt{2}/2$，向上移动。

然后粒子向右移动，在某个时刻它会到达这个最大值的下方。在最大值处，$\sin$ 函数是 1。所以我们不知道这个时间是什么时候——这是这种方法的一个弱点，它不是定量的，而是定性的。所以在某个时刻，我们在最大值下方，然后我们以斜率 1 向上移动。这比我之前画的要陡峭。

再后来，我们仍然向右移动，在某个时刻会到达比如 $3\pi/4$ 的位置，这里是在 $\pi/2$ 处。然后是 $3\pi/4$。我们现在又以 $\sqrt{2}/2$ 的斜率向上移动。然后你注意到，随着我们继续前进，我们现在正在接近这个不动点。事实上，我们将渐近地接近它，并且（你知道）永远不会到达，但在时间趋于无穷时会接近它。所以你现在可以看到答案了，对于这个初始条件，当 $t \to \infty$ 时，$x(t)$ 的极限将是 $\pi$。

但我们也可以看到轨迹的形状，或者说时间序列。这里是 $\pi$。所以我们将渐近地接近它。也就是说，轨迹…时间序列，我不想说轨迹，因为轨迹是在相空间中的 x 轴上发生的。但我们的时间序列 $x(t)$ 定性上会是这样的。也就是说，我们得到一些信息，最初 $x$ 是凹向上增长的，它在加速，越来越快，直到它穿过 $\pi/2$。然后它是凹向下的，它在减速，因为它接近 $\pi$。

好的。这就是使用相空间论证来定性地画出一些东西的例子，你知道，没花多少力气。我不知道我是否用了这些名称，但我想说的是，这类不动点被称为稳定的（Stable）。稳定意味着附近轨迹被吸引到该点。所以如果我们从它旁边扰动一下，会被拉回来。而这种不动点是不稳定的（Unstable）。箭头从它流出。所以一个小扰动会被放大并增长，会变得更大。所以，记号规则将是，我们总是将不稳定的点画成空心圆，稳定的点画成实心圆。

关于那个例子有什么问题吗？

好吧，让我再试一个。我想我只剩几分钟了。我们之前提到了种群生物学中的 Logistic 方程（Logistic Equation）。它由这个微分方程给出：$\dot{x} = rx(1 - x/K)$。其中 $r$ 是一个正参数，$K$ 也是正参数。我们可以试着稍微解释一下这个方程。也就是说，它是从哪里来的？这里有一种思考方式。生物学家会说，一个自然的量是 $\dot{x}/x$。如果 $x$ 是种群的大小——想象很多细菌在有营养物质维持它们生命的培养皿中生长——然后它们每 20 分钟分裂一次，产生新的细菌。所以 $x$ 是种群大小。那么 $\dot{x}$ 就是增长率，对吧？单位时间内产生的生物体数量。当然，生物体越多，增长率就越快，增长率就越大。但你想要做的是用当前种群数量进行归一化。也就是说，$\dot{x}/x$，你可以把它看作是每个细菌的增长率，对吧？这是一个单位个体的增长率（Per Capita Growth Rate），尽管字面意思是“每个头的增长率”，我不知道谈论细菌的头是否有意义，也许有吧。但无论如何，这是单位个体增长率。

所以在 Logistic 模型中，想法是单位个体增长率作为种群数量的函数，是可能的最简单的递减函数。它就是一条直线，从某个值 $r$ 开始下降。当细菌数量很少时，增长率就是 $r$，这会导致指数增长。Logistic 模型的原因是想说，嗯，指数增长在细菌不多的时候可能是对的，但一旦有很多细菌，它们在培养皿里互相挤压，那么它们就会竞争食物，在某个点上，它们过度拥挤，以至于单位个体增长率应该下降。事实上，在这个叫做环境容纳量（Carrying Capacity, K）的地方，增长率将等于死亡率。如果在环境容纳量 K 之后还有更多的细菌，那么实际上你会预期…现在它们死亡的速度会比出生的速度快，它们过度拥挤了。所以这是包含过度拥挤效应的最简单的模型。

如果我们想分析它的行为，我们可以直接画出我们之前的类似图像。你可以很快得出一个很好的小结论。也就是说，如果我们画出 $\dot{x}$ 对 $x$ 的图像，它就是一个抛物线，对吧？因为 $rx(1 - x/K)$ 是一个在 $K$ 和 $0$ 处有根的抛物线图像。注意这里是正的。这里有一个不动点，这里也有一个不动点。然后在这边是负的。

所以预测是，在环境容纳量处有一个稳定的不动点。也就是说，如果你从任何地方开始这个细菌种群，它们会增长直到最终达到水平 $K$。所以当 $t \to \infty$ 时，$x(t) \to K$。也就是说，如果初始条件是正的，只要开始时有任何数量的细菌，它们最终都会达到所谓的环境容纳量，也就是培养皿能支持的数量。如果数量超过了那个值，它们就会死亡减少，直到再次达到环境容纳量。

所以，你看，得出这个结论没花多少功夫。但这就是这种方法的威力所在。

好的，那么我们就在这里结束。下次见。

