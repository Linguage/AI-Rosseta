
# 一种关于无监督学习的理论视角

- 视频链接：[An Observation on Generalization](https://www.youtube.com/watch?v=AKMuA_TVz3A)

## 讲座介绍

本次讲座由 OpenAI 的 Ilya Sutskever 主讲，他分享了对无监督学习的一种理论思考视角。由于无法透露当前的具体研究工作，Sutskever 选择回顾其在 2016 年左右形成的一些关于无监督学习基础原理的见解，这些见解深刻影响了他后续的思考路径。

讲座首先简要回顾了监督学习的理论基础，强调其具有明确的数学保证，使得其成功机制相对清晰。随后，Sutskever 指出了无监督学习研究所面临的核心困境：缺乏类似的理论保障，且优化目标与最终期望获得的下游任务性能之间存在看似神秘的联系。

为寻求更坚实的理论基础，Sutskever 提出了以“压缩”为核心的框架来理解无监督学习。他认为，一个足够强大的压缩器在处理联合数据集时，必然会发现并利用数据间的共享结构以提高压缩效率。这一过程，从信息论的角度看，恰恰解释了无标签数据为何能辅助有标签任务的学习。讲座进一步将此思想推向理论极限，引入柯尔莫哥洛夫复杂度作为理想化的最优压缩器和无监督学习的终极目标，并探讨了其与现实中神经网络训练（如通过 SGD 进行优化）的类比关系。

为了验证该理论框架，Sutskever 展示了早期在图像领域进行的 iGPT 实验，证明了通过优化“下一个像素预测”（一种压缩形式）确实能够学习到高质量、有助于下游任务的图像表示。最后，讲座也坦诚地讨论了该框架的局限性，如未能完全解释线性表示的涌现、忽略计算成本等，并就相关问题与听众进行了深入的问答交流。

## 内容纲要

```
 演讲主题：一种关于无监督学习的理论视角
    ├── 引言
    │   ├── 讲者介绍与演讲背景
    │   ├── 分享早期（2016年）关于无监督学习的思考
    │   └── 设定期望
    ├── 回顾监督学习：一个相对清晰的领域
    │   ├── 学习为何有效？
    │   ├── 监督学习理论（PAC、统计学习理论）
    │   ├── 监督学习成功的数学保证（低训练误差 + 模型复杂度 < 数据量 => 低测试误差）
    │   ├── 关键前提：训练与测试同分布
    │   └── (旁注) VC维度的作用与局限
    ├── 无监督学习：困惑与挑战
    │   ├── 定义与核心困境（优化目标 vs 关心目标）
    │   ├── 缺乏类似监督学习的成功保证
    │   ├── 历史方法与局限性
    │   └── “魔法”般的现象：为何有效？
    ├── 一种有保证的无监督学习思路：分布匹配
    │   ├── 定义：寻找函数 f 使 Dist(f(X)) ≈ Dist(Y)
    │   ├── 例子：机器翻译、语音识别、密码破译
    │   ├── 特点：高维下的强约束，类似监督学习的“保证”
    │   └── 局限：设置可能过于“人造”
    ├── 核心框架：通过压缩理解无监督学习
    │   ├── 压缩 vs 预测：压缩提供更直观视角
    │   ├── 关键思想实验：联合压缩 X 和 Y
    │   ├── 核心洞察：$C(X+Y) \le C(X) + C(Y)$，差值代表共享结构
    │   └── 关联：联合压缩解释了无监督数据(X)如何帮助有监督任务(Y)
    ├── 理论极限：柯尔莫哥洛夫复杂度 (Kolmogorov Complexity)
    │   ├── 定义：$K(X)$ - 生成X的最短程序长度（最优压缩）
    │   ├── 最低“遗憾”：$K(X)$ 相对于任何压缩器 C
    │   ├── 条件复杂度：$K(Y|X)$ - 借助X生成Y的最短程序
    │   ├── 终极目标：$K(Y|X)$ 定义了无监督学习的理想解（零遗憾）
    │   ├── 关联：联合压缩 $K(X+Y)$ 近似条件压缩 $K(Y|X)$
    │   └── 局限：理论概念，不可计算
    ├── 连接现实：神经网络、SGD 与压缩
    │   ├── 类比：神经网络 ≈ 有限程序，SGD ≈ 程序搜索
    │   ├── 大型网络 ≈ 逼近 K-压缩器，减少遗憾
    │   ├── 仿真论解释架构改进难度
    │   └── 联合压缩与最大似然训练的联系
    ├── 实验验证：iGPT (Image GPT)
    │   ├── 目的：在视觉领域验证压缩框架
    │   ├── 方法：图像转像素序列，进行“下一个像素预测”
    │   ├── 结果：压缩性能（预测准确率）与下游任务线性可分性（Linear Probe）正相关
    │   └── 结论：好的压缩器能学习到高质量通用特征
    ├── 讨论与开放问题
    │   ├── 线性表示之谜：压缩理论未直接解释线性可分性
    │   ├── 自回归 vs BERT 表示能力的比较与推测
    │   ├── 训练动态与数据顺序（课程学习效应）
    │   ├── 其他概率模型（扩散模型）与框架的兼容性
    │   ├── 理论框架忽略计算成本的局限
    │   └── 模型大小、压缩效果与理论的权衡
    ├── 总结
    │   └── 压缩视角为无监督学习提供理论基础
    └── 问答环节
        ├── 关于自回归优于BERT表示的推测
        ├── 关于二维像素预测的鲁棒性（与扩散模型比较）
        ├── 关于训练动态与K复杂度的差异（搜索过程）
        ├── 关于区分分布、预测与压缩的联系（密码学视角）
        ├── 对VC维度的辩护（量子态学习例子）
        ├── 关于Transformer/SGD处理整个数据集与K复杂度的关系
        ├── 关于压缩框架、线性表示与下游任务非直接关联的情况
        ├── 压缩理论对监督学习的启示（函数类、参数与样本关系）
        ├── 自回归建模的具体重要性（与其他最大似然模型比较）
        ├── 模型大小增加与压缩器自身复杂度的关系
        ├── 使用验证集是否弥合理论与实践差距
        ├── 关于使用gzip+KNN进行分类的论文
        └── 关于课程学习效应的当前经验情况
```



# 演讲主题：一种关于无监督学习的理论视角

## 引言

**YEJIN CHOI:** 他的论文引用次数达到了六位数，超过了13.9万次，甚至更多。所以非常期待听到 Ilya 关于大语言模型（LLMs）和未来的分享。交给你了。

**ILYA SUTSKEVER:** 好的，大家好。[掌声] 大家好，谢谢介绍。当 Umesh 邀请我参加这个活动时，我感到非常兴奋。我看了所有的演讲者名单，心想，太好了，我会去讲点什么。

然后我遇到了一个问题，那就是我们在 OpenAI 做的很多技术工作，我其实不能公开谈论。[笑声] 所以我真是绞尽脑汁思考我能讲些什么。

就在不久前，我把我所有的研究重心都转移到了人工智能对齐（AI alignment）上。我们在这方面会有非常酷的成果可以展示，但不是现在。所以我想，这得留到下次演讲了。那么这次演讲讲什么好呢？我想到了一个主意。

我会告诉你们一些我们很久以前在 OpenAI 取得的非常古老的结果，甚至可以追溯到 2016 年，这些结果确实影响了我对无监督学习的思考方式。我想和大家分享一下。也许到了现在，你们会觉得这些显而易见，但也可能不全是。所以至少还有一点小小的可能，你们会觉得有趣。所以我想先把期望值设得低一点，然后希望能超出预期。

所以，一个关于无监督学习的理论。这样的东西怎么可能存在呢？

## 回顾监督学习：一个相对清晰的领域

在我们讨论无监督学习之前，我们想谈谈学习本身。什么是学习？学习为什么能起作用？为什么计算机应该能够学习？

现在我们已经习惯了这个事实，我们想当然地认为神经网络能够学习。但它们为什么能学习呢？从数学上讲，为什么它们应该能学习？为什么数据会具有我们的机器学习模型能够捕捉到的规律性？这不是一个显而易见的问题。

多年前，由多人共同完成的机器学习领域一个重要的概念性进展是监督学习的发现和形式化。它通常被称为 PAC 学习（Probably Approximately Correct learning）或统计学习理论（Statistical Learning Theory）。监督学习的好处在于，它给出了一个精确的数学条件，在此条件下学习必然成功。

理论告诉你，如果你有一些来自某个数据分布的数据，如果你设法达到了较低的训练损失，并且你的模型的自由度数量（例如参数量）小于你的训练集大小，那么你将获得较低的测试误差。并且这是有保证的。所以你有一个数学条件，你可以说，如果我确实从我的函数类中找到了一个函数，它实现了低训练误差，那么学习就会成功。

你可以说，是的，这是一个我们可以进行推理的非常合理的数学事物。这就是为什么监督学习相对容易理解。然后你有了所有这些我认为很简洁的定理，我发现它们很优雅。你可能见过这样的定理。基本上，这类定理就是，如果你知道它，你会说，“哦，是的，那个东西。”如果你不知道，那就不可能在 30 秒内解释清楚。不过，5 分钟内解释清楚是可能的，只是 30 秒不行。这些东西都不复杂。

你有一个小小的证明，它说，如果你函数类中有一定数量的函数，那么至少有一个函数的训练误差远离其测试误差的概率……这里有一些数学推导，而且数学很简单。这就是全部的数学——三行数学。所以三行数学就能证明整个监督学习。嗯，这很好。这非常好。

所以监督学习是（相对而言）被很好理解的东西。我们知道它为什么必须成功。因此，我们可以去收集大型监督学习数据集，并完全确信模型会持续变得更好。这就是监督学习的故事。

是的，我忘了提及这些结果中一个非常重要的部分。测试分布和训练分布必须相同。如果它们相同，那么你的监督学习理论就能生效并取得成功。所以从概念上讲，它是清晰明了的。

我们对于监督学习为什么有效，为什么语音识别应该有效，为什么图像分类应该有效，都有了答案，因为它们都归结为监督学习，而监督学习是有效的，有这种数学保证。所以这非常好。

这里我想对 VC 维度（VC dimension）做一个小小的旁注，给那些关心这类事情的人。可能只有一小部分人。所以如果你想在接下来的 30 秒钟走神，请随意。很多关于统计学习理论的文章都强调 VC 维度是一个关键组成部分。但 VC 维度被发明的主要原因——实际上是唯一原因——是为了让我们能够处理具有无限精度的参数。VC 维度是为了处理具有无限精度的参数而被发明的。所以如果你有一个线性分类器，每个参数都是无限精度的。

但是，当然，在现实中，我们所有的浮点数都是有限精度的，而且它们的精度还在缩水。所以你可以——所以你拥有的——所以由计算机实现的函数数量实际上是有限的。你可以把它归结回那个小公式，它几乎给出了你能从监督学习中得到的最好的界限。所以我发现这很酷。我发现这很有吸引力，因为你的证明行数更少。

## 无监督学习：困惑与挑战

现在，让我们来谈谈无监督学习。

首先，什么是无监督学习？它是什么？监督学习就像是，你有一些数据告诉你，这里这样做，那里那样做，你有所有这些数据。你在训练误差上做得很好，你的训练误差很低。你的训练数据比你函数类中的自由度（参数）要多。也可能有其他类型的自由度——比如比特。然后你说，你的监督学习会成功。

但是无监督学习是什么？关于无监督学习你能说些什么呢？我要说，至少我没有看到过一个关于无监督学习的阐述，是我觉得满意的。如何从数学上对其进行推理？我们可以凭直觉推理，但能从数学上推理吗？

作为背景，无监督学习的古老梦想是什么？顺便说一句，这个梦想已经被实现了，但它是在经验层面上实现的。我们能否稍微超越经验结果一点点？比如，仅仅通过观察图像，或者仅仅通过观察文本，而没有被告知要用它们做什么，就能以某种方式发现数据中存在的真正隐藏结构，并以某种方式帮助你？

但这为什么会发生？它应该发生吗？我们应该期望它发生吗？你没有任何与监督学习保证类似的东西。监督学习的保证是说，是的，获得低训练误差，你就能实现学习。这将是一个巨大的成功。

所以无监督学习，看起来——看起来不是这样的。人们讨论它已经很久了，在 80 年代。玻尔兹曼机（Boltzmann machine）就已经在讨论无监督学习了。而且无监督学习在小规模上也并不奏效，但所有的想法都在那里，比如去噪自编码器（denoising autoencoder），对于那些还记得它的人来说。它就像是 BERT 或者扩散模型（diffusion model），只是内部有一个微小的扭曲，最微小的扭曲。旧时代的语言模型，它们也能生成在当时看来很酷的样本，但它们的无监督学习表现远不如今天的模型。

但我想说明的是，这令人困惑，因为它就像——为什么令人困惑？你优化。无监督学习是如何工作的？你说，让我们优化某种重构误差，或者让我们优化某种去噪误差，或者某种自监督学习误差。你优化一个目标。哦，是的，我刚说了。但你关心的是一个不同的目标。那么这难道不意味着你没有理由期望你会得到任何好的无监督学习结果吗？或者说，你在经验上确实得到了它们，但是，这其中的神秘程度相当高，我认为。这似乎是一个完全无法触及的现象。你优化一个目标，但你关心另一个目标。然而它却有帮助。这怎么可能呢？魔法。

另一件事，顺便说一句，是无监督——嗯，我猜我要说的话只有 90% 是对的。无监督学习不——你可以说，好吧，你只是学习了输入分布的结构，它帮助了你。但是，如果你从均匀分布中训练呢？那么你所有的无监督学习算法都会失败。你应该如何思考这个问题？那么我们能说些什么呢？我们需要做假设吗？什么样的假设？

## 一种有保证的无监督学习思路：分布匹配

所以我想提出一种思考无监督学习的方式，我认为，我个人觉得它很有趣。也许你也会觉得有趣。让我们拭目以待。

我想向你们展示一种进行无监督学习的方式，它不一定广为人知，因为它从未成为主流的无监督学习方式。但它有一个很酷的特性，那就是与监督学习类似，它 *必须* 起作用。

那么，什么样的神秘无监督学习过程，在你没有给任何输入打标签的情况下，仍然保证有效呢？

分布匹配（Distribution matching），分布匹配。

那么什么是分布匹配？假设我有我的数据。我有 $X$ 和 $Y$ 这两个数据源。它们之间没有对应关系。我只有两个数据源，数据源 $X$ 和数据源 $Y$，比如语言一、语言二，文本、语音——它们之间没有对应关系。

让我们看看这个标准：找到一个函数 $f$，使得 $f(X)$ 的分布与 $Y$ 的分布相似。即 $Dist(f(X)) \approx Dist(Y)$。这是对 $f$ 的一个约束。

在机器翻译和语音识别的例子中，这个约束可能是有意义的。你可以说，是的，如果我应用函数 $f$ 到英语句子的分布上，得到的东西非常类似于法语句子的分布，你可以说，好的，我找到了关于 $f$ 的真实约束。

如果 $X$ 的维度和 $Y$ 的维度足够高，这将给你很多约束。事实上，你可能几乎可以从这些信息中完全恢复 $f$。

这是一个无监督学习的例子，它仍然保证有效，与监督学习保证有效的意义相同。另外，替换密码（substitution ciphers），比如那些简单的小加密方法，也符合这个框架。

就是这样。我在 2015 年独立发现了这一点。我对此非常着迷，因为我想，哇，也许关于无监督学习，我们可以说一些有意义的、数学上有意义的东西。

但是，我们来看看。这种设置的问题在于，它仍然有点人为。它仍然——现实中的机器学习设置不是这样的。而且我们喜欢思考无监督学习的方式也不是这样的。

## 核心框架：通过压缩理解无监督学习

现在我将向你们介绍我想要说的核心内容——一种思考无监督学习的提议方式，它让你——它将其置于与监督学习同等的地位。那么好吧，它在数学上做了什么？你怎么能确定你的无监督学习是好的呢？

压缩来救场（Compression to the rescue）。

显然，众所周知——我不应该说显然。这并非显而易见，但是众所周知，压缩即预测（compression is prediction）。每个压缩器都可以是一个预测器，反之亦然。所有压缩器和所有预测器之间存在一一对应的关系。

然而，我认为，为了思考无监督学习，压缩的语言提供了一些优势，至少对我来说是这样。也许对你也是如此。

那么，考虑以下思想实验。这个思想实验是最重要的一页幻灯片。假设你有两个数据集，$X$ 和 $Y$。你有两个数据集，在你巨大的硬盘上有两个文件。假设你有一个非常棒的压缩算法 $C$，它接收数据输入，并输出压缩后的对象。

假设你 *联合* 压缩 $X$ 和 $Y$。你将它们连接起来。你把这两个数据集连接起来，然后把它们喂给你的压缩器。会发生什么？

嗯，让我们看看。特别地，一个重要的问题是，一个足够好的压缩器会做什么？我的答案是，非常直观地，它会利用存在于 $X$ 内部的模式来帮助它压缩 $Y$，反之亦然。你可以对预测提出同样的主张，但不知何故，当你用压缩来说这件事时，它更直观。我不知道为什么会这样，但我发现确实如此。

所以这是我们的线索。你可以写出这样一个等式，你说，嘿，如果你的压缩足够好，如果它是一个真正伟大的压缩器，它应该满足：你连接后的巨大文件的压缩结果 $C(X+Y)$，应该不比你分别压缩两个文件的结果之和 $C(X) + C(Y)$ 更差。即 $C(X+Y) \le C(X) + C(Y)$。

那么，通过连接获得的任何额外的压缩量 $C(X) + C(Y) - C(X+Y)$，就是你的压缩器注意到的某种共享结构。你的压缩器越好，它提取的共享结构就越多。这个差值就是共享结构，或者叫算法互信息（algorithmic mutual information）。

这很有趣，对吧？你可以看到我在暗示什么。$Y$ 是你的监督任务的数据。$X$ 是你的无监督任务（数据）。但突然之间，你有某种数学上的理由，让 $X$ 中的信息、模式去尝试帮助 $Y$。

还要注意它是如何推广分布匹配的。如果我们处于分布匹配的情况，你有 $X$ 是语言一，$Y$ 是语言二，并且你知道存在某个简单的函数 $F$ 将一个分布转换为另一个分布。那么肯定地，你的压缩器，如果它足够好，会注意到这一点，并利用它，甚至可能在内部尝试恢复这个函数。

我认为这非常酷。我们形成了一个闭环。

## 理论极限：柯尔莫哥洛夫复杂度 (Kolmogorov Complexity)

那么我们该如何将其形式化呢？无监督学习的形式化将是什么？让我们看看。让我们看看我能否做到。

考虑一个机器学习算法。顺便说一下，在下文中，我会有点不严谨，我会互换使用压缩和预测。假设你有一个机器学习算法 $A$。它是一个算法 $A$，它试图压缩 $Y$。并且假设它可以访问 $X$。$X$ 是文件一，$Y$ 是文件二。你希望你的机器学习算法，你的压缩器，能够压缩 $Y$，并且它可以根据需要探测 $X$。目标是尽可能好地压缩 $Y$。

我们可以问自己，使用这个特定算法的“遗憾”（regret）是多少？你会明白我的意思。相对于什么而言的遗憾？如果我做得足够好，如果我的遗憾很低，意味着我已经从这些无标签数据中获得了所有我可能获得的帮助。这些无标签数据已经尽可能多地帮助了我。我对此感觉良好。我没有感觉我遗漏了一些预测价值在桌面上，而其他人用更好的压缩算法本可以利用这些价值。这就是它的含义。

特别是，这就像，是的，你可以晚上安心睡觉了，知道如果在无标签数据中有一些可以帮助我的任务的信息，没有其他人——没有人能比我做得更好。我在从我的无标签数据中受益方面做得最好了。

所以我认为这是朝着思考无监督学习迈出的一步。你不知道你的无监督数据集是否真的有用。它可能超级有用，它可能包含答案。它也可能完全没用，它可能是均匀分布。但是如果你有一个低遗憾的无监督学习算法，你可以说，无论是第一种情况还是第二种情况，我知道我已经尽力了。我知道我已经尽力从我的无标签数据中获益了，没有人能比我做得更好。

现在，我想绕道去理论领域，这有点晦涩。但我认为它很有趣。柯尔莫哥洛夫复杂度（Kolmogorov complexity）作为终极压缩器，给了我们终极的低遗憾算法——虽然它实际上不是一个算法，因为它不可计算。但你很快就会明白我的意思。

首先，作为背景，这里有多少人熟悉柯尔莫哥洛夫复杂度？好的，大约 50%。柯尔莫哥洛夫复杂度是那种很容易在 1 分钟内解释清楚的东西，所以我就这么做。它就像，想象一下，如果你给我一些数据，或者你给我一些数据。我要通过给你一个可能存在的最短程序来压缩它，这个最短程序存在，如果你运行它，它就会输出你的数据。

**观众：** 这里有个笔误。[听不清] 应该是 X 而不是 Y。
**ILYA SUTSKEVER:** 是的，你说得对。被你抓到了。[笑声] 它是输出 $X$ 的最短程序的长度。是的。

直观上，你可以看到这个压缩器相当好，因为你可以证明这个定理，这个定理也很容易证明，或者说，很容易感受到它。一旦你感受到了，你就可以有点相信我它很容易证明。你基本上可以说，你的柯尔莫哥洛夫压缩器，如果你用它来压缩你的字符串，你对你的压缩质量会有非常低的遗憾。

你可以证明这个结果。它说，如果你有一个字符串 $X$，你的数据集，数据库，随便什么，输出 $X$ 的最短程序的长度 $K(X)$，比你的压缩器 $C$ 需要输出的长度 $C(X)$ 要短，最多加上一个小项，这个小项是你实现你的压缩器 $C$ 所需的代码字符数（即 $K(C)$）。数学上讲， $K(X) \le C(X) + K(C) + O(1)$。

直观上，你可以看到这是有道理的，通过模拟论证（simulation argument）。模拟论证是，如果你告诉我，嘿，我有一个非常棒的压缩器 $C$，我会说，酷，它有附带计算机程序吗？你能把这个计算机程序给 $K$ 吗？因为 $K$ 会运行计算机程序，你只需要支付程序的长度。

所以，在不给你细节的情况下，我想我给了你它的感觉。柯尔莫哥洛夫复杂度，柯尔莫哥洛夫压缩器可以模拟其他压缩器如何工作，只要给它那个压缩器的程序。这也是为什么它不可计算。它不可计算，因为它模拟——它感觉非常自由地可以模拟所有计算机程序。

但它是存在的最优压缩器。而我们之前在讨论用于无监督学习的好的压缩。

现在，让我们推广柯尔莫哥洛夫复杂度，一个允许使用辅助信息（side information）的柯尔莫哥洛夫压缩器。我会更详细地谈谈。我会多次重申这一点，因为这一点很重要。

我将定义 $K(Y|X)$。它就像是输出 $Y$ 的最短程序，如果它被允许探测 $X$。这就是那个输出 $Y$ （如果允许探测 $X$）的最短程序的长度。你可以证明类似的结果（关于遗憾）。你可以立刻看到，是的，这根据定义就是无监督学习的解决方案。如果你使用它，你可以晚上睡得非常非常安稳，知道没有人比你做得更好的无监督学习。它就是字面意思。

所以这是无监督学习的终极低遗憾解决方案，只不过它不可计算。但我确实认为这是一个有用的框架。

这里我们是*以一个数据集为条件*，而不是一个样本。这个东西会从 $X$ 中提取出所有用于预测 $Y$ 的价值，是预测整个数据集 $Y$，而不是单个样本 $Y$。所以这是无监督学习的解决方案——完成，成功。

还有一个小小的技术细节，我需要花点时间谈谈，那就是我们之前讨论的条件柯尔莫哥洛夫复杂度 $K(Y|X)$，我们讨论的是那些试图压缩一个东西（$Y$），同时可以访问另一个东西（$X$）的压缩器。这在机器学习的背景下有点不自然，当你关心处理大数据集时，至少在今天看来是这样。虽然情况变化相当快。但我认为仍然可以说，没有真正好的方法可以*以一个大数据集为条件*进行操作。你可以拟合一个大数据集，但你不能以它为条件，还不行，不是真正意义上的。

所以这个结果表明，嘿，如果你关心使用经典的柯尔莫哥洛夫压缩器来对你的监督任务 $Y$ 进行预测，这个压缩器只是压缩 $X$ 和 $Y$ 的连接 $X+Y$，那么它的效果将和使用你的条件压缩器 $K(Y|X)$ 一样好。对于我刚才说的内容，还有更多的细节和一些微妙之处。如果有人感兴趣，我很乐意在线下讨论它们，但这基本上是说，如果之前你说，嘿——上一张幻灯片说你可以使用这个条件柯尔莫哥洛夫压缩器来解决无监督学习。这张幻灯片说你也可以使用你的常规柯尔莫哥洛夫压缩器。只需要把你的所有数据都扔进去。把你所有的文件拿来，连接它们，压缩它们。这将在你的监督任务，你关心的任务上，做出一些很好的预测。

关于为什么这是真的，有一些直觉。这个结果实际上——证明它稍微有点棘手，所以我不会做。

所以无监督学习的解决方案，就是把所有东西都交给你的柯尔莫哥洛夫复杂度——你的柯尔莫哥洛夫压缩器。

最后一点是，我要提到这种联合压缩，如果我们不过拟合的话，就是最大似然（maximum likelihood）。如果你有一个数据集，那么给定你的参数，所有数据点的似然之和（的负对数）就是压缩该数据集的成本。你还需要支付压缩参数本身的成本，但你可以看到，如果你现在想压缩两个数据集，没问题。只需将更多点添加到你的训练集，你的数据集中，并将对应的项添加到总和中。

所以这种连接，这种联合压缩，在机器学习的背景下非常自然，这就是为什么值得费力去说，是的，我们有我们的条件柯尔莫哥洛夫复杂度。然后我做了一些论证。我提出了一个主张，但没有完全捍卫它，但有可能捍卫它，即使用常规的——只是压缩所有东西——的柯尔莫哥洛夫复杂度也同样有效。

所以我认为这很优雅。我喜欢它，因为它表明，好吧，如果你眯着眼睛看，你可以说这解释了我们的神经网络在做什么。

## 连接现实：神经网络、SGD 与压缩

显然，柯尔莫哥洛夫压缩器是不可计算的。它是不可判定的。但是，嘿，因为它像是在搜索所有程序，你知道吗，如果你在一个有 100 层的神经网络的参数上运行 SGD，它自动地就像是在一个具有一定内存量、一定步数的计算机上进行程序搜索。这有点像微型微型微型同态（homography? - unclear word, likely meant analogy），比如拟合一个神经网络。你有点能感觉到那种相似性。

这有点神奇，对吧？神经网络可以模拟真实的程序。它们是小型的计算机。它们是电路。电路是计算机，是计算机器。而 SGD 在程序上进行搜索。整个深度学习都建立在 SGD 这个奇迹之上，即我们实际上可以用 SGD 训练这些计算机。这行得通。我们确实从数据中找到了那些电路。

因此，我们可以计算我们的微型柯尔莫哥洛夫压缩器。顺便说一句，模拟论证在这里也适用。我只想提一下这个事实。我不知道你是否——如果你曾经尝试设计一个更好的神经网络架构，你会发现这有点难。你说，好吧，让我们添加这个连接。让我们添加那个连接。让我们修改这个和那个。为什么很难？模拟论证，因为你的新架构可以相当直接地被你的旧架构模拟。

除非它不能。那些是罕见的情况。在那些罕见的情况下，你会有巨大的改进，比如当你从小型的 RNN 切换到 Transformer 时。RNN 有一个瓶颈，即隐藏状态。所以它很难实现 Transformer。然而，如果我们找到一种方法来工程化[听不清]一个非常非常大的隐藏状态，也许它会再次变得和 Transformer 一样好。所以这就是联系。

你开始看到我们是如何从形式化的领域转换到神经网络领域的。但你看到了相似性。

你可以说，嘿，大型神经网络上的 SGD 是我们的大规模程序搜索。更大的神经网络越来越好地逼近柯尔莫哥洛夫压缩器。所以也许这也是为什么我们喜欢大型神经网络，因为我们正在接近那个不可接近的柯尔莫哥洛夫压缩器的理想，它真正没有遗憾，而我们只是想随着我们训练越来越大的神经网络，在提取预测价值方面拥有越来越少的遗憾。

## 实验验证：iGPT (Image GPT)

现在，这种理论如何应用于 GPT 模型——你知道，我认为这个理论也适用于 GPT 模型。但关于 GPT 模型有点棘手的是，它们的行为理论也可以在不引用压缩或无监督学习的情况下得到解释。你只需说，不，这只是互联网上文本的条件分布。少样本学习（Few-shot learning），只需想象一个包含一些重复模式的文档，模式很可能会继续下去。所以 GPT 模型可以凭直觉得到解释，至少它们的少样本行为绝对可以在不提及这个理论的情况下得到解释。

所以我想，这样会很好——我们能否找到这个理论的其他直接验证？现在，我们能否找到一个不同的领域，比如视觉？因为视觉，你有像素。你能证明在像素上这样做会导致好的无监督学习吗？

答案是，是的，你可以。这是我们在 2020 年做的工作。我们只是称之为 iGPT。这是一个昂贵的概念验证。它的目的不是——它并非旨在成为一个实用的程序。它旨在成为一篇论文，表明如果你有一个真正好的下一步预测器（next step predictor），你将做出很棒的无监督学习。并且它在图像领域得到了证明。

在那里，我直接说明。你有你的图像。你把它变成一个像素序列。每个像素应该被赋予一些离散的强度值。然后就做下一个像素预测（next pixel prediction）。使用相同的 Transformer。就是这样——与 BERT 不同。只是下一个标记预测（next token prediction），因为这最大化了似然，因此进行了压缩。

就像我们看到的，我们看到的一个直接结果——这些是 CIFAR-10 上的结果。你有不同大小的模型。这是它们在像素预测任务上，即它们的无监督学习任务上的下一步预测准确率。这是线性探针（linear probe）准确率，线性探针，当你选择神经网络内部的某个层，最好的层，拟合一个线性分类器，看看它做得如何。你得到了这些看起来不错的曲线，它们开始变得越来越相似。这有点像你想要的。它表明它在起作用。

与下一个词预测相同类型的像素预测，下一个——不仅仅是像素——不仅仅是单纯的像素预测，而是下一个像素预测，导致了越来越好的无监督学习。我认为那非常酷。

我们将其扩展到不同程度，我们表明，它确实学得相当好。我们接近了，但我们没有完全弥合我们的无监督学习与当时 ImageNet 上最好的无监督学习之间的差距。但这显然是一个——它确实感觉像是在扩展，而且是计算资源的问题，因为那些（SOTA）方法使用大型、高分辨率的图像，而我们使用的是像 64x64 这样的小图像，配上当时看来巨大的 Transformer——以今天的标准看很小，但在当时是巨大的，60 亿参数。

所以这就像，是的，你在一个大型图像数据集上进行你的无监督下一个像素预测，然后在 ImageNet 上拟合你的线性探针。你得到了强劲的结果。就像，好的，这很酷。

CIFAR，是的——我们得到的一个很酷的事情是，如果你用这种方法在 CIFAR-10 上达到了 99% 的准确率，那很酷。2020 年是不同的时代，但这很酷。

## 讨论与开放问题

我将以几个关于线性表示（linear representations）的评论来结束。我喜欢压缩理论，因为我觉得它困扰了我很长时间，你无法严格地思考无监督学习。我认为现在你可以了，至少在某种程度上。仍然需要很多挥手示意（hand-waving，指不严谨的论证），但也许比以前少了一点。

但它并没有说明为什么你的表示应该是线性可分的。它没有说明线性[听不清，可能是probe]应该发生。但是线性表示一直都在发生。其背后的原因必定是深刻和根本的。我认为我们也许能在某个时候清晰地阐明它。

我发现一件有趣的事情是，这些下一个像素预测模型，自回归模型（autoregressive models），似乎比 BERT 具有更好的线性表示。蓝色的准确率是 BERT 对比自回归模型。我不确定为什么会这样，或者说我可以推测。我有一些推测。但我认为如果能更多地理解为什么，比如真正地理解为什么那些线性表示会形成，那会很好。

## 总结

是的，这就是结束。感谢大家的关注。[掌声]

## 问答环节

**问：** 你能提供一下那个推测吗？

**答：** 是的。哦，是的，是的。我认为推测基本上是这样的：如果你在做下一个像素预测，你是从所有之前的像素来预测下一个像素。所以你需要观察长距离结构。但是在 BERT 中，你有你的向量。假设你丢掉了 25% 的标记（token），在这个例子里是像素，那么你做的任何预测，实际上通过稍微往前看一点和稍微往后看一点就能做得很好。所以你移除了所有困难的预测任务，或者让它们变得容易得多。下一个像素预测中最难的预测任务，比 BERT 预测情况中最难的预测任务要难得多。所以这是一个论点。如果我们尝试设计一个实验来测试它，我们甚至可能能够测试它。但是，是的，这就是推测。

**问：** 是否有更鲁棒的二维版本的下一个像素预测？

**答：** 我会说更鲁棒的——我会说任何形式上——你做的任何将神经网络转化为一个为不同输入分配概率的概率模型的事情都是。所以另一种做下一个标记预测的重要方式是扩散模型（diffusion models）。扩散模型也像——不是那些——人们在高质量图像生成器中使用的扩散模型并不真正最大化其输入的似然。它们有不同的目标。但是最原始的公式是最大化似然。顺便说一句，扩散模型是对——或者说，扩散模型，我也会声称，应该比下一个标记预测模型具有更差的表示，原因和 BERT 一样。所以我觉得这在我看来进一步增加了导致线性表示形成的因素的神秘性。

**问：** 是的。谢谢你的演讲。我喜欢柯尔莫哥洛夫复杂度和神经网络之间的类比。我猜有一个地方看起来存在差异，那就是神经网络有训练动态。而如果你做像仅仅考虑所有计算机程序这样的事情，它更像是内存。所以如果你用柯尔莫哥洛夫复杂度进行压缩，数据的顺序不重要。但它对神经网络显然是重要的。你有简单的启发式方法和在训练早期学到的特征，这些特征可能会在训练后期持续存在。所以，我猜，你对于如何在这个图景的背景下思考这个问题有什么想法？

**答：** 是的。我的意思是，这个类比并不完美。这是真的。你描述它——这个类比最不适用的地方是在搜索过程（search procedure）中。这确实是你所暗示的，比如，数据顺序很重要。为什么？因为我们使用的是一个弱搜索过程。柯尔莫哥洛夫压缩器使用无限昂贵的搜索过程，即每次都从头枚举所有东西。所以，是的，我的意思是——我的意思是——我想说对于这个特定的类比应该谨慎使用。它很明显不是普遍适用的。但我确实认为在这种情况下——我确实认为在解释无监督学习从何而来方面，这里有一些价值。

**问：** 所以你现在——在你形式化地在压缩和下一个比特预测之间来回切换时，你正在将无监督学习与监督学习联系起来。那么如果你从密码学回溯，有一种理论。可以追溯到 80 年代，他们谈论压缩等同于下一个比特预测，等同于能够区分两个分布。所以如果你有[听不清]，那么你就有一个可以预测的算法——那么你就有一个可以压缩的算法。我的意思是，密码学是反过来的。你说没有办法压缩[听不清]。因此没有办法[听不清]。所以我想知道这种能够区分的想法，如何能自然地转化为任何东西？

**答：** 我想我理解这个问题。让我复述一下。我对你提到的领域不是很精通。但你是说，如果你能区分两个分布，你可以利用这种可区分性来做一些——来预测。我猜问题是，什么是——我有一些——

**观众：** 你有来自一个分布的样本，有来自另一个分布的样本。你可以区分它们[听不清]。

**答：** 所以我猜我的问题是，你能预测得多好——或者你是在谈论你能预测一点点？你指的是这个吗？

**观众：** 是的，[听不清]。你可以预测下一个比特会是什么，比如说，在一个样本中。

**答：** 所以——

**观众：** 实际上，[听不清]，[听不清]你可以预测那些。

**答：** 我的意思是，我可以提到一件相关的事情，那就是基于能量的模型（energy-based models）。所以基于能量的模型提供了另一种将神经网络转化为概率分布的方式，其中一个基于能量的模型会说，只需给我你的向量配置，我就会告诉你它的感觉如何。然后你对所有配置进行归一化。我觉得当涉及到基于能量的模型时，特别是分布的比率对应于能量的差异。也许这与你说的有些关系。我想我可能没有精确地评论你所说的事情，但不幸的是，我似乎没有更多可以补充的了。

**问：** Ilya，也许我只想为 VC 维度的荣誉辩护一小句。

**答：** 请讲。

**观众：** 嗯，所以在 2007 年，我有一个关于量子态的 PAC 学习的定理。这恰好是一个例子，即使你不关心无限精度，即使你离散化状态空间，比如你看 VC 维度，或者胖分裂维度（fat shattering dimension）之类的，它也比假设类别大小的对数要指数级地小。所以我确实认为有些情况下你仍然需要 VC 维度。

**答：** 这是一个很酷的例子。[笑声]

**问：** 我没有完全跟上你的符号。大写 X 是来自一个分布的样本吗？

**答：** 是的。

**观众：** 分布是——

**答：** 是数据集（the data set）。

**观众：** 那么 transformer，SGD——我不确定你是否能把它看作是压缩[听不清]的最佳程序。也许因为它一次只得到一个样本。

**答：** 这是真的。我们还做了另一个假设。如果你看总的训练损失——假设你有一些神经网络。它不一定是 transformer——某个为你的数据分配对数概率的神经网络。你有很多训练案例。你可以运行这个神经网络。你需要某个神经网络。你可以计算它在每个案例上的对数概率。你可以把它们加起来。这将是该神经网络赋予整个数据集的对数概率。现在，这个神经网络无法——这种特定的表述使得神经网络无法明确地注意到数据顺序中可能存在的时间或其他任何类型的结构。但我仍然认为说，是的，你可以计算整个数据集的对数概率是有意义的。这给了你你的负对数概率，字面上就是使用这个神经网络作为压缩器来压缩这个数据集所需的比特数。

**问：** 如果我能复述一下，我认为你在主张将压缩作为一个框架来理解或推动无监督学习。你在最后提出的一个观点是，如果你将该框架应用于语言模型，应用于下一个词预测，它可能感觉有点肤浅，因为下一个词预测，任何文本任务都可以转化为下一个词预测。因此，无监督学习在某种程度上与文本的监督学习表面上是相同的。所以我们转向 image GPT，在那里你不能将任何给定的任务表述为下一个像素预测。也许你可以，但我们就说你不能。但是然后你可以使用线性表示作为一种方式来表明压缩是制定无监督学习的一个好方法。但是，存在一些高效的压缩器，它们不会给你一个有用的线性表示。所以我想知道，是否存在无监督学习和监督学习不是表面上相同的情况，[听不清]，但是你不需要你的压缩器给你一个有效的线性表示来表明压缩是一个好的无监督目标？

**答：** 是的。这是一个非常——我对这个问题有想法。首先，我会说线性表示，一个好的线性表示是一个额外的好处（bonus）。这个论点在任何时候都没有说，因此线性表示应该出现。然而，我认为理论确实表明好的微调（fine tuning）应该出现，因为联合压缩有点像是使用糟糕的搜索算法（即 SGD）进行的粗糙的近似微调。现在，我们知道来自那些旧实验的证据表明，当在图像上运行时，BERT 比下一个像素预测学习到更差的线性表示。也许对于扩散模型也是如此。这看起来可能性很高。我认为看看微调后的扩散模型表现如何会非常有趣。也许这里已经有人知道了。

**问：** 我想知道你是否能把你关于无监督学习的想法带回来。在我看来，似乎可以从中获得一些对监督学习[听不清]的见解。

**答：** 嗯，我认为这里这让你对——所以你可能得到的特定见解是关于函数类，期望的函数类的见解。你希望你的神经网络有很多层。例如，如果你有很多层，它可以进行更多的思考。你希望那些层更宽，更大的神经网络。我的意思是，本质上，这就是这个领域已经发现的东西。

**观众：** 但是你可能不需要比[听不清]数量更多的样本。在监督学习中，这也许可以解释为什么你不一定需要更多的参数。

**答：** 没错。所以这可能，例如，是——所以这个理论的一个弱点——顺便说一句，这个理论有一个巨大的实践弱点，那就是它忽略了计算成本。它只关注信息。所以你们都熟悉通用 transformer（universal transformer），也许——基本上，它就像是一个 transformer。我们在每一层使用相同的权重。这是一个好主意，只不过如果你想拥有很多参数，你需要为此付出大量的计算成本。没人想那么做。你不能忽略计算成本。这个理论忽略了计算成本。如果你忽略计算成本，它会给你一个如何进行的指导方针。

**问：** 你认为自回归建模（autoregressive modeling）在概率分布中的重要性具体是什么？你可以将 BERT 视为在进行最大似然训练。我认为你可以找到从 BERT 中采样的方法，例如。

**答：** 所以某些扩散模型可以被设置为最大似然模型。因此所有这个理论预测的是，扩散模型也应该——应该有可能让扩散模型做出同样伟大的事情，也许有一些常数因子的差异——因为这个——正如之前的回答，这不是一个对计算敏感的理论。所以它会说，好吧，也许你需要像 10 或 15 倍的计算量，然后自回归模型和扩散模型之间的事情就会变得相同。自回归模型，它只是简单。它很方便。也许基于能量的模型会做出更伟大的事情。但从那个角度来看，它们都是一样的。

**问：** 看起来 GPT-4 目前可能是最好的压缩器，推测它也是目前最大的模型。所以一方面，它能够更好地压缩。另一方面，压缩器本身的大小也在增加。或者说，从[听不清]复杂性理论的角度来看，情况并非必然如此？

**答：** 嗯，我的意思是重要的是——你真正想要的是——这个理论与现实不太对应的另一种方式是，这个理论说，你有一个固定的数据集想要压缩。但是在我们训练 GPT 模型的方式中，你说，你有一个大的训练集，然后你有一个测试集，假设是无限的。如果测试集是无限的，并且你关心压缩测试集，那么你就不关心你的压缩器的大小，只要测试集的大小远大于它。所以我认为这也是，可以说，一个差异之处，需要更仔细的思考来获得清晰度。

**问：** 使用一个独立的验证集，只要它是分开的，是否就足够了？这是否弥合了差距？

**答：** 是否足够？这是一件好事。做这件事是好的。它是否真正——问题在于我认为它也是——实际上，比如在单轮训练（single epoch）的情况下，如果你处于单轮训练的情况，那么你可以在训练时计算你的对数概率，这将类似于模型对数据集的压缩。这也给了你对验证集的一个很好的估计。所以在单轮训练的情况下，我认为情况非常相似。

**问：** 我只是想让你知道上个月在[听不清]上有一篇论文。它使用了 gzip，然后是 k-最近邻（k-nearest neighbor）分类器进行文本分类。所以更多的训练，更多的参数。是压缩后的字符串，就像你展示的那样，将两个字符串连接在一起[听不清]单独地，然后计算距离。有一种方法是使用 gzip 的输出作为[听不清][?代码?][听不清]。

**答：** 是的。我对此唯一的评论是 gzip 不是一个非常强大的文本压缩器。所以我认为它确实表明在某种程度上事情是可能的，但是所有真正有实质内容的东西都发生在你挤压最后那点比特的时候，如果你明白我的意思的话。

**观众：** 它看起来像一个玩具级的概念验证，但它确实有效。

**观众：** 我认为之前那里有一些错误——

**ILYA SUTSKEVER:** 它无效。

**观众：** [听不清] 目前的结果。

**问：** 既然 Jacob 提到了课程效应（curriculum effects），以及它们如何出现在神经网络中，但对于——你看不到它，但对于柯尔莫哥洛夫复杂度来说却没有。我们午餐时还在讨论当前的经验情况是怎样的，关于课程效应实际上有多重要。我们都不知道答案。

**答：** 嗯，这有点——我对此有一个看法，那就是越容易——我们作为一个领域做了很多工作来使 Transformer，比如我们正在使用的架构，变得相对容易优化。我们找到了好的初始化方法。我们找到了好的超参数。我们对架构进行了修改，以便训练尽可能容易。训练优化问题越容易，你就越不容易受到课程效应的影响。这是已知的。例如，那些曾经训练各种奇特架构的人，比如神经图灵机（Neural Turing Machines），它们是这些非常复杂的东西。还有超级超级大量的异构层，它们是不同的。对于那种东西，你必须对你的课程非常非常小心，因为如果你一开始就给它完整的数据集，它就会失败。

**YEJIN CHOI:** 好的，让我们再次感谢 Ilya。[掌声]


# 要点回顾

好的，这是从视频脚本中提取的框架与要点内容，以简体中文输出，并按照要求进行了格式化：

**演讲主题：一种关于无监督学习的理论视角**

- **引言**
    - 演讲者 Ilya Sutskever (OpenAI) 被邀请分享关于大语言模型 (LLM) 和未来的看法。
    - 由于 OpenAI 当前很多技术工作涉及保密内容，演讲者选择分享一些关于无监督学习的早期（约2016年）思考和成果。
    - 这些早期工作深刻影响了他对无监督学习的理解方式。
    - 演讲者设定了适度的期望，希望内容能引起听众兴趣。

- **回顾监督学习：一个相对清晰的领域**
    - 学习为何有效？数据为何具有可被模型捕捉的规律性？
    - 监督学习理论（如 PAC 学习、统计学习理论）为学习的成功提供了数学基础。
    - 核心保证：若能在训练集上实现低错误率，且模型复杂度（自由度，如参数量）低于训练样本量，则模型在与训练集同分布的测试集上也能取得低错误率。
    - 数学表达（简化示意）：$P(\text{训练误差} \ll \text{测试误差}) \le \text{小概率}$。
    - 关键前提：训练分布与测试分布相同。
    - 因此，监督学习的成功是有数学保障的，概念上相对简单。
    - （旁注：VC 维度主要用于处理无限精度参数，在实际有限精度计算中，函数数量有限，可以直接应用简单的计数原理。）

- **无监督学习：困惑与挑战**
    - 无监督学习的定义：从未标记的数据中学习隐藏的结构。
    - 缺乏类似监督学习的明确成功保证。
    - 核心困境：优化一个目标函数（如重构误差、去噪误差、自监督损失），却期望在另一个不同的下游任务上获得好效果，其内在机制不清晰，看似“魔法”。
    - 历史上的无监督学习方法（如玻尔兹曼机、去噪自编码器）虽有想法，但在小规模数据上效果并不显著。

- **一种有保证的无监督学习思路：分布匹配**
    - 提出一种特殊的无监督学习范式：分布匹配。
    - 目标：给定两个独立的数据源 $X$ 和 $Y$（无样本对应关系），寻找一个函数 $f$，使得 $f(X)$ 的分布尽可能接近 $Y$ 的分布（$Dist(f(X)) \approx Dist(Y)$）。
    - 例子：机器翻译（将英语分布映射到法语分布），语音识别（文本分布映射到语音分布），替换密码破译。
    - 特点：在高维空间中，这种分布匹配约束足够强，可能恢复出有意义的函数 $f$。这种方法具有类似监督学习的“保证”。
    - 局限：这种设置在现实应用中可能过于“人造”或不直接适用。

- **核心框架：通过压缩理解无监督学习**
    - 提出使用“压缩”的视角来思考无监督学习，认为这比“预测”更直观、更有优势。
    - 基础：压缩与预测本质上是等价的（任何压缩器都是预测器，反之亦然）。
    - 关键思想实验：考虑两个数据集（大文件）$X$ 和 $Y$。将它们 *连接* 起来 ($X+Y$) 并使用一个足够好的压缩器 $C$ 进行联合压缩。
    - 核心洞察：一个强大的压缩器会利用 $X$ 中的模式来帮助压缩 $Y$，反之亦然。
    - 数学表达：联合压缩的长度 $C(X+Y)$ 应小于或等于分别压缩的长度之和 $C(X) + C(Y)$。差值 $C(X) + C(Y) - C(X+Y)$ 代表了 $X$ 和 $Y$ 之间的“共享结构”或“算法互信息”，被压缩器所利用。
    - 关联无监督学习：可以将 $X$ 视为无监督数据， $Y$ 视为有监督任务的数据。联合压缩提供了一个数学理由，说明 $X$ 中的模式为何能帮助关于 $Y$ 的任务。
    - 此框架也能解释分布匹配：如果存在简单的 $f$ 使得 $Dist(f(X)) \approx Dist(Y)$，好的压缩器应能发现并利用这一点。

- **理论极限：柯尔莫哥洛夫复杂度 (Kolmogorov Complexity)**
    - 引入柯尔莫哥洛夫复杂度 $K(X)$：能生成字符串 $X$ 的最短程序的长度。这是理论上最优的压缩器。
    - $K(X)$ 相对于任何实际压缩器 $C(X)$ 具有最低的“遗憾”（regret）：$K(X) \le C(X) + \text{const}$，常数是描述压缩器 $C$ 本身的复杂度。
    - 条件柯尔莫哥洛夫复杂度 $K(Y|X)$：在允许访问（查询）数据 $X$ 的条件下，生成 $Y$ 的最短程序的长度。
    - $K(Y|X)$ 定义了无监督学习的终极目标：利用 $X$ 中的所有信息来以最有效的方式“压缩”（预测）$Y$，实现零遗憾。
    - 结论：使用 $K(Y|X)$ 作为目标，可以确保最大限度地从无标签数据 $X$ 中获益，用于任务 $Y$。
    - 重要关联：在一定条件下，联合压缩 $K(X+Y)$ 与条件压缩 $K(Y|X)$ 效果相近。这意味着简单地将所有数据（无监督 $X$ 和有监督 $Y$）拼接起来，用最优压缩器进行压缩，就能实现最优的无监督学习效果。
    - 局限：柯尔莫哥洛夫复杂度是理论概念，不可计算。

- **连接现实：神经网络、SGD 与压缩**
    - 类比：训练大型神经网络的过程（尤其是通过 SGD 优化）可以看作是在进行一种“程序搜索”。
    - 神经网络 ≈ 有限计算能力的“计算机”或“电路”。
    - SGD ≈ 在这些“计算机”上搜索能很好压缩数据的“程序”（即网络参数）的算法。
    - 深度学习的成功依赖于 SGD 这个“奇迹”，它能有效地找到这些复杂的函数/程序。
    - 更大、更深的网络 ≈ 更接近理想的（但不可计算的）柯尔莫哥洛夫压缩器，能更好地捕捉数据中的复杂模式，从而在利用无监督数据时达到更低的“遗憾”。
    - 仿真论：解释了为何改进神经网络架构通常很难（除非克服了根本瓶颈，如 RNN vs Transformer），因为强大的旧架构往往能模拟新架构。
    - 联合压缩与最大似然：在机器学习中，联合压缩对应于在 $X$ 和 $Y$ 的并集上进行最大似然训练（最大化 $log P(X, Y | \theta)$），这是一种自然的操作。

- **实验验证：iGPT (Image GPT)**
    - 目的：在非文本领域（视觉）验证压缩框架的有效性。
    - 方法：将图像视为像素序列，使用类似 GPT 的自回归模型进行“下一个像素预测”，目标是最大化像素序列的似然（即压缩图像）。
    - 结果 (2020年)：
        - 在 CIFAR-10 等数据集上，模型在“下一个像素预测”任务上的性能（衡量压缩/无监督学习能力）与模型内部表示用于下游分类任务的线性可分性（通过 Linear Probe 测量）高度相关。
        - 模型规模越大，两方面的性能都越好，证明了通过优化压缩目标可以学习到有用的表示。
        - 在 ImageNet 上也取得了有竞争力的无监督学习效果。
    - 结论：实验有力支持了“好的压缩器（预测器）能够学习到高质量的通用特征”这一观点。

- **讨论与开放问题**
    - 线性表示之谜：压缩理论本身并未直接解释为什么模型会学习到特别适合 *线性* 分类的表示，这是一个待深入理解的问题。
    - 自回归 vs. BERT：实验观察到自回归模型（如 iGPT）似乎比掩码模型（如 BERT）在图像上学习到更好的线性表示。推测可能与预测任务的难度有关（自回归预测更依赖全局/长距离信息）。
    - 训练动态与数据顺序：神经网络训练受数据顺序影响（课程学习效应），这与理论上的 K 复杂度不依赖顺序的特性不同，反映了 SGD 搜索过程的特性。优化越容易，对课程学习的依赖可能越小。
    - 其他概率模型：扩散模型 (Diffusion Models) 如果以最大似然为目标，也属于压缩框架，理论上应有类似效果，但可能在表示学习和计算效率上有所不同。
    - 计算成本：当前的压缩理论框架主要关注信息量，忽略了实际计算成本，这是一个重要局限。
    - 模型大小与压缩：更大的模型（如 GPT-4）可能是当前最好的压缩器，但压缩器本身的大小（参数量）也增加了。理论与实践的权衡需要考虑测试集大小等因素。

- **总结**
    - 通过“压缩”（尤其是以柯尔莫哥洛夫复杂度为理想目标）的视角，可以为无监督学习提供一个更统一、更严谨的理论框架，解释其为何以及如何在实践中（通过大型神经网络）有效运作。
    - 核心思想是：好的无监督学习算法致力于找到数据中的共享结构并利用它进行压缩/预测，从而为下游任务提供价值。