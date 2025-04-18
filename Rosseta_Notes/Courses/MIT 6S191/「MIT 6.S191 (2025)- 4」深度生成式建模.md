
# 深度生成式建模
 - [MIT 6.S191: Deep Generative Modeling](https://www.youtube.com/watch?v=SdTZAMDKrNY&t=1747s)
- 博主官方：[链接](https://www.youtube.com/@AAmini)

### 导言

本次讲座系统性地介绍了生成式建模的基础理论与核心方法。在生成式人工智能飞速发展的今天，掌握其背后的原理显得尤为重要。讲座首先明确了生成式建模与监督学习的差异，将其归入无监督学习范畴，阐述了其核心目标——学习数据的底层概率分布 `p(x)`，并利用该分布生成全新的数据实例。讲座深入探讨了“隐变量”的概念，并以此为基础，详细讲解了两大类 foundational 模型：自编码器（Autoencoders, AEs）与变分自编码器（Variational Autoencoders, VAEs）。内容涵盖了它们的编码器-解码器架构、基于重构损失的无监督训练方式、VAE引入的概率化隐空间、KL散度正则化以及重参数化训练技巧。接着，讲座重点介绍了生成对抗网络（Generative Adversarial Networks, GANs），生动解释了其独特的生成器与判别器之间的“对抗”训练过程，并展示了其在分布转换和样本生成方面的能力，同时提及了CycleGAN等重要变体。讲座结合实例讨论了这些技术在特征发现、异常检测、新数据创造及数据偏见处理等方面的应用价值。以下为本次讲座内容的完整文字实录，适合希望深入了解生成式建模基础的读者阅读。

### 讲座内容纲要

```
生成式建模讲座纲要
├── 一、生成式建模 (Generative Modeling) 导论
│   ├── 讲座主题介绍与重要性 (当前 Generative AI 时代)
│   ├── 生成式建模核心概念 (超越模式识别，生成新数据)
│   ├── 与监督学习对比
│   ├── 无监督学习定义
│   ├── 生成式建模基本原理 (学习数据分布 p(x))
│   ├── 两大应用方向
│   │   ├── 密度估计 (Density Estimation)
│   │   └── 样本生成 (Sample Generation)
│   ├── 核心挑战 (如何有效学习 p(x))
│   ├── 重要性与应用场景
│   │   ├── 特征发现 (如人脸特征、数据公平性)
│   │   ├── 异常检测 (如自动驾驶)
│   │   └── 新数据生成 (Generative AI 基础)
│   └── 本讲座重点 (AE/VAE, GANs)
│
├── 二、隐变量 (Latent Variables)
│   ├── 概念引入 (柏拉图洞穴寓言)
│   ├── 定义 (无法直接观测的底层特征/结构)
│   └── 生成式建模目标之一 (捕捉和提取隐变量)
│
├── 三、方法一：自编码器 (AEs) 与变分自编码器 (VAEs)
│   ├── 1. 自编码器 (Autoencoder, AE)
│   │   ├── 基本思想 (自我编码)
│   │   ├── 结构 (编码器 Encoder, 解码器 Decoder)
│   │   ├── 低维隐空间 z 的意义 (压缩, 提取核心特征)
│   │   ├── 训练方式 (无监督, 重构损失 Reconstruction Loss, 如 MSE)
│   │   ├── 核心机制 (瓶颈层 Bottleneck)
│   │   └── 问答：为何关心 z 的维度？(提取重要特征)
│   │
│   ├── 2. 变分自编码器 (Variational Autoencoder, VAE)
│   │   ├── 动机 (引入随机性以生成新样本, 学习良好隐空间)
│   │   ├── 与 AE 的关键区别 (z 是概率分布而非确定点)
│   │   ├── 概率视角 (编码器学 p(z|x), 解码器学 p(x|z))
│   │   ├── VAE 损失函数
│   │   │   ├── 重构损失
│   │   │   └── 正则化项 (KL 散度, 对比 p(z|x) 与先验 p(z))
│   │   ├── 正则化的目的与隐空间性质
│   │   │   ├── 先验选择 (常用标准正态分布 N(0,1))
│   │   │   ├── 期望性质：连续性 (Continuity) & 完备性 (Completeness)
│   │   │   └── 正态先验如何帮助实现这些性质
│   │   ├── 训练技巧：重参数化技巧 (Reparameterization Trick)
│   │   │   ├── 问题 (采样操作阻断梯度)
│   │   │   └── 解决方案 (分离随机性 z = μ + σ * ε)
│   │   └── VAE 应用与特性
│   │       ├── 生成新样本
│   │       ├── 隐变量的可解释性 (如控制人脸姿态)
│   │       └── 应用于特征发现与数据去偏见
│   │
│   └── 3. AE/VAE 总结 (压缩, 无监督, 随机性, 可解释性, 生成)
│
├── 四、方法二：生成对抗网络 (Generative Adversarial Networks, GANs)
│   ├── 主要目标 (生成高质量新样本)
│   ├── 核心思想 (学习从简单分布到目标分布的转换)
│   ├── 架构：两个竞争网络
│   │   ├── 生成器 (Generator, G): 噪声 -> 假数据, 目标: 欺骗 D
│   │   └── 判别器 (Discriminator, D): 输入真/假数据, 目标: 区分真假
│   ├── 训练过程 (对抗训练, Minimax 博弈)
│   │   └── 1D 直观示例 (逐步逼近真实分布)
│   ├── 理想状态 (纳什均衡, G 完美模仿, D 无法区分)
│   ├── GAN 的能力
│   │   ├── 分布转换
│   │   └── 平滑插值 (噪声空间插值 -> 数据空间平滑过渡)
│   ├── GAN 的变种：CycleGAN
│   │   ├── 功能 (非配对域转换, 如马 <-> 斑马)
│   │   ├── 应用实例 (风格迁移, 语音转换 - 奥巴马例子)
│   │   └── 机制 (循环一致性损失)
│   ├── 问答：GAN 损失函数细节 (Minimax 公式解释)
│   ├── 问答：GAN 训练稳定性问题
│   └── GAN 总结 (竞争机制, 侧重样本生成, 与 VAE 对比)
│
└── 五、总结与展望
    ├── AE/VAE 与 GAN 作为 foundational 方法
    ├── 为 Diffusion, LLMs 等先进模型铺路
    ├── 驱动当前 Generative AI 浪潮
    ├── 未来课程预告 (Lec 6 & 10: Diffusion Models)
    ├── 本次实验课内容介绍 (基于 CNN 的 VAE 做人脸检测与去偏见)
    ├── 结束语 & 助教介绍
    └── 问答：Piazza 平台, 助教 Victory 介绍

```



## 讲座实录：深度生成式建模

### 一、 生成式建模（**Generative** Modeling）导论

大家好，接下来这节课，无论从主题本身还是从生成式建模的相关性来看，都是我最喜欢的课程之一。我想，大家来到这里，可能也是因为认识到我们正处在一个生成式AI的非凡时代。今天，我们将深入学习生成式建模的基础知识。我们将探讨如何构建系统，这些系统不仅能在数据中寻找模式并利用这些模式做决策，更能超越这一步，基于学习到的模式实际生成全新的数据实例。

这是一个极其复杂且强大的思想，在过去几年里，它在众多应用领域呈现爆发式增长。实际上，我们已经初步感受到了这类生成式模型的强大和巨大潜力。昨天的课程开始时，我们就展示了图像生成和音频生成方面的一些进展。今天，我们将继续沿着这个主题深入探讨。

这里有三张人脸照片，我想请大家花点时间思考一下，这三张脸中，哪一张是真实的？

（稍作停顿）

认为A是真实的请举手？（观察）认为B是真实的？（观察）认为C是真实的？（观察）

好的，看起来选A的是大多数。但实际上，这三张脸都不是真实的，它们全都是假的。这确实凸显了这些方法的逼真程度以及生成式建模的力量。

的确，借助生成式建模，我们能够处理一系列全新的学习问题。到目前为止，在本课程中，我们主要关注的是所谓的监督学习问题。这意味着我们获得一组带有标签的数据，我们的目标是学习一个从输入数据到标签（比如类别标签或数值）的映射。因为这是一门关于深度学习的课程，我们一直关心的是学习由深度神经网络定义的这些映射。但从根本上说，那个从数据映射到标签的函数可以是任何东西。

现在，我们要把注意力转向一类全新的问题，即所谓的无监督学习。在这种情况下，我们只有数据，不一定有标签。我们的目标是构建一个深度学习模型，该模型能够学习数据底层的结构和模式。这可以让我们在基础层面洞察数据的分布，并能被用来实际生成全新的数据实例。

生成式建模——作为无监督学习的一个实例和类型——其根本原理是：给定来自某个训练集的样本，我们想要学习一个模型，该模型能够表示我们从中采样的数据的分布。我们可以通过几种方式来使用这样一个模拟概率分布的生成式模型。

第一种方式是进行所谓的密度估计。其原理是，给定一些遵循某个概率分布的样本，我们想要训练并构建一个模型，该模型能够学习描述和捕获这些数据来源空间的底层概率分布。当我们学习了这个分布后，它允许我们从这个概率分布中采样，从而实际生成全新的数据实例。因为我们构建的模型捕捉了数据底层的概率分布，这意味着生成的样本能够反映该分布。

在这两种情况下，我们潜在的问题都是：我们如何能有效地学习到这个概率分布 `p(x)` 的估计，使其尽可能地接近并类似于真实的数据分布？这就是生成式建模的核心原理：努力学习一个能很好地代表你数据的概率分布。

那么，我们为什么关心生成式建模？它在现实世界中有什么用处？首先，通过进行密度估计和概率分布学习，生成式模型能够揭示数据集中的底层特征。例如，如果我们有一个人脸数据集，里面可能有各种各样的面孔。事先我们可能不知道这些人脸在诸如发色、肤色、姿态、衣着等特征上的底层分布是怎样的。我们的训练数据可能在某些特征上过度代表，而在另一些特征上代表不足，我们可能并不知道这一点。正如大家将在今天的实验中看到的，使用生成式模型，我们可以自动地发现和识别这些特征，了解哪些特征的代表性或多或少，并利用这一点来创建更公平、更具代表性的数据集。

另一个很棒的例子和用例是异常检测。在Alexander介绍的自动驾驶和自主系统案例中，确保汽车能够处理在路上可能遇到的所有可能场景至关重要，而不仅仅是最常见的那些。使用生成式模型，我们可以识别那些罕见的事件，那些位于我们概率分布尾部的异常值，并利用这一点来检测这些罕见实例，并相应地调整汽车的控制。

最后，也许是许多人最感兴趣或最熟悉的用例，那就是实际使用生成式模型来创建新的数据样本和实例。因为这些生成式模型在建模和学习概率分布，这意味着从该分布中采样会产生新的数据实例。这确实是生成式AI的根本支柱。在本课程中，大家将看到这个概念在从自然语言到计算机视觉，乃至科学和医疗保健等领域是多么强大。

希望这些能激发大家对生成式模型的兴趣，并为我们为什么如此关注它奠定基础。今天，我们将重点关注两类基础的生成式模型：隐变量模型，具体分解为自编码器，以及一个我们称为生成对抗网络（GANs）的基础架构。

### 二、 隐变量（Latent Variables）

这两类基础模型都属于我们所说的隐变量模型。要理解这一点，我们首先需要明白什么是隐变量。

我认为一个很好的例子可以阐释这一点，这个故事来自古老的著作——柏拉图的《理想国》，被称为“洞穴神话”或“洞穴寓言”。故事中，有一群囚犯，作为惩罚的一部分，他们被束缚着面向一堵墙。他们唯一能看到的东西是物体经过他们身后的火堆时投下的影子。他们只能看到墙上的投影或影子。对于这些囚犯来说，那些影子，那些观察到的现象，就是他们的现实。但他们无法直接看到或测量那些投下他们所观察到的影子的真实结构。那些在囚犯头后的物体，就像是决定数据集分布的底层特征或潜在的隐变量。而我们所能做的，只是提供某种方式来观察那些数据实例。但也许我们最终关心的，是捕捉那些产生我们所能观察到的现象的、驱动性的底层特征或隐变量。

所以，我们生成式建模的目标之一，可以看作是找到一种有效的方法，在只给定一些观测数据的情况下，捕捉和提取这些底层特征，即隐变量。

### 三、 方法一：自编码器（Autoencoders, AEs）与变分自编码器（Variational Autoencoders, VAEs）

**1. 自编码器（Autoencoder, AE）**

我们将要探讨的第一种方法，是一个简单直观的生成式模型，我们称之为自编码器。这些模型试图做的是对它们看到的输入数据进行自我编码。

让我们通过手写数字图像这个简单的例子来看看自编码器是如何工作的。这里，我们以图像作为原始数据输入，将其传入一个深度神经网络，比如卷积层。最终，自编码器所做的是，它通过这些连续的层，试图输出一个低维的隐空间（latent space），即数据的表示，这是我们试图建模和预测的目标。我们称这个网络为编码器（Encoder），因为它将数据 `x` 映射到这组隐变量 `z`。

现在，让我们问问自己，我们为什么要关心这组隐变量 `z` 的维度？
（稍作停顿，面向听众）
关于我们为什么要关心我们试图学习的隐变量的数量，大家有什么想法吗？

**问：**（听众席，模糊不清，大意是提取重要特征）
**答：** 我们想要提取最重要的特征，这些特征可能对其他方面来说不是必需的。

**答：**（讲者）完全正确。我们试图提取并浓缩到那些最重要的特征。保持一个较低维度的隐空间意味着我们有效地压缩了数据，将其编码成一个小的潜在向量，并学习这种非常紧凑、非常丰富的特征表示。

现在的问题是，好吧，如果我们能够生成这个低维的隐空间，我们如何实际训练模型来学习这个隐变量向量 `z` 呢？我们是否有关于这个训练数据 `z` 的任何明确的例子或标签，供我们尝试建模？我们能进行普通的监督学习吗？

**问：**（听众席，思考状）
**答：** 我认为原则上我们有数据，但我们没有（标签）数据。所以我们添加一些……

**答：**（讲者）是的。如果我们对我们关心的特征有一些先验知识，也许可以。我们可以尝试对此进行监督。但请记住，我们的根本目标是自动地发现这些特征。我们希望直接从数据中学习，无需任何监督，这样我们就不会因为我们人类对哪些特征是重要的先入之见而产生偏见，而是以数据驱动的方式来确定。

所以，想法是，我们不使用由我们人类预先指定的标签，而是利用数据本身作为信号，以无监督的方式学习这些特征。我们可以这样做：不假设这些特征是什么的任何标签，而是尝试去重构输入。我们训练一个神经网络，从图像的像素空间开始，下降到这个低维空间，然后构建一个解码模型（Decoder），该模型能够从那个隐空间重构出原始图像。

现在，在这里，我们可以比较原始输入和重构输出，并通过简单地最小化输入与重构输出之间的距离来训练网络。在图像中，一种简单的方法是采用输入和重构输出之间的均方误差（Mean Squared Error, MSE）。将两张图像相减，然后对差值平方，这就给了我们一个像素到像素的度量，衡量输入与重构之间的差异。

所以，你可能体会到的是，现在如果我们看我们实际用来训练网络的这个损失函数，它不需要任何关于标签的规定，也不需要知道这些重要特征的身份。我们仅仅利用重构输入的信号，就可以作为学习这些特征的一种方式。

让我们稍微简化一下这个图示，抽象掉自编码器这两个组件——编码器和解码器——中的各个层。再次强调，我们的损失函数根本不需要任何标签。这确实是一个非常强大的想法，因为现在我们具备了无监督学习的能力。我们可以学习像那些隐变量 `z` 这样的量，而无需任何预先指定，也无需直接观察到它们。

回到关于隐空间维度为何重要的问题。它对你能够提取的特征的丰富性以及你设置的瓶颈有巨大影响。如果我们把自编码的概念看作是一种压缩形式，那么这意味着隐空间的维度越低，我们压缩数据的程度就越高，我们在重构方面的表现就越差。因此，现在，这种自编码方法的关键概念是，我们可以使用这个瓶颈隐藏层来提取这些隐特征 `z`，而无需任何预先指定或监督的标签，只需使用一种称为重构损失的损失函数，它通过解码回传并重构输入的过程，迫使网络尽可能多地编码信息。通过这种方式，我们自动地将数据中的信息编码到隐空间 `z` 中。

**2. 变分自编码器（Variational Autoencoder, VAE）**

自编码器的这个原理，在实践中，常用的是对其思想的一种扩展和变体，它引入了更多的多样性，以便能够实际生成新的数据样本。这就是变分自编码器（VAEs）的概念，它确实是隐变量建模能力方面一个非常重要的主力生成模型。

正如我们刚才看到的，在传统的自编码器中，操作是确定性的。我们的编码器中有普通的神经网络层，就像我们之前看到的任何其他层一样。我们的解码器中也有普通的层，它们接收隐变量并解码输出以生成结果。但这带来的问题是，如果我们输入一个数据，只要权重保持不变，我们总会得到相同的重构输出。如果我们不改变权重，给定的输入总会产生相同的重构输出。可以将其视为一种确定性编码，允许我们重构输入。

对于VAEs，为了学习一个高质量的隐空间，我们实际上需要在这个自编码器中引入一些随机性，一些随机过程（stochasticity）。这就是变分自编码器（VAEs）背后的原理。

在VAEs中，我们现在不再拥有一个纯粹确定性的层 `z`，而是要引入一些采样，一些随机性的概念。我们不再直接学习隐变量。如果我们把每个隐变量参数化为一个由均值 `μ` 和标准差 `σ` 定义的概率分布，我们现在可以分别学习这些均值向量和标准差向量，使得我们在隐空间中的每个隐变量都有一个分布。这意味着，它仅仅是在自编码概念上的一个概率性扭转。实际上，这意味着现在我们可以从这些均值和标准差中采样，从而产生新的数据实例。大家可以看到，VAEs 与编码、下降到隐空间、再解码回原始数据空间的概念是相同的，只是加入了这种概率性的扭转，使得我们可以通过这些隐变量层进行采样。

如果我们现在开始让这个概念更形式化一点，实际上，编码器和解码器所做的就是试图学习概率分布。编码器计算给定输入数据 `x` 时隐空间 `z` 的概率分布 `p(z|x)`。而解码器则做相反的事情，试图计算给定隐变量 `z` 时数据 `x` 的概率分布 `p(x|z)`。这两个网络由两组独立的权重 `φ` 和 `θ` 定义。但我们可以用一个单一的损失函数来端到端地训练这个网络，这个损失函数是输入数据 `x` 以及这两组权重 `φ` 和 `θ` 的函数。

现在，如果我们仔细看一下这个损失函数是什么样子的。我们有两项：一项是重构损失，这与我们在标准自编码器中看到的非常相似；第二项是一个新的项，称为正则化项，我们稍后会更详细地讨论它。

对于重构损失，它和之前一样。你可以把它看作是你的输入与你的重构输出之间的误差或比较，你希望尽可能地匹配，使其尽可能接近，做到忠实的重构。

现在，对于正则化项，事情变得更有趣一些。回想一下，我们现在试图学习的是给定数据 `x` 时这些隐变量的概率分布，这是由编码器计算的。作为正则化这个概率分布的一部分，这意味着我们想要对这些隐变量的分布应该是什么样子做出一些初始的先验猜测。这有助于我们推断并强制隐变量遵循这个先验。因此，当我们引入这个正则化项时，我们需要一种方法来计算隐变量的分布与我们对其概率分布应有的先验之间的距离感。

为了进一步分解这一点，`D` 实际上只是一个距离度量。我们比较的是，推断出的隐变量的概率分布与我们对其分布应有的某种先验（我们设定的初始猜测）有多相似。

为了更深入地理解这一点，让我们首先思考我们甚至如何选择这个先验以及它为什么重要。为VAE选择先验的一种非常常见的方法是说，好吧，让我们做一些简单的事情。假设我们促使这些隐变量大致遵循一个均值为0、标准差为1的正态分布（Normal Distribution）。这鼓励我们VAE中的编码器现在尝试将隐变量均匀且平滑地分布在隐空间的中心周围，并分布编码，以便我们可以平滑地覆盖这个隐空间。

就像任何其他的损失函数，如交叉熵损失或均方误差一样，我们需要一个度量来计算我们离那个初始先验有多近。一种非常常见的方法是使用一种距离度量来比较两个概率分布有多接近，这个度量被称为KL散度（KL Divergence）。对于正态先验的KL散度的公式这里展示了，但实际上，你可以把它看作是一种计算和量化两个概率分布之间距离的方法。

好了，到目前为止，你可能在想，好吧，我理解我们试图学习这些隐变量的概率分布的原理，我们也希望它们的外观有一些先验，但这到底为什么重要呢？我们为什么甚至需要设置这些先验？为什么我们需要用正则化来约束我们的隐空间？

为了获得直观理解，让我们首先考虑我们希望我们的隐空间实际达到哪些属性。我们在学习这些特征时关心的第一件事是所谓的连续性（Continuity）。这意味着，如果我们有两个数据实例，并且它们在隐空间中最终靠得很近，那么这两个数据实例中应该有相似的内容。也就是说，隐空间中的接近对应于数据空间中的接近。第二个标准是这个完备性（Completeness）的概念。我们不希望存在间隙，意味着如果我们从隐空间中的某个地方采样，我们应该仍然能够重构或解码出一些有意义的数据实例，它不应该是完全随机或完全无用的垃圾。

为了更直观地理解这一点，让我们现在考虑一下，如果我们对这些隐变量不施加任何先验并且不对它们进行正则化，会有什么后果。没有正则化，我们可能会遇到这样的情况：隐空间中的两个点在我们的原始数据空间中具有完全不同的含义。在这个例子中，我们考虑的是形状：正方形、三角形和圆形。这里，如果一个正方形和一个三角形在隐空间中最终靠得很近，但在解码后或在原始数据空间中并不相似，那这是不希望的。我们希望三角形映射到离其他三角形更近的地方，而不是离正方形更近。其次，如果我们没有完备性，如果我们只是从隐空间中随机抽取一个样本，我们可能会得到无意义的曲线，而不是有意义的形状。

相比之下，正则化允许我们做的是鼓励这种接近性，使得在隐空间中接近的点在语义上是相关的，即相似的形状。同时，它也鼓励完备性，意味着我们可以从隐空间网格的任何地方采样，并且在解码时仍然能得到一个好的形状。

所以，这是一个非常非常重要的概念：使用隐空间的正则化来确保连续性和完备性。需要牢记的是，仅仅选择某个概率分布并不一定能保证这些属性。没有一个好的正则化项和好的先验，我们的隐空间质量仍然可能存在问题。事实证明，通过使用正态先验，我们能够相应地正则化隐变量，通过将均值居中并控制方差的扩展，从而鼓励这些隐空间中的连续性和完备性。

希望这传达了关于正则化概念的一些直观理解，以及为什么像正态先验这样的先验通常能够很好地工作，以构建一个既连续又完备的隐空间。

这在核心上触及了隐变量建模的概念，以及通过VAEs，我们如何从编码到隐空间，再解码回来。最后一步是明确，有了损失函数的这些组成部分——重构项和正则化项——我们如何能够实际地端到端训练网络。

我们遇到的问题是，因为我们有这个概率性的隐空间，我们无法将梯度反向传播回去。我们不能像在第一讲中看到的那样正常地进行反向传播。反向传播需要确定性的神经网络层或神经网络节点。

解锁训练VAEs能力的关键思想，实际上是对这个采样操作进行巧妙的修改，以允许使用反向传播进行端到端训练。我们不直接从由均值和标准差参数化的正态分布中采样我们的隐变量 `z`，而是可以将隐变量 `z` 采样为固定、确定性的均值 `μ` 集合，加上固定的标准差 `σ` 集合，并将这些标准差乘以另一个控制我们关心的所有随机性、所有随机过程的项。我们称这个常数为 `ε`。实际上，这意味着现在 `z` 是 `μ` 加上 `σ` 乘以这个从那个正态先验中抽取的随机常数 `ε` (`z = μ + σ * ε`)。

我们可以通过现在看这样一个图表，以及它如何影响反向传播和实际训练网络，来非常清晰地可视化这一点。最初，如果我们试图直接通过这个采样节点 `z`，我们无法反向传播，也无法传递梯度。相反，如果我们现在将 `z` 分解出来，把所有的采样随机性都控制和编码到这个随机常数 `ε` 中，我们就可以允许梯度直接通过 `z` 反向传播，一直回传到输入 `x`。这现在真的非常非常重要，因为我们现在可以实际地端到端传递梯度，并基于数据以数据驱动的方式学习这些隐变量。

最后，一旦我们训练好了网络，VAEs 的强大之处在于，我们可以进入并检查那些隐变量，看看模型在编码和解码过程中实际学到了哪些特征。而且非常优美和直观的是，这些特征通常在原始数据空间中具有可解释的对应关系。

所以，如果我们看看在图像的背景下如何做到这一点。假设我们有一个在人脸图像上训练好的VAE。现在我们从隐空间的变量中采样，通过解码来生成新的数据实例。如果我们能保持除一个变量之外的所有变量固定，只慢慢地扰动单个隐变量的值，你可以看到，这实际上对应于一个非常可解释的特征，关于图像中的什么东西被这个隐变量捕捉到了。在这种情况下，是姿态，头部相对于摄像机的视角变化。

所以，这触及了这样一个概念：通过像VAE这样的方法，我们能够捕捉到不同的隐变量，这些隐变量对应于我们所关心的数据空间中不同的可解释特征。正如大家将在软件实验课中看到的，我们可以使用这些能够揭示底层隐变量的模型，作为一种手段来实际发现数据集中哪些特征相对充分地被代表了，或者哪些特征代表不足。这对于我们思考用于训练这些深度学习模型的数据集中可能存在的偏见或代表性不足问题，具有非常非常重要的意义。大家将在软件实验课中亲身体验这一点，在那里你们将实际构建一个VAE模型，来自动发现人脸数据集中潜在的特征。

好了，总结一下这些自编码器方法（如VAEs）的关键概念：
-   它们能够将数据压缩成一组维度较低的隐特征。
-   我们可以完全无监督地做到这一点，无需任何标签，只需通过解码器从这种表示中重构原始输入。
-   我们可以在完全无监督的方式下生成重构。
-   我们看到了如何使用重参数化技巧来端到端地学习这些网络。
-   我们也看到了这些隐变量实际上具有关键意义，对应于我们所关心的数据空间中重要且可解释的特征。
-   最后，通过从这些隐变量中采样，你可以使用网络的解码器部分来生成原始数据空间的全新实例。

所以，VAEs确实为我们提供了一种非常强大的方式，将对一组隐变量的密度估计与通过解码进行的样本生成结合起来。

### 四、 方法二：生成对抗网络（Generative Adversarial Networks, GANs）

但如果我们的主要目标是生成新的样本作为输出，而我们不太关心拥有一组可能具有可解释性的隐变量呢？一个非常早期且非常基础的、更侧重于样本生成的方法，是一种称为GANs或生成对抗网络的方法。

GANs的原理是基于这样一个事实：如果我们只关心生成与我们训练模型所用数据非常相似的新数据实例？这意味着我们试图从这个极其复杂的分布中采样，并且我们希望我们的模型学习一种好的方式来近似该分布。直接学习这个分布可能非常非常困难。因此，GANs提出了一种方法，将非常简单的东西，甚至像完全随机的噪声一样简单的东西，转换为我们实际关心的复杂数据分布。正如我们将看到的，GAN方法训练一个生成器模型，该模型可以学习一个从完全随机噪声的分布到我们训练样本分布的映射。

GANs采取的方法实际上相当聪明和有趣。我们的目标是产生这种生成数据的分布，使其尽可能接近真实数据。GANs提出了一种通过将两个相互竞争的神经网络——一个生成器（Generator）和一个判别器（Discriminator）——并排放置在一起来实现这一目标的方法。其概念是它们处于一种相互对抗的状态中。

生成器网络的任务是尝试从完全随机输入噪声的分布出发，产生数据的仿制品。然后，判别器查看那些据称是数据仿制品的生成实例，它的目标是试图辨别什么是真实的，什么是假的，并学习一个分类器来区分真实与虚假。通过让这两个网络相互竞争，我们可以试图迫使判别器学习得非常好，知道如何区分好的真实数据与假数据。而当它在这方面变得越好时，它又反过来迫使生成器在产生能够试图欺骗判别器的假数据方面做得越来越好。

为了理解这背后的直觉以及它是如何工作的，让我们从这个我最喜欢的、传达这种直觉的插图例子开始。假设我们只有一条一维线上的数据。有一些假数据的实例，它们会落在这条线上的某个位置。记住，生成器是从完全随机的噪声开始的。所以，最初没有任何训练时，它在产生假数据方面不会很擅长。它产生了一些实例。现在，判别器看到了这些点，它也看到了一些真实数据。它的任务是经过训练，能够输出它看到的任何给定数据样本是真实的概率。

所以，我们要训练判别器。一开始，它的预测可能不怎么样。但我们训练它，它开始提高真实数据的概率，降低假数据的概率，直到我们得到一个完美的分离，判别器可以完美地区分什么是真实的，什么是假的。

现在，轮到生成器了。它看到了真实数据的位置，然后开始将其生成的假数据越来越靠近那些真实实例。现在，判别器接收到这些新的点，这新一轮的生成。它的任务再次是训练和学习如何区分真实与虚假。它将估计任何给定点是真实的概率，并学会降低假数据点的概率，提高真实数据点的概率。

我们再重复一次。生成器开始将其创造物移得越来越近，越来越靠近真实数据，以至于假数据几乎完全与真实数据的位置重叠。现在，在这一点上，对于判别器来说，要将其分类器应用于这些实例，并很好地区分真实与虚假将变得非常非常困难，因为那些生成的实例与真实数据如此接近。

所以，这确实是GAN这两个组件如何本质上相互竞争的核心直觉。

回到我们的图表，我们可以这样总结：生成器只是试图创造新的数据实例来欺骗判别器，而判别器则试图通过生成器与判别器之间这种竞争性的目标来识别这些实例。理想情况下，我们达到一个最优状态，生成器能够完美地再现真实数据分布，并完全欺骗判别器的分类能力。

所以，这确实是一个非常有趣和好玩的想法，最初引发了人们对生成式模型的极大热情。我希望大家从根本上理解的是，你可以把像GANs这样的生成式模型看作是在学习一种分布转换。从能够纯粹的高斯噪声、随机噪声出发，最终能够产生跨越学习到的目标分布的实例。

当一个训练好的GAN的生成器在合成新实例时，它所做的就是利用它学到的从高斯噪声分布到目标数据分布的映射，来学习从噪声分布中某一点到目标数据空间中特定输出点的映射。如果我们考虑噪声初始分布中的另一点，另一个初始点，并将其输入生成器，那么它现在会在目标数据分布的别处，在数据流形的别处产生一个新的实例。

我们实际上可以做的是，在完全随机噪声的空间中平滑地插值和遍历。事实证明，这会在学习到的数据流形中产生实际的平滑插值。正如你所看到的，结果是相当惊人的，我们可以非常具体地看到一系列的转换，反映了这种对数据空间的可解释的遍历或横穿。

所以，这是一个非常强大的概念，触及了分布转换的理念。我们可以做一些看似疯狂的事情，比如从完全随机噪声的分布转到某个目标分布。我们也可以做一些事情，比如从一个不是随机的源头转到另一个目标源头。GANs的一些变种，例如CycleGANs，正是提出了这一点。我们不从高斯噪声开始移动到目标数据流形，而是可以考虑一个数据流形，并尝试学习一个将我们带到另一个数据流形的映射。

这非常酷，因为它带来了一些明显的能力，比如在风格转换方面。例如，在图像中，我们可以使用这种称为CycleGAN的架构，在两种风格之间进行完全不成对的图像翻译。这个可视化向您展示了一个在自然图像上训练的CycleGAN。这里我们看到的是从马的领域到斑马的领域的域转换。这实际上是风格转移的概念。CycleGAN的工作原理是，它们采用这种循环损失，你实际上有两套生成器和判别器，每个域各一套，还有一个额外的代码依赖性将这两个域连接在一起。

事实上，就在几年前，我们自己构建了一个CycleGAN，来做我们在昨天开篇讲座中介绍过的事情，那就是语音和音频转换。事实证明，你实际上可以将音频波形表示为称为频谱图（spectrograms）的图像。与我们在斑马-马例子中看到的非常相似，我们在五年前所做的是训练一个CycleGAN，将语音频谱图从一种风格转换为另一种风格。

如果你还记得，Alexander展示了奥巴马介绍几年前我们使用的课程的视频片段。正如你所看到的，那个视频是合成的。不幸的是，奥巴马并没有真的莅临现场为我们介绍这门课。我们所做的，是使用了数小时的音频录音，然后将这些音频录音转换为源语音和目标语音的频谱图图像，并训练CycleGAN来完成这种从一个语音域到另一个语音域的非配对翻译。

（面向听众提问）
**问：**（听众席）你使用的（损失）函数是……？
**答：**（讲者）是的，让我实际调出它，我正好有。这是个好问题。核心原则是，我们希望将判别器和生成器放在一起，并联合优化它们，对吧？所以我可以实际调出确切的损失函数。

（展示或描述损失函数）

损失项基于比较真实数据与生成数据实例的相同直觉。首先，如果我们从判别器的角度考虑损失项，它寻求的是最大化数据被正确识别为真实的概率，以及（假数据）被正确识别为假的概率。正如你所看到的，这涉及到对生成器输出 `G(z)` 的判别，以及对真实数据 `x` 的判别——假的与真实的。再次强调，这关注的是判别器。

另一方面，生成器现在试图最小化其生成的数据被识别为假的概率。所以现在是相同的目标函数，但它做的是相反的事情：我们试图最小化假数据被分类为假的概率。我们希望尽可能地将其移向真实数据。

然后我们可以将它们结合起来。这里我们有一个项，它被判别器联合最大化，并被生成器联合最小化。所以这是一种双重、这种竞争性的目标。再次强调，核心直觉是，我们希望优化判别器，使其在区分真实与虚假方面做得尽可能好；并优化生成器，使其产生尽可能逼真、合成度高的实例。

**问：**（听众席，可能关于可微性）
**答：**（讲者）这是个好问题。它是可微的，但事实证明，在实践中，要稳定地训练GANs可能非常非常困难。因此，已经有研究提出了对这种损失函数的变体，或引入其他方法来尝试提高稳定性。

太棒了。

（稍作停顿）

所以，总结一下并或许结束关于GANs的部分。首先，核心原则是这两个网络之间的竞争，可以通过我们刚才看到的这个目标函数进行联合优化和训练。这与更侧重于密度估计的方法（如VAE）形成对比，在VAE中，我们的目标是真正学习能够捕捉数据中核心特征的底层隐变量，这些特征为我们的数据实例提供了一个低维表示。

### 五、 总结与展望

这些都是生成式建模的基础方法，它们为过去几年中取得的巨大进步铺平了道路，这些进步在许多领域都产生了非常非常高保真度和高质量的生成结果。我们将在明天的课程中看到一些生成式建模领域非常前沿和新兴的进展，包括像Diffusion模型、语言模型等，它们是驱动我们今天看到的生成式AI进展的核心工具。

所以，我最后给大家一个预告，我们在第6讲和第10讲中还有更多关于不同领域Diffusion模型的内容。希望这能让大家对生成式建模的前景和力量感到兴奋。大家将在今天的软件实验课中获得实践经验，该实验课将计算机视觉的主题与VAEs和生成式模型的主题结合起来，你们将实际训练一个基于CNN的VAE来进行人脸检测和人脸检测系统的去偏见处理。

那么，我们就到此结束。下载和开始实验的链接可以在线获取。在我们结束并进入答疑时间（office hours）之前，我想……我相信我们的助教今天也加入了我们。所以，如果你们能举手或到前面来，那就太好了，这样班上的每个人都能认识你们，并在软件实验上寻求你们的帮助。

（助教上前或示意）

**问：**（听众席）Piazza是……
**答：**（讲者）是的，Piazza是用于异步发布问题的地方。

**问：**（听众席）Victory是……
**答：**（讲者）是的，我们要进入答疑环节了。Victory是我们出色的助教之一。她将能够帮助回答与TensorFlow、PyTorch以及实验相关的问题。当然，如果大家对讲座内容本身有问题，Alexander和我也会在这里。

谢谢大家。