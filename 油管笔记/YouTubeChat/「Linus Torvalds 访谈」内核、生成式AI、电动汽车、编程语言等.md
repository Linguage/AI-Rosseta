
#  Linus Torvalds 访谈：内核、生成式AI、电动汽车、编程语言等

- [Linus Torvalds on the kernel, GenAI, EVs, programming languages and more…](https://www.youtube.com/watch?v=s4wlrxFf2lM)
- [TFIR](https://www.youtube.com/@TFiRio)

### 内容介绍

本文档整理了 Linux 创始人 Linus Torvalds 在奥地利维也纳开源峰会期间接受的一次深度访谈实录。在这场对话中，Torvalds 以其一贯坦诚和务实的风格，分享了他当下的工作状态与在 Linux 内核开发中所扮演的角色，并回顾了 Linux 生态系统从早期“狂野西部”到如今成熟稳定状态的演变历程。

访谈深入探讨了 Linux 内核社区的现状与挑战，包括社区规模扩张带来的管理模式变化、维护者面临的压力与吸引力，以及对潜在风险的思考。Torvalds 还阐述了他对 Linux 应用边界的看法，尤其是在微控制器等新兴领域，并分享了他对开源理念、贡献模式以及如何看待仅使用不贡献者的观点。

此外，内容还涵盖了 Torvalds 对具体技术话题的见解，如他对 C、Rust、C++ 等编程语言的态度，Clang/LLVM 编译器的整合历程，内核安全问题的处理哲学，以及对“永不破坏用户空间”原则的实践与考量。他还评论了当前热门的技术趋势，包括他对 AI 炒作周期的冷静观察和对电动汽车的个人体验。访谈最后也触及了他的工作沟通偏好、个人爱好等轻松话题。

### 内容纲要

```
Linus Torvalds 访谈纲要
├── 一、 Linus Torvalds 的近况与角色
│   ├── 当前主要工作：代码合并与审查
│   └── 角色定位：连接点与决策者（"坏人"）
├── 二、 Linux 内核与生态发展
│   ├── 对市场份额的态度：不关心，关注使用驱动的改进
│   ├── 开发模式变迁：个人贡献者 -> 大公司主导，更专业化
│   ├── 今昔对比：“狂野西部” vs. 稳定平静
│   └── 对当前流程的满意度：流程改进，牺牲部分兴奋感
├── 三、 内核社区健康与挑战
│   ├── 社区规模：指数级增长带来的变化
│   ├── 信任模型：层级化与维护者依赖
│   ├── 维护者现状：数量相对不足，部分过劳
│   ├── 维护者吸引力：技术挑战与职业价值
│   └── 潜在风险：关键人物依赖与专业知识集中
├── 四、 Linux 的应用边界与开源理念
│   ├── 微控制器领域：承认局限，接受小型 OS 的存在
│   ├── 开源模式：基础架构领域的必然选择
│   └── 对“搭便车者”的态度：接受其存在，非核心担忧
├── 五、 工作方式与沟通偏好
│   ├── 沟通工具：偏爱异步邮件，厌恶同步会议（Zoom/电话）
│   ├── 互动对象：主要与维护者交流，减少与新人直接互动
│   └── 邮件处理：选择性回复重要或有趣的问题
├── 六、 技术项目与工具
│   ├── 项目动机：解决自身需求（Git, Subsurface）
│   └── 未来项目：目前无新项目计划
├── 七、 Linux 桌面与硬件趋势
│   ├── Linux 桌面：个人满意度高，Web 化降低 OS 依赖
│   ├── 硬件发展：ARM 崛起，多架构支持利好 Linux
│   └── 软件模式：传统 OS 绑定模式式微
├── 八、 内核中的编程语言与兼容性
│   ├── C 语言：个人核心偏好
│   ├── Rust：接受其潜力，个人非重度用户，社区态度不一
│   ├── C++：个人不喜欢，但项目（Subsurface）中使用
│   ├── Clang/LLVM：支持其编译内核，过程漫长但已实现共存
│   └── 用户空间兼容性：坚持原则，但有例外（安全/维护）
├── 九、 安全性视角
│   ├── 核心观点：安全漏洞即 Bug
│   └── 主要痛点：安全保密性（Embargo）与开源模式冲突
├── 十、 对新兴技术与趋势的看法
│   ├── AI / GenAI：承认潜力，厌恶炒作，选择观望
│   ├── 技术热情点：个人持续关注软硬件接口
│   ├── Raspberry Pi：赞赏其普及价值而非技术本身
│   └── 电动汽车 (EVs)：喜欢其驾驶体验，对自动驾驶兴趣不大
├── 十一、 个人生活与爱好
│   ├── 主要爱好：阅读（消遣性）与水肺潜水
│   └── 对汽车的态度：实用工具，非爱好者
└── 十二、 结束语
    └── 个人理念：无意强加观点，开源是个人选择
```




---

# Linus Torvalds 访谈实录：开源峰会维也纳站

**主持人 (BH):** 嗨，我是主持人 BH，我们现在在奥地利维也纳的开源峰会上。时隔很久，我们再次请到了 Linus Torvalds。首先，非常高兴你能再次来到我们的节目。

**Linus Torvalds:** 也很高兴再次来到这里。我记得上次见面是几年前了，忘了是在哪里，可能是温哥华吧。那是在新冠疫情之前，你知道的，然后疫情打乱了一切。

## 一、 Linus Torvalds 的近况与角色

**问：** 这就引出了我的第一个问题，你最近在忙些什么呢？

**答：** 我还在做同样的事情。很少进行实际的开发工作。这周我做了大量的合并工作，因为现在是合并窗口期。过去至少十年都是这样，实际的编码工作由其他人完成，我扮演的更像是一个连接点，偶尔还得当那个说“不，这不对，我不能接受这种形式”的坏人。

但总的来说，我觉得内核开发一直都非常顺利。我们确实会遇到技术问题，但技术问题也是我们非常擅长解决的事情。所以，在过去几年里，我们并没有遇到任何重大的、棘手的问题。

## 二、 Linux 内核与生态发展

**问：** 生态系统已经成熟，应用也越来越广泛。你对 Linux 在 IT 领域的普及程度有多满意？

**答：** 事实是，我从来都不在乎这个。对我来说，我希望 Linux 被广泛使用，不是因为我关心市场份额之类的数字，而是因为使用能够发现 Bug，使用也能发现新的、有趣的用例，这些反过来会影响开发本身。但同时，对我而言，内核被使用的广泛程度从来不是首要问题，重点始终在于技术层面。所以我不做统计，也不去追踪哪些大公司在使用 Linux 之类的事情。我的自负已经足够大了，不需要再去弄清楚这些。

**问：** 我记得你曾经说过，你的自负小得像行星一样大，对吧？

**答：** 也许吧。

**问：** 现在还是这样吗？

**答：** 是的。

**问：** 但当我们环顾四周，几乎所有东西都在不经意间由 Linux 驱动。这也像我之前和 Dirk 聊到的，早期我们还在讨论为什么人们应该使用 Linux，而现在每个人都在用了。当你与社区互动时，对比过去，你看到了什么样的反差？

**答：** 我认为最大的反差在于，早期我们有更多个人贡献者，人们有很多他们需要修复的个人问题。而现在，很大程度上是因为我们已经解决了所有容易实现的目标（low-hanging fruits），很多开发来自于大型网站或有非常具体需求的巨头公司。通常，这些需求描述得也更清楚，因为这更专业了。

从某些方面来说，这有点更无聊了。过去更像是“狂野西部”时代，当我们还没有那么多大公司依赖最终结果时，我们可以做更多疯狂的事情。也许不像 25-30 年前那样有着好的意义上的疯狂。

**问：** 那你是更怀念那个“狂野西部”时代，还是更喜欢现在这种更稳定、平静的状态？

**答：** 我更喜欢稳定和平静。但同时，我确实有点怀念那种疯狂，怀念我们可以做一些不那么严肃的事情，怀念人们不像今天这样把 Linux 或者我个人看得那么重。我觉得今天我说话必须更加小心，因为人们太把我当回事了。早期的日子在很多方面更自由奔放，也更有趣。

但同时，从技术角度来看，我更喜欢我们终于弄清楚了如何正确地做事。这花了我们很长时间，我确实很享受这一点，我认为我们现在的流程比过去好得多。所以，你失去了一些兴奋感，可能也失去了一点个性，但在某个时刻你需要失去它，而那个时刻是几年前的事了。

## 三、 内核社区健康与挑战

**问：** 就像你说的，早期很多贡献者是个人，现在主要是公司。这对内核社区有何改变？因为曾几何时，我们也在讨论内核社区正在老化，需要新鲜血液。请谈谈你如何看待内核社区的实力和可持续性？

**答：** 我认为最大的变化与其说是严肃的商业大公司与个人的对比，不如说我们社区的规模变得庞大太多了。30 年前，大概只有几十个核心开发者和几百个参与者，而现在是几百个核心开发者和成千上万的参与者。这是一个巨大的变化。

这意味着你不再能像以前那样认识身边的每一个人，你必须能够更好地扩展（scale），必须扩展你的信任。你不能再信任身边的每一个人，你必须找到那些你认识的、属于你圈子的人。扩展开发的方式就是，这些人再去与他们信任的更多人合作。这改变了事情的心理层面。过去更像是一对一的关系，而现在，例如我，就必须依赖我经常互动的那顶尖的 50 或 100 位维护者。对于每个版本发布中涉及的上千名甚至更多的其他开发者，我已经没有一对一的关系了。这不仅仅是我，每个人都是如此，我们不得不变得更有组织性，拥有比很久以前更清晰的开发者层级结构。

我认为商业化的一面恰好与这个变化同时发生，但我不认为这是它们参与进来的原因。

**问：** 谈到技术，我们经常讨论技术人才短缺，当然最近也有很多裁员发生。但就内核社区而言，你是否觉得维护者和贡献者不够？还是你觉得我们现在的状况非常好？

**答：** 嗯，我们的状况不错。话虽如此，我认为我们的开发者确实比维护者多。我的意思是，我知道开发者比维护者多，但我认为如果我们有更多的维护者会更健康，这样我们现有的维护者有时就不会那么劳累。这在一定程度上取决于具体的领域。内核的不同部分情况各异，有些领域比其他领域更“幸福”，因为它们没有同样的……我的意思是，有些领域的开发者人均拥有更多维护者，这分散了工作量、痛苦和压力。

在很多方面，担任维护者压力可能非常大，因为现在你必须……在很多情况下，责任最终落到你头上（the buck stops with you）。作为一个只负责某个小驱动程序的终端开发者，压力会小很多，因为你只需要关心一件小事。而作为一个大型子系统的维护者，压力可能非常大。我希望我们能有更多的维护者，但这并不总是一份有趣的工作。

**问：** 内核社区不像一个组织，可以制定策略来吸引更多维护者。但你有什么方法来培养或壮大维护者队伍吗？

**答：** 嗯，壮大我们维护者基础的原因在于，这份工作可能不总是最令人愉快的，但它很有趣。如果你在寻找技术挑战，我觉得即使在 30 年后的今天，成为一名内核维护者仍然是你能做的最有趣的事情之一。好消息是，这份工作不仅受到其他内核维护者的赞赏，而且如果你是一名内核维护者，在行业内找工作往往也相当容易。所以，它确实有其优点。

**问：** 你是否看到（维护者）兴趣增长的迹象？或者你觉得这在未来 5 到 10 年，当现有的维护者变老或离开时，可能会成为一个问题？你觉得你面临的挑战是什么？

**答：** 所以，我担心的不是特定的领域，有时是特定的人和工作流程。例如，我曾经非常担心 Greg Kroah-Hartman，因为他承担了太多的工作。我和他谈过好几次，说：“嘿，你把自己摊得太薄了，你在做这么多事情，在这么多领域都如此重要，你确定这样健康吗？”他总是说他真的很享受他所做的事情，并且他已经将他所做的很多工作自动化到了一个他觉得压力并不大的程度。

还有某些子系统，只有一个真正承担了该子系统大量工作的人。我知道有些人觉得我说这话有点傻，因为我自己作为顶级维护者已经很久了。但同时，我觉得有很多人可以做我现在做的事情，他们可能不想做，但这并不需要非常专业的知识，更多的是关乎在社区中被信任。然而，我们在内核中确实有一些领域存在非常专业的知识，并且掌握这些知识的人非常少。我认为这比我这种情况更危险，虽然我在社区中被信任，但同时也有很多其他人同样被信任。

## 四、 Linux 的应用边界与开源理念

**问：** 如果你还记得 ARM 或 Nvidia 的早期，那些都是新的挑战。在现代世界，有哪些新的用例让你觉得潜力巨大但存在一些挣扎？或者你觉得 Linux 已经征服了一切，所以你甚至不再关心了？

**答：** 嗯，在某种程度上，我们在如此多的不同领域都做得如此出色，以至于我确实不那么担心了。我认为有一个用例，我觉得 Linux 的表现未必像一些人希望的那样好，那就是微控制器（Microcontroller）世界。我确实看到一些项目，人们为更小的工作负载开发了小型内核。我认为这很自然，而且我不认为这是 Linux 将会……我不是说“成长到”（grow into），而是“缩小到”（shrink into）的领域。人们尝试制作更小体积的 Linux 已经很长时间了，但这似乎从未真正成功。当你拥有一定量的、每个人都视为理所当然的基础设施时，你就已经超过了一定的大小。所以我接受 Linux 不会无处不在的事实，因为如果你想要一个非常小的、微型的设备，你可能使用一个非常小的、微型的操作系统会更好。

好消息是，通常那些小型微型设备会逐渐“长大”，然后它们终究还是想要 Linux。不过摩尔定律的终结可能会改变这个规则。

**问：** 是的，还有 Zephyr 等等，有很多实时操作系统（RTOS）。

**答：** 好消息是它们都是开源的。不仅仅是 RTOS，还有 Zephyr。我确实认为人们已经深刻认识到，当你做基础设施时，无论你做什么操作系统，它都将是基础设施，而开源是唯一的途径。试图制作一个定制的、商业化的小型操作系统是赚不到钱的，毫无意义。所以，是的，无论将来有什么在低端市场取代 Linux，我觉得它都将是开源的。

**问：** 我今天看到的是，几乎每个人都在使用开源，无论我们看向哪里。挑战在于他们并不知道那是开源，也没有成为良好的开源公民。你对此有何看法？

**答：** 嗯，我的意思是，这种情况一直存在：很多人、公司或领域想要使用开源，但不想参与其中。我觉得，好吧，这种情况永远不会消失。有些公司、有些人就是只想获取提供的东西，而不愿回馈。这是他们的选择，对吧？这意味着他们将不会参与未来更新的开发，也无法将项目的方向推向他们可能想要的方向。这就是一种权衡。

我不担心这个。有些人认为社区里有“寄生虫”（leeches），我不同意。我的意思是，不愿意参与开发本身也是可以的。有时候，他们可能没有额外的技术资源，也并非出于恶意，有时候只是……

**问：** 很多时候也与意识有关。

**答：** 嗯，是的。确实存在不良行为，有时确实是因为你是个坏人或坏公司，这个我无法改变，谁也无法改变。我们确实努力鼓励人们和公司做正确的事情。最终，显然也有一些组织，在极端情况下，会考虑采取法律行动。但我必须高兴地说，这种情况很少见，真的很少见。这并不是我个人觉得担忧的事情。

## 五、 工作方式与沟通偏好

**问：** 回顾 Linux 的早期，你喜欢和开发者互动，那些来自学校、大学的年轻孩子们。你现在还和那些年轻人互动吗？还是说你只和这些成熟的开发者打交道？我的意思是，你怀念那种与年轻人合作的感觉吗？因为他们看待世界的方式……我不是说你我老了，但我们确实……

**答：** 我现在不怎么和新开发者互动了。部分原因是性格问题，我不是一个擅长交际的人（people person），我从未声称自己是。即使我与其他开发者互动，我也更喜欢在技术层面上交流。而且，我们现在遇到的问题往往更多是关于维护，而不是一些真正革命性的新功能。所以我互动的人往往是其他的维护者。

这并不是说偶尔不会有人……这种情况确实会发生，人们知道我的电子邮件地址，我会忽略掉 90% 我觉得不需要回复的邮件。但仍然会有人发来有趣的邮件、有趣的问题，一个我觉得自己是少数能回答的人之一的问题，那我就会回复。正因为我觉得我只会回复那些我认为自己是权威的邮件，所以回复的往往是非常古怪、特定的领域。如果你给我发邮件只是问一个随意的 Linux 问题，我会忽略它。我甚至不会多想，我收到太多邮件了，我不会删除它，只会存档然后继续处理下一封。但偶尔，会有对开源和 Linux 非常感兴趣的高中生，他们仍然会提出有趣的问题，我偶尔也会回答这些。大多数问题并不有趣。

**问：** 内核开发仍然通过邮件列表进行吗？

**答：** 是的，我几乎完全还是基于电子邮件。我们显然使用 Git 进行实际的代码传输，但对于所有真正的讨论，对我来说，全是电子邮件。我很擅长忽略那些我不需要互动的邮件。我绝对厌恶 Zoom 通话或任何形式的视频会议，电话甚至更糟。而且它们对于内核开发来说效果非常差，因为每个人都处于不同的时区。所以电子邮件的整个异步特性对我来说远比……有些人喜欢使用聊天工具（Chat）和与人实时互动要合适得多。那不是我的风格。

不过，我完全使用电子邮件并不一定意味着其他人也都这样做。我们显然有人仍然在使用 IRC 或更现代的聊天工具，相当频繁，比如 Discord 等等。最终，电子邮件是我使用的方式，但不一定是其他所有内核开发者的方式。

**问：** 你不喜欢参加 Zoom 会议，是因为你还在浴室工作吗？因为你想说……引出你想问的，你的工作与生活是怎样的？

**答：** 嗯，部分原因是“浴袍问题”（bathrobe issue），虽然我这么说更多是开玩笑。更重要的是，我讨厌同步会议，因为那样你就必须……你必须把它记在你的日历上，必须在特定的时间出现在那里。这对我来说经常打断我的心流（flow）。如果我正忙于某件事，并且进展顺利，最糟糕的事情就是我的日历闹钟响了，提示“五分钟后开会”。

所以我一直积极地避免会议，基本上是从一开始就是。即使我在 Transmeta 工作时，不是做内核，而是作为公司内部的开发者，即使我在办公室，会议只是走过几个房间和人们坐在一起，即使那样我也绝对讨厌。就因为如果我正好在做某件事，它会打断你的注意力，让你脱离那个状态。所以我从来不喜欢任何需要你与他人同步的沟通模式，因为它对我来说效果不好。这就是为什么我不喜欢 Zoom，不喜欢电话，这也是为什么我对面对面会议也不是特别热衷。话虽如此，我喜欢面对面会议远胜于 Zoom 通话。我一点也不羡慕那些在新冠疫情期间每天开八小时 Zoom 会议的人。如果我必须开会，我宁愿和面前的人开会。

**问：** 是啊，还有个笑话是“这个会议本可以是一封邮件”。

## 六、 技术项目与工具

**问：** 在我们谈别的之前，既然你提到了 Git，你创建了 Linux，创建了 Git，然后创建了 Subsurface。还有其他你正在做的项目吗？或者我们应该制造一个问题让你来解决？

**答：** 我希望没有。我希望别人来做。我所有做过的项目都是因为我觉得当时没有其他可用的东西能解决问题。Git 尤其如此，我的意思是，显然有其他的源代码控制项目，但没有一个完全适合我的工作流程。

至于 Subsurface……现在，我实际上觉得我的需求被满足得很好。我没有看到其他任何新项目出现，但永远别说永远（never say never）。

## 七、 Linux 桌面与硬件趋势

**答：** （接上文）人们仍然嘲笑所谓的“Linux 桌面年”，但事实上，就我个人而言，过去近三十年对我来说一直都是“Linux 桌面年”，因为 Linux 一直在做我想让它做的一切，除了一些例外，比如 Git 和 Subsurface。

**问：** 不，既然你提到了 Linux 桌面，事实是 Steam Deck，你知道，这就是 Linux，我的意思是，我有一个 Steam Deck，也有华硕的那款（ROG Ally），我玩游戏……

**答：** 我其实从未尝试过 Steam，我根本不是游戏玩家。

**问：** 我是个重度玩家，所以我有一个 Steam Deck，也有这个，你知道的，当然还有 Android，还有现代的电动汽车，它们都运行在 Linux 上。所以桌面……还有微软的 WSL2，Linux 现在是默认自带的。所以，我的意思是，讽刺的是，微软已经成为了最大的发行商。

**答：** 是的，但我的意思是，即使在所有这些真正的 Linux 桌面出现之前，回想 20 年前，仅仅是 Web 以及大量使用 Web 浏览器就极大地改变了局面。20 多年前，你必须有一个 Windows 应用程序来做一些基本的事情，而现在，很多那些随机的、一次性的应用程序不再是应用程序了，它们是网页。所以我认为这对 Linux 桌面来说是巨大的变化，对于很多人来说，你最终真正需要的几乎就是一个 Web 浏览器，对吧？我的意思是，这就是 Chromebook 之类东西的背景。然后你确实有想要其他东西的游戏玩家。我们现在不再谈论这些了。

**问：** 所以在早期我们经常讨论这个，因为我们消费软件的方式也绝对改变了。那么你如何看待你和我们周围世界的变化？

**答：** 我实际上认为我们大多已经达到了一个平台期，但我确实认为我们将看到另一波增长，特别是现在有了 Windows 和整个 ARM 生态系统。这将再次推动任何试图以操作系统为中心、试图只支持 Windows 的剩余应用程序。这变得如此痛苦，我的意思是，通常尝试支持 Web 存在或更便携的模型要比传统的、几乎已经消失的软件模型容易得多。我认为它正变得越来越不重要。

这显然对 Linux 来说是件好事，尤其是我们支持这么多不同架构这一事实。过去确实是这样，我过去不仅运行 Linux，我还在 Alpha、PowerPC 上运行 Linux，然后是 ARM，嗯，ARM64。这些年来变得容易多了，因为软件行业中这种单一操作系统、单一架构的模式已经少了很多。

**问：** 即使是苹果，他们也转向了自己的 ARM 芯片，M1、M2、M3 芯片。所以大家都在转向 ARM。

**答：** 但他们以前也做过。我认为他们再次在过渡方面做得非常出色。部分原因是因为他们对整个生态系统的控制远超……当然远超 Linux 生态系统，Linux 生态系统是如此分散、广泛，有数百家不同的公司在做发行版之类的。所以在很多方面，苹果的模式要容易得多，因为他们控制硬件，也控制了他们软件栈的很大一部分。

## 八、 内核中的编程语言与兼容性

**问：** Rust 已经引入了内核。还有哪些语言是你正在拥抱的？或者有哪些你觉得很流行但你说“啊，现在还不行”的语言？

**答：** 我骨子里仍然是一个 C 语言的人。我老了，老狗学不会新把戏。我的意思是，我喜欢 Rust 的主要原因是没有什么真正令人厌恶的、可怕的东西。比如，我以不喜欢 C++ 而闻名，因为我认为那种语言做了太多糟糕的设计决策，以至于我不是无法想象用它编程——事实上，Subsurface 现在几乎完全是 C++ 写的——但它不是我喜欢的语言。

Rust 不是我热爱的语言，但同时，它也没有达到让我主动厌恶的程度。我认为它很有趣，我认为它可以带来新的想法和新的人。所以 Rust 不会是我个人会大量使用的东西。我希望随着它在内核中变得越来越普遍，我会更擅长阅读它，因为现在我看 Rust 代码时需要思考很多，它不像我看 C 代码那样自然而然，我看 C 代码看了太久了，甚至不用思考，看一眼就知道它在做什么。对我来说，Rust 代码还达不到那个程度，也许永远也达不到，那也没关系。

**问：** 那其他的维护者，比如 Greg，他们如何看待这些语言呢？

**答：** 哦，似乎有各种各样的看法。有些人真的完全不想和 Rust 扯上任何关系。Greg 似乎……他总是非常积极，对不同的人和不同的想法持开放态度，他似乎对 Rust 没问题。我不会开始点名，但有些人肯定不像他那样对整个问题持开放态度。这也很好，我觉得由此引发的所有口水战（flame wars）比什么都更有趣。老实说，如果你上网看看，很多关于 Rust 的负面讨论似乎并非来自核心内核开发者，而是很多随机的人，出于某种原因持有非常强烈的观点。

**问：** 那么，还有没有其他语言或项目试图进入 Linux，而你要么在抵制，要么很兴奋，“哦耶，让它们进来吧”？

**答：** 我不认为我们有任何其他语言。我的意思是，另一件与 Rust 有点类似、并且花了很长时间的事情——花了十多年才让 Clang 编译内核——那就是 LLVM。我甚至不记得整个 LLVM/Linux 项目是什么时候开始的，但已经是很久以前了。我个人曾经感到非常沮丧，因为拥有两个不同的编译器实际上是我非常想要的东西，但这比我希望的时间长得多。

但现在，在过去几年里，我们在内核社区中已经让 GCC 和 Clang 相当广泛地共存了。所以你有像谷歌这样的大公司，我认为 Android 现在几乎完全是用 Clang 编译的，并且已经有一段时间了。所以你有大公司在使用 Clang，尽管 GCC 显然仍然是传统的编译器。它们之间存在差异，我们确实有类似 `ifdef clang` 这样的代码，但它们相当少，而且在过去一年左右并没有成为大问题。不是说没有，我最近就看到一个补丁里有 `ifdef clang` vs GCC，但这只是另一个影响较小的项目，不像 Rust 那样。但它花了很长时间，惊人地长。

这就是为什么我认为，好吧，我们才为 Rust 这事工作了几年（之前也有一些努力），但它离准备就绪还差得远呢，这根本不让我担心，因为我见过其他侵入性小得多的项目都花了一二十年甚至更长时间。所以我没看到任何其他巨大的推动力。人们会提到其他语言，但目前看来都不太可能。

**问：** 你早些时候也提到过“我们从不破坏用户空间”（never break user space）。你的这个理念随着时间的推移有所改变吗？因为……

**答：** 没有，我的意思是，我们仍然有一条非常严格的规则，即我们从不破坏用户空间。但同时，“从不”（never）是那种黑白分明的词，有时现实会介入并给你带来麻烦。所以我们最终确实会……比如，如果出现重大的安全问题——虽然最近没有发生过——但我们遇到过这样的情况，我们不得不说必须做出这个改变，因为我们旧的行为不仅仅是 buggy，而是以一种我们无法接受的方式 buggy，它是一个安全隐患。

还有，在某个时候，比如我们已经到了无法合理维护某些旧架构的地步。很久以前我们停止了对原始 386 的支持，仅仅因为维护负担相对于其带来的价值来说太高了。所以，从某种意义上说，那确实是破坏了用户空间，因为如果你当时有一台基于 386 的机器，而内核说我们不能再支持它了，显然我们破坏了那种情况。所以我的意思是，你总是需要在“好吧，够了，我们不能再支持那个了”之间找到某种平衡。但总的来说，我们仍然坚持：你不能在添加新功能或试图修复一个 bug 时破坏其他东西，那不是 bug 修复，那需要用其他方式来完成。

## 九、 安全性视角

**问：** 既然你提到了安全，我也有点好奇，这些年来安全是如何变化的。过去这可能是别人的问题，现在有很多文化转变，比如 DevSecOps 和整个“左移”（shift left）运动。你对安全有何看法？不仅仅是针对内核，因为你们修复了东西，但它们可能没有被下游打补丁或应用。或者像你过去说的，Heartbleed 事件发生时，你那句名言“Bug 是软件开发过程的一部分”，我现在还经常引用。你如何看待内核领域的安全？

**答：** 我的意思是，安全总是重要的。但一直以来的一个问题是，伴随某些安全问题而来的保密性（secrecy）是一个巨大的痛苦。我的意思是，它从根本上与开源开发模式不兼容。所以，对我来说，安全方面的大问题往往出在安全公司和相关人员身上，当他们想要 90 天的禁运期（embargo），尤其是涉及到过去五年多我们遇到的硬件安全问题时，有些禁运期不是 90 天，而是一年半，硬件公司说他们无法修复这个问题，也不想让任何人知道，所以你不能谈论它，你不能在明年年底之前发布修复补丁。这一直是一个巨大的痛苦。

我对此进行了相当强硬的反击。我说，嘿，安全漏洞就是 Bug。而另一方面是，几乎任何 Bug 都可能成为安全漏洞。我的意思是，有些 Bug 非常简单，很难被滥用，但我们经常修复一些愚蠢的小 Bug，当时甚至没人意识到，直到一两年后才发现那个愚蠢的小 Bug 可以被滥用，而那个微不足道的修复后来成了一个巨大的安全修复。然后你就得回去把你当初认为不那么重要的东西向后移植（backport）到更旧的内核中去。

所以安全可能很痛苦，但就我而言，从开发的角度来看，我正努力确保我们将它们视为重要的、但仍然是常规的 Bug 来尽可能地处理。

## 十、 对新兴技术与趋势的看法

**问：** 现在我们来谈谈一些正在发生的普遍趋势，我想听听你的看法。其中一个，你知道的，现在最热门的话题是生成式人工智能（GenAI）。你怎么看？当然，你们所有东西都在邮件列表上，所以这甚至不是关于是否拥抱这些技术的问题，而是你对这些正在发生的现代技术有什么看法？具体点说，比如 GenAI。

**答：** 是的，我猜你指的就是这个。你知道吗，我认为人工智能（AI）真的很有趣，我认为它将改变世界。但同时，我非常讨厌炒作周期（hype cycle），以至于我真的不想去掺和。所以我现在对 AI 的态度基本上是忽略它，因为我认为围绕 AI 的整个科技产业处于一个非常糟糕的状态，90% 是市场营销，10% 是现实。

五年后情况会改变，到那时我们再看哪些 AI 被真正用于日常的实际工作负载，而不仅仅是像 ChatGPT 那样做出精彩的演示。它显然在很多领域被使用，尤其是在……我的意思是，很多领域，比如图形设计等等。但我真的讨厌这个炒作周期。这不仅仅是 AI 的问题，我认为这是一个行业问题。我的意思是，在 AI 之前的几年，人们唯一谈论的就是加密货币（Crypto）。我只是……我不喜欢炒作周期。

部分原因在于，我从根本上是那种人：我发现一些有趣的事情，然后我会坚持下去。这就是为什么 30 年后我还在做内核。然后我发现那些像社交蝴蝶一样的人，从一个问题飞到另一个问题，谈论今天什么酷，而不是十年来什么酷，我只是……那不是我的风格。

**问：** 即使我作为一名作家，我也会用它来做一些底层的工作，但你必须在此基础上创造价值。但你绝对是对的，炒作是问题所在，而不是技术本身。那么如果我换个问法，有哪些现代技术让你感到兴奋？你觉得“嘿，这东西真有趣”，甚至吸引了你的注意？

**答：** 我不知道。我过去常说，我认为如果你真的想做一些有趣的事情，你根本不应该待在 IT 行业，你应该去比如生物科学之类的领域。但我这是十多年前说的了，现在看来那个领域似乎也没那么有趣了。所以我认为，并不是说有一个唯一的有趣领域，而是对你来说什么是有趣的。对我来说，仍然是内核。我一直……并非内核本身，我一直对硬件和软件之间的那个领域感兴趣，这就是为什么我做内核，但我也喜欢编译器，这一直是我的兴趣所在。

但这只是我的兴趣，对其他人来说不应该、也不重要。我认为新技术也是如此，并不是说有这么一个所有人都应该为之兴奋的新技术。这实际上又回到了我对 AI 感到恼火的地方，人们应该努力找到他们感兴趣的东西，然后新技术可以成为让它变得有趣的东西。

举个例子，回想起来，我认为树莓派（Raspberry Pi）很棒，不是因为树莓派硬件本身有多么有趣，而是因为它让这些微控制器硬件变得如此广泛可用。通过使其广泛可用，你找到了全新的受众，他们可以做新的事情。并不是说树莓派本身是革命性的，但我认为它推动了整个……人们仍然在玩可穿戴计算，做这些随机的小项目，我认为这很棒。这让人们找到了不是那个唯一的新事物，而是对他们来说重要的事物。所以，我不知道对我来说地平线上有什么新的东西，因为我仍然对那个硬件和软件领域感兴趣。

**问：** 我的意思是，我几周前刚从 Microcenter 买到了第五代树莓派 5，因为它总是缺货，你永远找不到。我有几十个树莓派。但是，我的意思是，RPi 5 现在相当贵，大概 100 美元，以前是 35 美元。

**答：** 我认为在某种程度上，树莓派开启了廉价硬件的潮流，但现在有很多其他小型廉价硬件可以用于你自己的嵌入式项目。所以现在树莓派显然已经……它们正试图走向稍微高端一点的市场，这对那些想要更像真正计算机的人来说是好事。但我认为你会发现很多对初代 RPi 感到兴奋的人现在正在使用这些新的、随机的小型嵌入式平台，比如……是的，我们想要一些非常小、非常小的东西，可以塞进任何小盒子里，这就是我做很多项目的原因。

**问：** 你对电动汽车（EVs）有什么看法？因为电动汽车主要是软件，我的意思是，就像带轮子的电脑。驾驶部分是次要的，更多的是……你对自动驾驶电动汽车或其他有什么想法吗？这让你兴奋吗？

**答：** 我喜欢电动汽车，我们已经把大部分车都换成了电动车。我们现在的主要用车是一辆沃尔沃全电动汽车。我喜欢它们是因为我不喜欢内燃机。低转速时的即时扭矩对我来说让驾驶更有趣。我对整个自动驾驶并不那么感兴趣。我的意思是，我们有一辆开了 20 年的老车，换成了一辆现代电动汽车，我喜欢它能实现车道保持和所有我们老车没有的基础功能，但同时，是的，这在宏伟蓝图中只是一个小细节。

但同时，人们认为电动汽车是“带轮子的电子产品”的原因是，电动机本身比内燃机简单得多。如果你要制造传统的内燃机，你需要有几十年的内燃机历史才能制造出好的发动机。而从今天的电动汽车市场你可以看到，嘿，你不需要几十年的经验就能制造出好的电动机，因为它们简单得多。我的意思是，传统发动机和电动机的运动部件数量大概相差两个数量级。

**问：** 我更喜欢电动汽车的地方，正如你所说，不是自动驾驶，而是所有新功能都是软件驱动的，所以你可以修复、打补丁。你的沃尔沃运行的是你自己的内核吗？还是仍然运行沃尔沃的操作系统？你有没有尝试过改装它？或者你不碰它？

**答：** 我很确定它里面运行的是 Linux，但我不碰它。是的，它有……

**问：** 对你来说它就像个电器？

**答：** 是的，对我来说它绝对是个电器。我不是一个汽车爱好者（car person），尽管我这么说，但我确实有过一辆跑车开了 20 年，那是一辆小型的双座敞篷车，我真的很喜欢开。但即便如此，我也从未真正成为一个汽车爱好者。所以汽车对我来说只是……

**问：** 便利。

**答：** 是的，是的。我喜欢它方便、舒适，但除此之外我不太在乎。这也是我最终处理掉我的运动敞篷车的原因之一，我决定，嘿，电动汽车的优点之一就是这种平稳的加速，以及不需要换挡，这对我来说让汽车好开得多。而很多严肃的汽车爱好者，他们讨厌这部分，他们想要 V8 发动机的轰鸣声，他们想要……

**问：** 我开野马（Mustang），所以我能理解，他们喜欢手动换挡之类的……

**答：** 我学开车就是那样学的。不，手动挡并不好，我宁愿完全没有档位。所以，是的，我不是一个严肃的汽车爱好者。

## 十一、 个人生活与爱好

**问：** 你有什么新培养的爱好吗？

**答：** 没有，我还是……我从来没有很多爱好。我的主要爱好是阅读。水肺潜水（Scuba diving）仍然是……当我旅行时，我尽量去潜水，这次旅行不太行，但是……我们几周后有家庭度假，要去夏威夷，我打算去潜水。

**问：** 你都读些什么类型的书？

**答：** 垃圾读物。哦，绝对是恶心的垃圾读物。我过去常常读硬科幻，像传统的阿西莫夫、海因莱因那种。我的意思是……我买了个 Kindle，我们家以前书架上堆满了书，占了很多空间。很多年前我买了 Kindle，然后发现我真正喜欢做的是买那些非常便宜的、完全可以被遗忘的书。我阅读不是为了获取信息或成为一个更好的人，我阅读是为了消遣。所以这些天我随便读读奇幻小说，仍然读科幻小说，完全没什么严肃的内容。

## 十二、 结束语

**问：** 还有其他你想谈论的吗？或者你觉得我们……

**答：** 不，我没有什么信息要传达。我的意思是，我以前也说过，我不会试图把我的世界观强加给别人。我认为……我认为开源很有趣，但同时，我从来不是那些认为所有人都应该这样做的自由软件人士之一。这是我想做的事情，但我没有信息要传达，我没有什么想告诉别人去做或者告诉别人关于我自己的事情。

**主持人 (BH):** 非常棒，你知道，能坐下来聊聊，既能重温记忆，也能回顾过往。非常感谢你。你知道，像往常一样，只要你有兴趣，我很乐意再次与你交谈。但我非常感谢你这次。

**Linus Torvalds:** 几年后在某个会议上再聊吧，如果那时又有什么新鲜事发生的话。

*[音乐]*

---

# 要点回顾

好的，这是从视频脚本中提取的框架与要点内容：

**一、 Linus Torvalds 的近况与角色**
- Linus 目前主要工作是代码合并（Merging），尤其是在合并窗口期间。
- 他很少进行实际的开发编码工作，这在过去十年中已成为常态。
- 他的角色更像是连接点和“坏人”，负责审查并拒绝不合适的代码提交。
- 他认为内核开发过程整体上相当顺利，技术问题总能找到解决方案。

**二、 Linux 内核与生态发展**
- Linus 个人不太关心 Linux 的市场份额或具体被哪些大公司使用。
- 他关注广泛使用，因为使用能发现 Bug 和新的有趣用例，从而推动开发。
- 早期贡献者更多是个人，解决个人需求；现在更多来自有特定需求的大公司/站点，开发更专业化。
- 对比早期“狂野西部”时代，现在更稳定但也少了些疯狂和乐趣。Linus 喜欢现在的稳定，但也怀念过去的无拘无束。
- 认为当前的开发流程比过去好得多，虽然失去了一些兴奋感和个性，但这是发展所必需的。

**三、 内核社区健康与挑战**
- 社区规模巨大变化：从几十核心开发者/几百参与者，发展到几百核心开发者/几千参与者。
- 规模扩大导致个人认识减少，必须依赖层级结构和信任链（信任维护者，维护者再信任他们团队的人）。
- Linus 主要依赖他熟悉的 Top 50-100 位维护者。
- 社区形状良好，但开发者数量多于维护者，部分维护者可能工作负担过重。
- 希望有更多维护者来分担工作量、压力和责任，但维护者工作压力大，不总是“有趣”的工作。
- 成为内核维护者仍具吸引力：技术挑战有趣，且有助于职业发展（容易找到工作）。
- 担忧某些子系统过于依赖单一维护者或存在高度专业化知识集中在少数人手中的风险。

**四、 Linux 的应用边界与开源理念**
- Linus 感觉 Linux 在微控制器（Microcontroller）领域表现不如预期，更小的内核（如 Zephyr）可能更适合。
- 接受 Linux 不会无处不在，对于极小设备，小型操作系统更合适；但设备常会“长大”并最终需要 Linux。
- 认为基础架构（如操作系统）领域，开源是唯一途径，没有商业价值去开发定制的、封闭的小型操作系统。
- 对于只使用不贡献的“搭便车”者（Leeches），Linus 并不十分在意，认为这是他们的选择，代价是无法影响项目发展方向。
- 承认存在不良行为，但认为法律手段是极端情况，并不普遍担忧。

**五、 工作方式与沟通偏好**
- Linus 主要通过电子邮件进行工作沟通，极度厌恶 Zoom 等同步会议或电话。
- 异步的邮件模式适合跨时区协作，且不会打断他的工作流（Flow）。
- 他承认自己不是“people person”，更喜欢在技术层面交流。
- 现在与新开发者的直接互动减少，主要与维护者打交道。
- 偶尔会回复有趣的、他认为自己是权威能解答的邮件（包括来自学生的提问），但会忽略大量普通邮件。

**六、 技术项目与工具**
- Linus 创建的其他项目（如 Git、Subsurface）都是因为当时没有满足他需求的工具。
- Git 是为了解决他自身工作流的问题而创建的。
- Subsurface 是 C++ 编写的（虽然他不喜欢 C++），满足了他的潜水日志需求。
- 目前感觉自己的需求基本都被满足了，未预见需要创建新项目。

**七、 Linux 桌面与硬件趋势**
- 对 Linus 而言，过去近三十年一直都是“Linux 桌面年”，因为它满足了他的需求。
- Web 的普及极大改变了桌面生态，很多应用变成了网页，降低了对特定操作系统应用的依赖（如 Windows 应用）。
- Chromebook 等设备体现了浏览器为中心的趋势。
- Steam Deck 等设备拓展了 Linux 在游戏领域的应用。
- WSL 使 Windows 用户能方便使用 Linux。
- 硬件趋势：ARM 架构的崛起（包括 Apple 的 M 系列芯片），多架构支持对 Linux 是好事，软件行业越来越少单一 OS + 单一架构的模式。

**八、 内核中的编程语言与兼容性**
- Linus 本质上仍是 C 语言开发者。
- 对 Rust 的态度：不讨厌，认为它有趣，可能带来新想法和新人；但他个人不会大量使用，目前阅读 Rust 代码还需思考。
- 社区对 Rust 的态度不一，有人积极，有人反对。
- C++：Linus 不喜欢 C++ 的设计决策，但 Subsurface 项目使用了它。
- Clang/LLVM：支持 Clang 编译内核花费了很长时间（超十年），他对此曾感到沮丧，但现在 GCC 和 Clang 已能较好共存，有大公司（如 Android）使用 Clang 编译内核。
- “永不破坏用户空间”原则：仍然是非常重要的硬性规定，但存在例外（如严重安全问题、无法维护的旧架构支持，如放弃 386 支持）。

**九、 安全性视角**
- 安全很重要，但围绕安全问题的保密性（Secrecy）与开源开发模式冲突，是一大痛点。
- 对长达数月甚至一年半的硬件安全漏洞禁运期（Embargo）非常不满，并强烈反对。
- 主张将安全 Bug 视为普通 Bug 处理，因为任何 Bug 都可能被利用成为安全漏洞。
- 很多时候修复小 Bug 事后才发现是重大安全修复。

**十、 对新兴技术与趋势的看法**
- AI / GenAI：认为 AI 很有趣并将改变世界，但极度厌恶当前的炒作周期（Hype Cycle），选择暂时忽略，认为目前 90% 是市场营销。等待 5 年后看实际应用。
- 不喜欢技术领域的“社交蝴蝶”现象，倾向于长期专注于自己感兴趣的领域（如内核三十年）。
- Crypto：同样不喜欢之前的炒作周期。
- 真正令人兴奋的技术：对他而言，始终是软硬件接口领域（内核、编译器等）。
- 认为个体应寻找自己真正感兴趣的技术，而非追逐“热点”。
- Raspberry Pi：赞赏其普及了廉价硬件，激发了新的受众和项目，虽然硬件本身不一定革命性。
- 电动汽车 (EVs)：喜欢电动汽车（拥有 Volvo EV），因其低转速即时扭矩和驾驶乐趣，且不喜欢内燃机。对自动驾驶兴趣不大，更看重基础的辅助驾驶功能。认为电动汽车的电子化是因为电动机比内燃机简单得多。

**十一、 个人生活与爱好**
- 主要爱好是阅读和水肺潜水（Scuba Diving）。
- 阅读：读很多“垃圾读物”（科幻、奇幻），目的是消遣而非提升自我。偏爱 Kindle 上的廉价、易忘的书籍。
- 不是“汽车爱好者”，车对他主要是交通工具。

**十二、 结束语**
- Linus 表示自己没有特别的“信息”要传达给他人。
- 他认为开源很有趣，是他个人的选择，但并非要求所有人都必须这样做。