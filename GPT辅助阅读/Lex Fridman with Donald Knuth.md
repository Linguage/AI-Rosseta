
# Lex Fridman X Donald Knuth 

```
这篇访谈稿的整理比预期的困难很多。

我的处理流程如下：
1. 在YouTube上将视频生成的英文访谈文本拷贝出来。
2. 通过听视频将访谈稿进行必要的分割，主要为了区别提问者和回答者。但此部分并不容易，因为提问者经常插话，增加了不少零碎的内容。
3. 使用GPT将区分问答之后的文稿分部补充标点符号，从而获得可读性；
4. 使用GPT将英文稿翻译为汉语
5. 完成翻译工作之后，对全文稿进行精修。


```

## Introduction


The following is a conversation with Donald Knuth, one of the greatest and most impactful computer scientists and mathematicians ever. He's the recipient of the 1974 Turing award, considered the Nobel Prize of computing. He's the author of the multi-volume work, the magnum opus, "The Art of Computer Programming."

He made several key contributions to the rigorous analysis of computational complexity of algorithms, including the popularization of asymptotic notation that we all affectionately know as the Big O notation. He also created the TeX typesetting system, which most computer scientists, physicists, mathematicians, and scientists and engineers in general used to write technical papers and make them look beautiful.

I can imagine no better guest to have in 2019 than Don, one of the kindest, most brilliant people in our field. This podcast was recorded many months ago. It's one I avoided because perhaps counter-intuitively, the conversation meant so much to me. If you can believe it, I knew even less about recording back then, so the camera angle is a bit off. I hope that's okay with you.

The office space was a bit cramped for filming, but it was a magical space where Don does most of his work. It meant a lot to me that he would welcome me into his home. It was quite a journey to get there. As many people know, he doesn't check email, so I had to get creative. The effort was worth it. I've been doing this podcast on the side for just over a year. Sometimes I had to sacrifice a bit of sleep, but always happy to do it and to be part of an amazing community of curious minds. Thank you for your kind words, support, for the interesting discussions, and I look forward to many more of those in 2020.

This is the Artificial Intelligence Podcast. If you enjoy it, subscribe on YouTube, give it five stars on Apple Podcasts, follow on Spotify, support on Patreon, or simply connect with me on Twitter at Lex Friedman, spelled F-R-I-D-M-A-N.

I recently started doing ads at the end of the introduction. I'll do one or two minutes after introducing the episode, and never any ads in the middle that break the flow of the conversation. I hope that works for you and doesn't hurt the listening experience. I provide timestamps for the start of the conversation that you can skip to, but it helps if you listen to the ad and support this podcast by trying out the product or service being advertised.

This show is presented by Cash App, the number one finance app in the App Store. I personally use Cash App to send money to friends, but you can also use it to buy, sell, and deposit Bitcoin in just seconds. Cash App also has a new investing feature. You can buy a fraction of a stock, say $1 worth, no matter what the stock price is. Brokerage services are provided by Cash App Investing, a subsidiary of Square and member SIPC.

I'm excited to be working with Cash App to support one of my favorite organizations called FIRST, best known for their FIRST Robotics and Lego competitions. They educate and inspire hundreds of thousands of students in over 110 countries and have a perfect rating on Charity Navigator, which means that donated money is used to maximum effectiveness. When you get Cash App from the App Store or Google Play and use code "LexPodcast," you'll get $10 in Cash App, and Cash App will also donate $10 to FIRST, which again is an organization that I've personally seen inspire girls and boys to dream of engineering a better world.

And now, here's my conversation with Donald Knuth.

以下是与Donald Knuth的对话，他是有史以来最伟大和最有影响力的计算机科学家和数学家之一。他是1974年图灵奖的获得者，被认为是计算机界的诺贝尔奖。他是多卷著作《计算机编程的艺术》的作者。

他在算法的计算复杂性的严格分析方面做出了几项重要贡献，包括普及我们大家亲切称之为大O符号的渐近符号。他还创建了TeX排版系统，这是大多数计算机科学家、物理学家、数学家以及一般科学家和工程师用来编写技术论文并使其看起来漂亮的工具。

我无法想象比Don更好的2019年嘉宾，他是我们领域中最善良、最聪明的人之一。这个播客是很久以前录制的，我一直回避它，因为或许有些出乎意料，这次对话对我来说意义重大。如果你能相信，当时我对录音了解得更少，所以摄像机角度有点不对。希望你能接受。

办公空间有点拥挤，但对于拍摄来说却是一个神奇的地方，Don在那里完成大部分工作。他能够欢迎我进入他的家对我来说意义非凡。要到那里真的是一次不小的旅程，正如许多人所知，他不查看电子邮件，所以我必须有所创意。付出的努力是值得的。我已经在做这个播客超过一年了，有时候我不得不牺牲一点睡眠，但总是乐于为之，并成为一个充满好奇心的社区的一部分。感谢你的好评和支持，感谢有趣的讨论，我期待在2020年有更多这样的时刻。

这是《人工智能播客》。如果你喜欢它，请在YouTube上订阅，在Apple Podcasts上给予五星评价，关注Spotify，在Patreon上提供支持，或者简单地在Twitter上与我联系，用户名是Lex Friedman，拼写为F-R-I-D-M-A-N。

我最近开始在引言的结尾做广告。在介绍完一两分钟后，我会播放一两分钟的广告，而不会在对话中间插入任何打破流程的广告。希望这对你有用，不会影响听觉体验。我提供对话开始的时间戳，你可以跳过去，但如果你听广告并尝试广告中宣传的产品或服务，这对支持这个播客很有帮助。

这个节目由Cash App赞助，是App Store中排名第一的金融应用。我个人使用Cash App向朋友发送钱，但你也可以用它在几秒钟内购买、出售和存入比特币。Cash App还推出了一项新的投资功能，你可以购买一小部分股票，比如价值1美元，无论股价如何。经纪服务由Cash App Investing提供，是Square的子公司，是SIPC的成员。

我很高兴能够与Cash App合作，支持我最喜欢的组织之一，称为FIRST，以其FIRST机器人和乐高比赛而闻名。他们在110多个国家教育和激发数十万学生，并在慈善导航上获得了满分，这意味着捐赠的资金被最大程度地有效利用。当你从App Store或Google Play获取Cash App并使用代码“LexPodcast”时，你将获得10美元的Cash App，并且Cash App还将捐赠10美元给FIRST，这是一个我亲自看到激发女孩和男孩梦想工程更美好世界的组织。

现在，让我们开始与Donald Knuth的对话。

## Donald Knuth Interview

Questioner:In 1957 at Case Tech, you were once allowed to spend several evenings with an IBM 650 computer, as you've talked about in the past. Then you fell in love with computing. Can you take me back to that moment with the IBM 650? What was it that grabbed you about that computer?

Answerer: The IBM 650 was this machine that, well, it didn't fill a room, but it was big and noisy. When I first saw it through a window, there were just a lot of lights flashing on it. I was a freshman, and I had a job with the statistics group. I was supposed to punch cards and pour data, then sort them on another machine. But then they got this new computer, and I had a key to the building, so I could get in and look at it. I got a manual for it, and my first experience was based on the fact that I could punch cards.

Questioner: What was a big thing for you to deal with, considering the IBM 650's size and power?

Answerer: The IBM 650 was big in size but incredibly small in power and memory. It had 2,000 words of memory, and in a word of memory, there were 10 decimal digits plus a sign. To add two numbers together, you could probably expect that it would take, say, three milliseconds, so that's pretty fast. The memory was the constraint; it had 2,000 words of memory, and to read the data for an instruction, you had to wait for the drum to go around, which took five milliseconds.

Questioner: Did you have any random-access memory back then?

Answerer: We had no random-access memory whatsoever until my senior year. We got fifty words of random access memory, which were priceless. We would move stuff up to the random access memory in 60-word chunks, and then we would start again.

提问者：在1957年，你曾经有机会在Case Tech度过几个晚上与IBM 650计算机为伍，正如你之前所说的。后来你爱上了计算机。你能带我回到与IBM 650的那个时刻吗？是什么让你对那台计算机着迷？

回答者： IBM 650是一台机器，嗯，它并没有填满整个房间，但它很大且嘈杂。当我第一次通过窗户看到它时，上面有许多闪烁的灯光。我当时是一名大一新生，加入了统计小组的工作。我本应该打孔卡片、输入数据，然后在另一台机器上对它们进行排序。但后来他们引进了这台新计算机，而我有大楼的钥匙，所以我可以进去看看。我找到了它的手册，我的第一次经验基于我可以打孔卡片这个事实。

提问者： 对于你来说，考虑到IBM 650的大小和性能，那是一个很大的挑战吗？

回答者： IBM 650在体积上很大，但在性能和内存方面却非常有限。它有2,000个字的内存，每个字的内存包括10个十进制数字和一个符号。要将两个数字相加，你可能期望需要大约三毫秒，所以速度相当快。但内存是限制因素；它只有2,000个字的内存，要读取指令的数据，你必须等待滚筒转动，这需要五毫秒。

提问者： 那个时候你有随机存取内存吗？

回答者： 直到我大四的时候，我们根本没有随机存取内存。那时我们得到了50个字的随机存取内存，这是无价的。我们会将数据以60个字的块移至随机存取内存，然后重新开始。




## Predicting the Future

Questioner: So, it's separating when to go up there, and could you have predicted the future 60 years later of computing from then?

Answerer: You know, in fact, the hardest question I was ever asked was, "What could I have predicted?" In other words, the interviewer asked me. She said, "You know what about computing has surprised you?" Immediately, I rattled off a couple dozen things. Then she asked, "Okay, so what didn't surprise?" I tried for five minutes to think of something that I thought I would have predicted, and I couldn't. But let me say that this machine, I didn't know. Well, there wasn't much else in the world at that time. The 650 was the first machine that there were more than a thousand of. Ever before that, there might be a half a dozen examples, maybe my first mass-market, mass-produced, the first one, yeah, done in quantity. IBM didn't sell them; they rented them. But they rented them to universities at a great deal, and that's why a lot of students learned about computers at that time.

Questioner: You refer to people, including yourself, who gravitate toward a kind of computational thinking as geeks. For at least, I've heard you used that terminology. Is it true that you think there's something that happened to me as I was growing up that made my brain structure in a certain way that resonates with computers? So, there's the space of people, it's 2% of the population. You empirically estimate that's a prick; it's been proven fairly constant over most of my career. However, it might be different now because kids have different experiences when they're young. So, what does the world look like to a geek? What is this aspect of thinking that is unique to their makes it, yeah, that makes a geek? This is cuter.

Answerer: The important question in the 50s IBM noticed that there were geeks and non-geeks. So, they tried to hire geeks and put out ads or papers saying, "If you play chess, come to Madison Avenue for an interview," or something like this. They were trying for something. What is it that I find easy, and other people tend to find harder? I think there are two main things. One is this ability to jump levels of abstraction. So, you see something in the large, and you see something in the small, and can you pass between those unconsciously? In order to solve some big problem, what you need to do is add one to a certain register or anything that gets you to another step, and you can go below the, yeah. I mean, I don't go down to the electron level, but I knew what those milliseconds were, what the drum was like on the 650, I knew how I was going to factor a number or find a root of an equation or something because of what was doing. As I'm debugging, I'm going through, did I make a key punch error, did I write the wrong instruction, do I have the wrong thing in a register, and each level is different. So, this idea of being able to see something at lots of levels and fluently go between them seems to be more pronounced, much more pronounced in the people that work with computers. I got so, in my books, I also don't stick after the high level, but I mix low-level stuff with high level, and this means that some people think, you know, that I should write better books, and it's probably true. But other people say, well, but that's if you think like that, then that's the way to train yourself, like to keep mixing the levels and learn more and more how to jump between. So, that's one thing. The other thing is that it's more of a talent to be able to deal with non-uniformity where there's case one, case two, case three, instead of having one or two rules that govern everything. So, it doesn't bother me if I need like an algorithm has ten steps to it; each step is does something else. That doesn't bother me. But a lot of pure mathematics is based on one or two rules which are universal. This means that people like me sometimes work with systems that are more complicated than necessary because it doesn't bother us that we didn't figure out the simple rule.

Questioner: And you mentioned that while Jacobi, Boule, Abel, and all the mathematicians in the 19th century may have had symptoms of geek, the first 100% legit geek was Turing, Alan Turing. I think he had a lot more of this quality than anyone could from reading the kind of stuff he didn't show as hot as Turing. What influence has Turing had on you?

Answerer: Well, your way, and so I didn't know that aspect of him until after I graduated, some years later, as an undergraduate, we had a class that talked about computability theory and Turing machines. That sounded like a very specific, purely theoretical approach to stuff. So, when, how old was I when I learned that he thought he had designed when she and that he wrote the, you know, he wrote a wonderful manual for Manchester machines, and he invented all the subroutines. He was a real hacker that he had his hands dirty. I thought for many years that he had only done purely formal work. As I started reading his own publications, I could feel this kinship. And of course, he had a lot of peculiarities. Like he wrote numbers backward because from left to right, to the right to left, because that's the easier for computers to process him that way. What do you mean left to right? He would write PI as, you know, 9 5 1 4.3. I mean, okay, right, forget it, for one point three on the blackboard, I mean when he, he had trained himself to do that because the computers he was working with worked that way inside, trained himself to think like a computer. Well, there you go, that's nuts, geek thinking.

提问者： 所以，这是分离何时上升的一个方面，你当时能预测到60年后的计算机世界吗？

回答者： 你知道，事实上，我被问过的最难的问题是，我能预测什么，换句话说，面试官问我，她说，你知道计算机的哪些方面让你感到惊讶。我立刻列举了几十个事物。然后她问，那么有什么不让你感到惊讶的呢？我试了五分钟，试图想出我认为我可能会预测到的事情，但我不能。但让我说一下，这台机器，我并不了解，因为那时世界上没有太多其他东西。650是第一台有超过一千台的机器，之前从来没有超过一千台的，每台机器可能只有半打例子，也许是我第一次量产的，IBM没有卖给他们，他们是租给大学的，而且租金很便宜，所以那个时候很多学生学到了计算机。

提问者： 你提到那些倾向于一种计算思维的人，包括你自己，被称为“geeks”，至少我听过你用过这个术语。你认为那是真的吗？我认为有些事情发生在我成长过程中，使我的大脑结构以某种方式共鸣于计算机。这是一个人群，占人口的2%，你根据经验估计这是一个固定的比例，大部分我的职业生涯都是如此。然而，现在可能会有所不同，因为孩子们在年轻时有不同的经历。那么，对于一个geek来说，这个世界是什么样的？是什么独特的思维方式让他们成为geek？

回答者： 这是一个重要的问题。在50年代，IBM注意到有geeks和非geeks，于是他们试图雇佣geeks，并发布了一些文件，表示如果你擅长下棋，就来Madison Avenue面试之类的。他们试图找寻一些东西。那么我所发现容易而其他人往往发现困难的是两件主要的事情。一是能够跳跃抽象的层次，你在大的方面看到一些东西，你在小的方面看到一些东西，你能够在它们之间毫不费力地切换。你知道为了解决一个大问题，你需要在某个寄存器中加一，或者做一些将你带到下一步的事情。我们在调试时经常经历这个过程，每个层次都不同。所以这种能够在许多层次上看到东西并且流畅地在它们之间切换的能力，我觉得在与计算机有关的人中更为突出，更为显著。在我的书中，我也不仅限于高层次的内容，我将低层次的东西与高层次的内容混合在一起，这意味着一些人认为我应该写得更好，这可能是真的，但其他人说，那是一种培养自己的方式，保持混合层次，学会更多地跳转，所以这是其中一件事。另一方面，更多的是一种才能，能够处理非均匀性，存在案例一、案例二、案例三，而不是有一两个规则支配一切。所以如果一个算法有十个步骤，每个步骤都做一些不同的事情，对我来说没问题，但很多纯数学是基于一两个普遍的规则，这意味着像我这样的人有时候会处理比必要更复杂的系统，因为我们不在乎我们没有找到简单规则，这并不影响我们。你提到雅可比、布尔、阿贝尔以及19世纪所有的数学家可能都有geek的症状，但第一个百分之百合法的geek是图灵，艾伦·图灵。我认为他拥有比任何人都更多的这种品质。

提问者： 图灵对你有什么影响？

回答者： 直到我毕业几年后，我才知道他的这一方面。在我本科时，我们有一门课讲授可计算性理论、图灵机等等，那时一切听起来都是一种非常特定的纯理论方法。所以我是多大的时候，我才了解到他认为他设计了机器，并且他写了一份出色的手册给曼彻斯特机器，他发明了所有的子程序。他是一个真正的黑客，他的手很脏。多年来，我一直以为他只做了纯粹的形式工作，当我开始阅读他的出版物时，我能感到这种亲切感。当然，他有很多奇怪之处，比如他倒写数字，因为从左到右或者从右到左对计算机来说更容易处理。从左到右，他会写PI为9 5 1 4.3。我是说好吧，算了吧，为了黑板上的1.3，他训练自己那样做，因为他使用的计算机也是这样处理的，他训练自己像一台计算机一样思考。嗯，这就是疯狂的geek思维。

## literate programming

Questioner: You've practiced some of the most elegant formalism in computer science, and yet you're the creator of a concept like literate programming, which seems to move closer to a natural language type of description of programming. How do you see those two as conflicting, the formalism of theory and the idea of literate programming?

Answerer: So there we are in a non-uniform system. Well, I don't think one size fits all, and I don't think all truth lies in one kind of expertise. Somehow, in a way, you'd say my life is a convex combination of English and mathematics, and you're okay with that. And not only that, I think thriving. I wish, you know, I want my kids to be that way. I want to, not use left-brain right-brain at the same time. You get a lot more done; that was part of the...

Questioner: And I've heard that you didn't really read for pleasure until into your 30s, literature. True, you know more about me than I do, but I'll try to be consistent with what you're really, ya know, just believe me. Yeah, just go with whatever story I tell you; it'll be easier that way. The conversation I've heard mentioned a literary influence, Philip Roth's American Pastoral, which I love as a book. I don't know if it was mentioned as something, I think that was meaningful to you as well. In either case, what literary books had a lasting impact on you?

Answerer: Okay, good. So I met Roth already; we both got doctors from Harvard on the same day. So we had lunch together and stuff like that. But he knew that, you know, computer books would never sell. Well, all right, so you say you're a teenager when you left Russia. So I have to say that Tolstoy was one of the big influences on me. I especially like Anna Karenina, not because of a particular area of the plot or the story, but because there's this character who did the philosophical discussions. It's a whole way of life is worked out there among the characters until in and so that I thought was especially beautiful. On the other hand, Dostoevsky, I didn't like at all because I felt that his genius was mostly because he kept forgetting what he had started out to do, and he was just sloppy. I didn't think that he polished his stuff at all, and I tend to admire somebody who Todd's the i's and crosses the t's so that the music of the prose, this way you admire more. And that I certainly do admire the music of the language, which I couldn't appreciate in the Russian original, but I can. And Victor Hugo, Glenn's close friendships much his closer, but Tolstoy I like for the same reason I like Herman Wouk as a novelist. I think I like his book Marjorie Morningstar, has a similar character who developed his own personal philosophy and export, and it called goes in, is consistent. Yeah, right, and it's worth pondering. So, like Nietzsche and like what you don't like Friedrich Nietzsche or age? Yeah, no, no, you like this has like I keep seeing quotations from Nietzsche, and you never tempt me to read any further. Please, full of contradictions; we will certainly not appreciate him. But Schiller, you know, I'm trying to get the cross, what I appreciate in literature. And part of it is, as you say, the music of the language, the way it flows. Take Raymond Chandler versus Dashiell Hammett. Dashiell Hammett's sentences are awful, and Raymond Chandler's are beautiful; they just flow. So, I don't read literature because it's supposed to be good for me or because somebody said it's great. But I could find things that I like. I mean, you mentioned, you address, like James Bond. So, like, I love Ian Fleming; I think he's got a he had a really great gift for, if he has a golf game or a game of bridge or something, and this comes into a story, it'll be the most exciting golf game or the absolute best possible hands at bridge that exists. And he exploits it and tells it beautifully as well.

Questioner: In connecting some things here, looking at literate programming and being able to convey, encode algorithms to a computer in a way that mimics how humans speak, what do you think about natural language in general and the messiness of our human world about trying to express difficult things?

Answerer: So the idea of literate programming is to try to understand something better by seeing it from these two perspectives, the formal and the informal. If we try to understand a complicated thing, if we can look at it in different ways. So this is, in fact, the key to technical writing. A good technical writer tries not to be obvious about it but says everything twice, formally and informally, or maybe three times. But you try to give the reader a way to put the concept into his own brain or her own brain. Is that better for the writer or the reader or both?

Questioner: Well, the writer just tries to understand the reader. That's the goal of a writer is to have a good mental image of the reader and to say what the reader expects next and to impress the reader with what has impressed the writer, why something is interesting. So when you have a computer program, we try to, instead of looking at it as something that we're just trying to give an instruction to the computer, what we really want to be is giving insight to the person who's going to be maintaining this program or to the programmer himself when he's debugging it, as to why this stuff is being done. So all the techniques of exposition that a teacher uses or book writers make you a better program or if your program is going to be not just a one-shot deal.

提问者： 你在计算机科学中练习了一些最优雅的形式主义，但你也是文学编程这个概念的创造者，这似乎更接近于自然语言类型的编程描述。你如何看待这两者之间的冲突，理论的形式主义和文学编程的思想？

回答者： 那么我们就处于一个非均匀的系统中。嗯，我认为并非一刀切，我也不认为所有的真理都在一种专业中。以某种方式来说，你可以说我的生活是英语和数学的凸组合，而你对此感到满意。不仅如此，我认为我在这样的环境中茁壮成长。我希望，你知道，我希望我的孩子也能这样，我希望同时运用左脑和右脑。你会更有效率，这也是成功的一部分。

提问者： 我听说你直到30多岁才真正开始阅读文学作品，是文学。是的，你了解我比我自己更多，但我会尽量与你说的保持一致。是的，随便相信我说的任何故事吧，这样会更容易。在对话中，我听说提到了文学影响，菲利普·罗斯的《美国牧歌》是其中之一，我也喜欢这本书，我想这对你来说也是有意义的。无论如何，哪些文学作品对你产生了持久的影响？

回答者： 好的。我已经见过罗斯了，我们在同一天都从哈佛大学获得了博士学位。所以我们一起吃过午餐之类的。但他知道计算机书籍永远不会卖得好。好吧，你说你是离开俄罗斯时的十几岁少年。我不得不说，托尔斯泰对我有很大的影响，特别是我喜欢《安娜·卡列尼娜》，不是因为情节或故事的特定区域，而是因为有这么一个角色，他进行了哲学讨论，整个生活方式在那里得到了体现，是在人物之间的。所以我认为那是特别美丽的。另一方面，陀思妥耶夫斯基我一点都不喜欢，因为我觉得他的天赋主要是因为他总是忘记他最初想做什么，而且他太草率了。我认为他根本没有把自己的作品搞得井井有条。我认为值得钦佩的是那些能够把事情做到井井有条的人，他们会对文字的音乐感到钦佩。这种音乐的美，我在俄语原著中无法欣赏，但我能感受到。雨果、格伦斯·克洛斯的友谊更加亲密，但是托尔斯泰以相同的原因让我喜欢上了赫尔曼·沃克。作为小说家，我喜欢他的书《玛乔丽·莫宁斯塔》有一个类似的角色，他发展了自己的个人哲学并坚持，这被称为坚持一致。

提问者： 那么，你对自然语言有什么看法，以及我们人类世界的混乱，试图表达困难的事情？

回答者： 文学编程的理念实际上是为了通过从正式和非正式两个角度看待事物来更好地理解它。如果我们试图理解一个复杂的事物，如果我们可以从不同的角度看待它，这实际上是技术写作的关键。一个好的技术作者会试图不显而易见地这样做，但会正式和非正式地说一切，或者可能是三次。但你会试图为读者提供一种将概念放入他自己大脑或她自己大脑中的方法。这对于作者或读者哪一个更好，或者两者兼而有之？

提问者： 那么作者只是试图理解读者。这是作家的目标，是对读者有一个良好的心理形象，并说出读者下一步的期望，并向读者展示什么让作者感到有趣。所以当你有一个计算机程序时，我们试图的不是将其视为我们只是试图向计算机发出指令的东西，而是真正希望将洞察力传递给将要维护这个程序的人，或者当他调试时，作为程序员本人，为什么要这样做。所以所有教师使用的解释技巧或书写者使你更好的程序，如果你的程序不仅仅是一次性的话。




## Informal vs formal


Questioner: So how difficult is that? Do you see hope for the combination of informal and formal for the programming task?

Responder: I think I'm the wrong person to ask, I guess because I'm a geek. But for a geek, it's easy. I don't know, not everyone might have difficulty writing, and that might be because there's something in their brain structure that makes it hard for them to write, or it might be something just that they haven't had enough practice. I'm not the right one to judge, but I don't think you teach any person any particular skill. I do think that writing is half of my life, so I put it together and let programming. Even when I'm writing a one-shot program, I write it in a literate way because I get it right faster. Though now, does it get compiled automatically or...

Questioner: How difficult is a design, especially in a system where much of the programming is done informally?

Responder: On the technical side, my question was how difficult is to design a system where much of the programming is done informally. Yeah, informally, I think whatever works to make it understandable is good. But then you have to also understand how informal is. You have to know the limitations; you have to connect. So, by putting the formal and informal together, this is where it gets locked into your brain. Now you can say informally, "I'm working on a problem right now, so let's go there." I get that. Can you give me an example of connecting the informal and the formal? Well, it's a little too complicated an example. There's a puzzle that's self-referential, called a Japanese arrow puzzle...

Questioner: Can you give me an example of connecting the informal and the formal?

Responder: Well, it's a little too complicated an example. There's a puzzle that's self-referential, called a Japanese arrow puzzle...

Questioner: That's really interesting. So maybe an extension of that, there has been a resurgence in computer science and machine learning and neural networks, so using data to construct algorithms. It's another way to construct algorithms, really?

Responder: Yes, you can think of it that way. As opposed to natural language to construct algorithms, use data to construct others. So, what's the view of this branch of computer science where data is almost more important than the mechanism of the algorithm? It seems to be suited to a certain kind of non-geek, and would you know which is probably why it's taken off, that it has its own community? That really resonates with that, but it's hard to trust something like that because nobody, even the people who work with it, they have no idea what has been learned...

Questioner:That's a really interesting thought that it makes algorithms more accessible to a different community, a different type of brain. 

Responder:Yep, and that's really interesting because just like literate programming perhaps could make programming more accessible to a certain kind of brain, there are people who think it's just a matter of education, and anybody can learn to be a great programmer, anybody can learn to be a great skier. Yeah, you know, I wish that were true, but I know that there's a lot of things that I've tried to do, and I was well motivated, and I kept trying to build myself up, and I never got past a certain level. I can't, for example, view three-dimensional objects in my head...

Questioner: So let's go to the art of computer programming. In 1962, you set the table of contents for this magnum opus, right?

Responder: Yeah, 

Questioner: it was supposed to be a single book for 12 chapters. Now today, what is it? 57 years later, you're in the middle of volume 4 of 7 and in the middle of going for B 

Responder:is 4 B precisely. 

Questioner: Can I ask you for an impossible task, which is to try to summarize the book so far, maybe by giving a little examples from the sorting and the search in the combinatorial algorithms, if you were to give a summary, a quick elevator summary?

Questioner: Yeah, right, what depending how many floors that are in the building. Yes, the first volume called fundamental algorithms talks about something that you can't do without...

Responder: The stuff you can't do without. I guess that you have to know the basic concepts of what is a program, what is it, what is an algorithm, and it also talks about a low-level machine so you can have some idea what's going on. It has basic concepts of input/output and subroutines, induction, writes mathematical. So the thing that makes my book different from a lot of others is that all that I try to not only present the algorithm but I try to analyze them, which means to quantitatively. I say not only does it work, but it works this fast, okay, and so I need math for them. And then there's the standard way to structure data inside and represent information in the computer so that's all volume 1...Volume 2 talks, it's called semi-numerical algorithms, and here we're writing programs, but we're also dealing with numbers...

Responder: Algorithms deal with any kinds of objects but specific when there's objects or numbers, well then we have certain special paradigms that apply to things that have numbers. So there's like there's arithmetic on numbers, and there's matrices full of numbers, there's random numbers, and there's power series full of numbers. There's different algebraic concepts that have numbers in structured ways, 

Questioner: and the arithmetic in the way a computer would think about arithmetic is a floating point, 

Responder: floating point arithmetic, a high precision arithmetic not only addition, subtraction, multiplication but also comparison of numbers. So then check. Then volume 3 talks about, 

Questioner: I like that one, sort insert sorting, a circle of sorting, 

Responder: right? So here we're not getting necessarily with numbers because you slipped, you saw it, letters and other objects, and searching we're doing all the time. We googled nowadays but I mean we have to find stuff. So again, algorithms that underlie all kinds of applications like you know, none of these volumes is about a particular application, but the applications are examples of why people want to know about sorting, why people want to know about random numbers...So then volume 4 goes into combinatorial. I'll again; this is where we have zillions of things to deal with, and we keep finding cases where one good idea can make something go more than a million times faster. We're dealing with problems that are probably never going to be solved efficiently, but that doesn't mean we give up on them, and we have this chance to have good ideas and go much, much faster on them. So that's combinatorial algorithms, and those are the ones that I'm using. Charting is most fun for you. Well, how many combinatorial algorithms are the ones that I always enjoyed the most because that's when my skill in programming had most payoff...The difference between an obvious algorithm that you think up first thing and an interesting, subtle algorithm that's not so obvious but runs circles around the other one. That's where computer science 3D comes in, and a lot of these combinatorial methods were found first in applications to artificial intelligence or cryptography. And in my case, I just liked them, and it was associated more with puzzles. 


提问者： 那有多难呢？你认为在编程任务中，非正式和正式的结合有希望吗？

回答者： 我想我可能不是问这个问题的合适人选，因为我是一个极客。但对于一个极客来说，这很容易。我不知道，不是每个人都可能有写作困难，这可能是因为他们的大脑结构中有一些东西，使他们难以写作，或者可能只是因为他们没有足够的实践。我不是合适的人来评判，但我不认为你能教授任何人任何特定的技能。我确实认为写作是我生活的一半，所以我把它和编程结合起来。即使当我写一个一次性的程序时，我写它以一种有文化的方式，因为这样我能更快地弄清楚。不过现在它是否被编译是自动的，或者...

提问者： 设计一个系统，在其中大部分编程是非正式完成，这有多难？

回答者： 从技术角度来看，我的问题是设计一个系统，在其中大部分编程是非正式完成，这有多难。是的，非正式地，我认为任何使其可理解的方法都是好的。但是你必须也要了解非正式的程度，你必须知道其限制，你必须连接。通过将公式和非正式结合在一起，这就锁定在你的大脑中。现在你可以说非正式地：“我现在正在解决一个问题，所以让我们去那里。”我明白那一点。

提问者： 你能给我举一个连接非正式和正式的例子吗？

回答者： 嗯，这有点太复杂了，有一个自指的难题，被称为日本箭头难题...

提问者： 那真的很有趣。也许是这样，计算机科学和机器学习以及神经网络出现了复苏，所以使用数据构建算法。这是构建算法的另一种方式，对吧？

回答者： 是的，你可以这样认为。与使用自然语言构建算法相反，使用数据构建其他算法。那么，这个计算机科学分支的观点是数据几乎比算法的机制更重要。这似乎更适合某种非极客的人，你是否知道这可能是为什么它蓬勃发展，并且有自己的社群。我认为这真的很引人注目，因为甚至那些与之一起工作的人也不知道学到了什么...

提问者： 那是一个非常有趣的想法，它使算法更容易被不同社群、不同类型的人理解。是的，这真的很有趣，就像文学编程可能会使编程对某种类型的大脑更容易理解一样。有人认为这只是教育问题，任何人都可以学会成为一位出色的程序员，任何人都可以成为一位出色的滑雪者。是的，你知道，我希望那是真的，但我知道有很多事情我试图做，我也很有动力，我一直试图建立自己，但我从未超过一定水平。例如，我不能使用三维物体在我的脑中...

提问者： 那么让我们回到计算机编程的艺术。在1962年，你为这个巨著制定了目录，对吗？

回答者： 是的，

提问者： 它原本应该是一个单一的书，有12章。现在，今天是什么情况？57年后，你正在进行第4卷的中间，总共有7卷，而你现在正在进行4B

回答者： B卷，确切地是4B。

提问者： 我能请你完成一个不可能的任务吗，就是尝试通过给出排序和组合算法中的一些例子来总结这本书到目前为止？是的，根据建筑物的楼层数而定。是的，第一卷称为基础算法，讨论的是一些你无法缺少的东西...

回答者： 你无法缺少的东西。我猜你必须了解程序是什么，算法是什么，它还谈到了一个低级的机器，所以你可以对发生的事情有一些想法。它有输入/输出和子程序的基本概念，数学归纳法，写数学。因此，使我的书与其他许多书不同的是，我不仅试图呈现算法，而且试图分析它们，这意味着在数量上我说它不仅仅是工作，而且它的速度是多快，好吧，所以我需要数学。然后在计算机内部结构化数据和表示信息的标准方法，因此那就是所有卷1...第2卷谈到了，被称为半数值算法，这里我们写程序，但我们还涉及到数字...

回答者： 算法涉及到任何种类的对象，但是特定的情况是涉及到数字的对象，那么我们就有某些特殊的范例适用于具有数字的事物。因此，有像数字上的算术，有充满数字的矩阵，有随机数字，有充满数字的幂级数。有以结构化方式包含数字的不同代数概念...

提问者： 计算机在思考算法的方式中的算术，是浮点，

回答者： 浮点算术，高精度算术，不仅仅是加法、减法、乘法，还有数字的比较。所以检查。然后第3卷谈到，我喜欢那个，排序插入排序，一个排序的圈，对吧？

回答者： 对。所以在这里，你知道，我们不一定处理数字，因为你滑倒了，你看到了字母和其他对象，而搜索我们一直在做。我们现在搜索了很多，但我们必须找到一些东西。因此，像你知道的，这些卷中没有一个是关于特定应用的，但这些应用是人们为什么想要了解排序，人们为什么想要了解随机数字的例子...

回答者： 所以第4卷进入组合...

回答者： 再次，这是我们需要处理的无数事物的地方，我们发现其中一个好主意可能使某些东西的速度提高超过一百万倍，我们正在处理的问题可能永远不会被高效解决，但这并不意味着我们放弃，我们有机会拥有好的主意，而且我们在上面能够更快地进行。因此，这就是组合算法，这是我正在使用的算法...

## Graph theory
Questioner (Q): That's what I like the most in the domain of graphs and graph theory.

Answer (A): Graphs are great because they're terrific models of so many things in the real world. You throw numbers on a graph, you got a network. Combinatorial, in general, is in any arrangement of objects that has some kind of a higher non-random structure. It's possible to put something together satisfying all these conditions, like arrows pointing to each other.

Q: That's volume four.

A: That's volume four. What is a sage of Hawaiian for? In 1962 when I started writing down a table of contents, it wasn't going to be a book about computer programming in general; it was going to be a book about how to write compilers. I was asked to write a book explaining how to write a compiler. At that time, there were only a few dozen people in the world who had written compilers, and I happened to be one of them. I also had some experience writing for the campus newspaper and things like that. So, I said okay, I'm the only person I know who has written a compiler but hasn't invented any new techniques for writing compilers. All the other people I knew had super ideas, but I couldn't see that they would be able to write a book that would describe anybody else's ideas with their own. So, I could be the journalist and I could explain all these cool ideas about compiler writing. I started with a chapter about data structures, introductory material, and talking about searching because a compiler writer has to look up the variables in a symbol table. You need all these basic techniques. I also threw in a chapter on combinatorial methods, even though there weren't many algorithms known in 1962. Chapter twelve was going to be actual compilers applying all the stuff in chapters 1 to 11 to make compilers. That was my table of contents from 1962.

During the 70s, the whole field of combinatorics went through a huge explosion, people talk about it as a combinatorial explosion. They usually mean that the number of cases goes up, you change n to n plus 1, and all of a sudden, your problem has gotten more than ten times harder. There was an explosion of ideas about combinatorics in the 70s, to the point that, by 1975, I bet more than half of all the journals of computer science were about combinatorial methods.

**提问者（Q）：** 这是我在图表和图论领域最喜欢的东西。

**回答者（A）：** 图表非常棒，因为它们是现实世界中许多事物的出色模型。你将数字放在图上，你就得到了一个网络。组合学，总的来说，是任何具有某种较高非随机结构的对象排列。将满足所有这些条件的东西放在一起是可能的，就像箭头指向彼此一样。

**Q：** 那是第四卷。

**A：** 那是第四卷。夏威夷语中的“sage”是什么？1962年我开始写目录时，它不是一本关于计算机编程的一般书，而是一本关于如何编写编译器的书。我被要求写一本解释如何编写编译器的书。那时，世界上只有几十个人写过编译器，而我恰好是其中之一。我还有一些为校园报纸等写作的经验。所以，我说好吧，我是我所知道的唯一一个写过编译器但没有发明任何新技术来编写编译器的人。我认识的所有其他人都有很棒的想法，但我看不出他们是否能够写一本描述别人想法的书。所以，我可以成为记者，我可以解释有关编写编译器的所有这些酷想法。我从第一章开始谈论数据结构，引导性材料，以及关于搜索的内容，因为编译器编写者必须在符号表中查找变量。你需要所有这些基本技术。我还加入了一章关于组合方法的内容，尽管在1962年并不了解许多有关组合方法的算法。第十二章将是实际的编译器，应用在前11章中的所有内容上制作编译器。那是我1962年的目录。

在70年代，整个组合数学领域发生了巨大的爆炸，人们谈论它为组合爆炸。他们通常指的是情况的数量增加，你将n更改为n加1，突然之间，你的问题变得超过了十倍的难度。在70年代，有关组合数学的想法爆炸性增长，以至于到1975年，我敢打赌超过一半的计算机科学期刊都是关于组合方法的。

## Problems in combinatorics

**Questioner:** What kind of problems were occupying people's minds?

**Answer:** The problems in combinatorics, it's that.

**Questioner:** Gravity graph theory?

**Answer:** Yeah, gravity was quite dominant. I mean, all of the NP-hard problems like Hamiltonian path or foul sail going beyond graphs had efficient solutions in a small class of problems associated with Maitre D', a special mathematical construction. But once we went to things that involve three things at a time instead of two, all of a sudden, the problems got harder. Satisfiability problems, for example, where if you have clauses with three variables, nobody knows how to solve it efficiently. These articles were about finding better ways to solve cryptography problems and graph theory problems, where we have lots of data but didn't know how to find the best subset.

**Questioner:** So how did they continue to change from the 70s to today?

**Answer:** Now, there may be half a dozen conferences whose topic is cognate arcs, different kinds. Fortunately, I don't have to rewrite my book every month like I had to in the '70s, but there's still a huge amount of work being done. People are getting better ideas on these problems that don't seem to have efficient solutions, but we can still get into a lot more with them. The book I'm finishing now has a whole bunch of brand new methods that I know no other book covers, exploring the tip of the iceberg, trying out lots of things, and rewriting as I find better methods.

**提问者：** 人们都在关注什么样的问题？

**回答：** 在组合数学中的问题，就是那样。

**提问者：** 引力图论？

**回答：** 是的，引力相当占主导地位。我的意思是，所有的 NP-难问题，比如哈密顿路径或者超过图的费解问题，在一个与 Maitre D' 相关的特殊数学构造的小类问题中有了有效的解决方案。但一旦我们涉及到涉及三个事物而不是两个的问题，问题突然变得更加困难。例如，可满足性问题，如果子句中有三个变量，那么没有人知道如何高效地解决。这些文章都是关于寻找更好的解决密码学问题和图论问题的方法，其中我们有大量数据但不知道如何找到最佳子集。

**提问者：** 那么从70年代到现在，这些问题是如何发展变化的？

**回答：** 现在可能有半打与同源弧有关的会议，各种不同的会议。幸运的是，我不必像在70年代那样每个月都重写我的书，但仍然有大量的工作在进行中。人们在这些看似没有有效解决方案的问题上得到了更好的想法，但我们仍然可以在其中做更多。我正在完成的这本书有很多全新的方法，我知道没有其他书涵盖这个特定的方法，尽力探索冰山一角，尝试很多方法，并且随着发现更好的方法而不断重写。

## Thinking and Writing Process 

**Questioner:** So what's your writing process like, what's your thinking and writing process like every day?

**Answer:** It's actually the best question because I spend seven days a week doing it. The chair I'm sitting in is where the magic happens. I usually sit there, reading and writing, surrounded by other books. I found this chair, designed by a Swedish guy, and it's the only chair I can sit in for hours without realizing it. I also have a stand-up desk nearby. After writing with pencil and eraser, I get up and type, revise, and rewrite.

**Questioner:** The kernel, the idea, is first put on paper?

**Answer:** Yes, that's right. I call right maybe five programs a week, of course, literate programming. Before I describe something in my book, I always program it to see how it's working. For example, I learned of a breakthrough by Japanese people at the end of January, and I spent the next five days writing a program to implement it. Then I generalized more parts of it, tried it on other problems, and wrote the final draft involving new mathematical questions. I involve my friends who might be good at solving those problems, and they solve some, which I put in as exercises. A month later, I had absorbed one new idea. If I learn about another one, it might add more pages to the book.



**思考和写作过程**

**提问者：** 那么你的写作过程是什么样的，每天的思考和写作过程是什么样的？

**回答：** 实际上这是一个很好的问题，因为我每周都在七天都在做这件事。我坐的椅子是魔法发生的地方。我通常坐在那里，阅读和写作，周围是其他的书。我找到了这把椅子，是瑞典设计师设计的，是我唯一可以坐上几个小时而不知道自己在椅子上的椅子。我还有一个随身的站立式写字桌。用铅笔和橡皮擦写完后，我就站起来打字，修改和重写。

**提问者：** 核心思想首先被写在纸上？

**回答：** 是的，就是这样。我一周可能写五个程序，当然是文学化编程。在我描述书中的某个内容之前，我总是先编写程序看看它是如何工作的。例如，我在一月底得知日本人取得的突破性进展，然后花了接下来的五天编写一个实现它的程序。然后我对其进行了更多的泛化，尝试在其他问题上使用，并编写了最终的草稿，其中涉及到新的数学问题。我会找一些擅长解决这些问题的朋友，他们解决了其中的一些问题，我就将其放入练习中。一个月后，我吸收了一个新的想法。如果我了解到另一个想法，可能会给这本书增加更多的页面。

## Some days harder than others

**Q:** Well, so in the process in that one month process, are some days harder than others?

**A:** Are some days harder than others? Well, yeah, my work is fun, but I also work hard. Every big job has parts that are a lot more fun than others. So many days I'll say, "Why do I have to have such high standards? Like, why couldn't I just be sloppy and not try this out and just report the answer?" But I know that people are counting on me to do this. So, okay, so, okay, I don my grit my teeth and do it. And then the joy comes out when I see that actually, you know, I'm getting good results. And even more when I see that somebody has actually read and understood what I wrote and told me how to make it even better.

I did want to mention something about the method. So, I got this tablet here where I do the first, you know, the first writing of concepts.

**Q:** And what language?

**A:** I didn't write. So hey, take a look at, you know, here, random. Say, explain how to draw such skewed pixel diagrams. Okay, so I got this paper about 40 years ago when I was visiting my sister in Canada, and they make tablets of paper with this nice large size and just the right.

**Q:** Very small space between like, oh yeah, yeah. Particularly also just.

**A:** Yeah, you know, I've got these manuscripts going back to the '60s, and those are when I get my ideas on paper, okay? But I'm a good typist. In fact, I went to type in school when I was in high school, and so I can type faster than I think. So then when I do the editing, you know, stand up and type, then I revise this, and it comes out a lot different than what you look for. Style and rhythm and things like that come out at the typing stage.

**Q:** And you type in TeX.

**A:** And I type in TeX, and can you?

**Q:** Can you think in TeX?

**A:** No. So to a certain extent, I have only a small number of idioms that I use, like, you know, a beginning or theorem I do something for displayed equation I do something and so on, but I have to see it.

## Macros

**Q:** In the way that it's on here, yeah, right? For example, Turing wrote, what the other direction, you don't write macros. You don't think in macros.

**A:** Particularly. But when I need a macro, I'll go ahead and and these and do it. But the thing is, I also write to fit. I mean, I'll I'll change something if I can if I can save a line. It's like haiku. I'll figure out a way to rewrite the sentence so that it'll look better on the page. And I shouldn't be wasting my time on that. But I can't resist because I know it's only another three percent of the time or something like that.

**Q:** And it could also be argued that that is what life is about.

**A:** Ah yes, in fact, that's true. Like, like I worked in the garden one day a week, and that's kind of a description of my life is getting rid of weeds, you know, removing bugs for programs.

**Q:** So, you know, a lot of writers talk about, you know, basically suffering the writing processes. Yeah, having, you know, it's extremely difficult. And I think of programming, especially the or technical writing that you're doing can be like that. Do you find yourself methodologically? How do you every day sit down to do the work? Is it a challenge? You kind of say it's, you know, it's fun, but it'd be interesting to hear if there are non-fun parts that you really struggle with.

**A:** Yes, the fun comes with when I'm able to put together ideas of two people who didn't know about each other. And so I might be the first person that saw both of their ideas, and then, you know, then I get to make the synthesis, and that gives me a chance to be creative. But the drudge work is where I've got to chase everything down to its root. This leads me into really interesting stuff. I mean, like I learned about Sanskrit, and again, you know, I try to give credit to all the authors. And so I write to people who know that the people thought as if they're dead. I communicate this way. I got to get the math right, and I got to check all my programs, try to find holes in them, and I rewrite the programs after I get a better idea.

**Q:** Is there ever dead-ends data and?

**A:** So, yeah, I throw stuff out. Yeah, look, one of the things that I spent a lot of time preparing a major example based on the game of baseball. And I know a lot of people for whom baseball is the most important thing in the world, you know, yes. But it's, but I also know a lot of people for whom cricket is the most important in the world or soccer or something, you know. And I realized that if I had a big sample, I mean, it was gonna have a fold-out illustration and everything, I was saying, "Well, what am I really teaching about algorithms here where I had this, this is this baseball example? And if I was a person who knew only cricket, wouldn't think, what would they think about this?" And so I ripped the whole thing out, but I, you know, I had something that would really appeal to people who grew up with baseball as a major theme in their life.

**Q:** Which is a lot of people but the small minority. I took out bowling to even a smaller minority.

**Q:** What's the art in the art of programming? Why is there of the few words in the title? Why is art one of them?

**A:** Yeah, well, that's what I wrote my Turing lecture about. And so when people talk about art, it really, I mean, what the word means is something that's not of nature. So when you have artificial intelligence, that art comes from the same root saying that this is something that was created by human beings. And then it's gotten a further meaning, often a fine art, which has this beauty to the mix and says, you know, we have things that are artistically done. And this means not only done by humans but also done in a way that's elegant and brings joy. And has, I guess what Tolstoy burrs dusky, but anyway, it's that part that says that it's done well, as well as not only different from nature in general. Then, alright, is what human beings are specifically good at. And when they say, "Hey, like artificial intelligence," well, they're trying to mimic human beings.

**Q:** But there's an element of fine art and beauty you are well.

**A:** That's what I try to also say that you can write a program and make

 a work of art.

 ## 有些日子比其他日子更难

**问：** 那么，在那一个月的过程中，有些日子比其他日子更难吗？

**答：** 有些日子比其他日子更难吗？嗯，是的，我的工作很有趣，但我也很努力工作。每个大项目都有比其他部分更有趣的部分。因此，有很多天我会说：“为什么我必须有这么高的标准呢？为什么我不能草率一些，不试一试，只是报告答案呢？”但我知道人们指望我这样做。所以，好吧，我咬紧牙关，去做，然后当我看到实际上，我知道我正在取得良好的结果时，喜悦就出现了，当我看到有人真的读懂了我写的东西，并告诉我如何使它更好时，我甚至更加高兴。

我确实想提一下关于这种方法的一些事情。所以，我有这个平板，在这里我进行概念的第一次书写。

**问：** 用什么语言？

**答：** 我没有写。所以，嘿，看一看，你知道，这里，随机。说，解释如何绘制这样倾斜的像素图。好吧，所以我大约40年前在加拿大访问我姐姐时得到了这个纸张，他们用这个漂亮的大尺寸和合适的纸制作平板。

**问：** 像哦，是的，是的。特别是，只是。

**答：** 是的，你知道，我有这些手稿可以追溯到60年代，那时是我将我的想法记录下来的时候。好吧，我是一个好打字员。事实上，我上高中的时候上过打字学校，所以我打字比我思考得更快。所以当我进行编辑时，你知道，站起来打字，然后我对此进行修改，结果与你寻找的风格和韵律等方面大不相同。

**问：** 你用TeX打字。

**答：** 我用TeX打字，你能吗？

**问：** 你能用TeX思考吗？

**答：** 不能。在某种程度上，我只使用一小部分惯用语，比如你知道开始或定理，我为显示的等式做一些事情等等，但我必须看到它。

## 宏

**问：** 就是这样的吗？例如，图灵以相反的方式写了什么，你不写宏，你不考虑宏。

**答：** 尤其是。但当我需要宏时，我会继续并这样做。但问题是，我也会进行修改以适应写作。我的意思是，如果我可以节省一行，我会改变一些东西。这就像俳句一样，我会想出一种重写句子的方式，使其在页面上看起来更好。我不应该浪费时间在这上面，但我无法抗拒，因为我知道这只是另外百分之三的时间左右。

**问：** 还有一个论点，也可以说这就是生活的真谛。

**答：** 啊是的，事实上，这是真的，就像我每周在花园里工作一天一样，那是我生活的一种描述，摆脱杂草，消除程序中的错误。

**问：** 所以，你知道，很多作家谈论的是，你知道基本上受苦于写作过程，是的，有很多困难。我认为编程，特别是你正在进行的技术写作，可能会是这样。你发现自己在方法上吗？你每天如何坐下来做工作？是一种挑战吗？你是否说这很有趣，但听到有非有趣的部分，你真的很努力吗？

**答：** 是的，有趣的部分是当我能够将两个人的想法结合起来时。因此，我可能是第一个看到他们两人的想法的人。那么，你知道，我有机会创造，但枯燥的工作是我必须追逐一切到根源。这把我引向真正有趣的事情。比如我了解梵文，再一次，你知道，我试图给所有作者以赞誉。因此，我写信给那些知道那些人已故的人，以这种方式沟通。我得把数学搞对，我得检查所有我的程序，试图找

到其中的漏洞，我在得到更好的想法后重写程序。

**问：** 有死胡同的时候吗？

**答：** 是的，我扔掉一些东西。比如，我花了很多时间准备一个基于棒球比赛的主要示例。我知道很多人对于棒球是世界上最重要的事情。但我也知道有很多人，对他们来说，板球是世界上最重要的事情，或者什么什么的。我意识到，如果我有一个大的样本，我会有一个折叠插图，我在说什么，我真的在教授这里的算法，而我有了这个例子，如果我是一个只知道板球的人，我会想：“他们对这个有什么看法？”我就剪掉了整个东西。但我，你知道，我有一个真的吸引那些把棒球作为他们生活中的主要主题的人的东西。

**问：** 这是很多人，但只是少数人，我也取消了保龄球，甚至是更小的少数人。

**问：** 在《计算机程序设计的艺术》中，为什么艺术是其中几个字之一？为什么有艺术的？ 

**答：** 是的，这是我关于艺术的图灵演讲的主题。当人们谈论艺术时，实际上这个词的意思是不是自然的事物。因此，当你有人工智能时，这个艺术来自相同的根源，说明这是由人类创造的东西。然后它得到了更深层次的含义，通常是美术的含义，这将美丽引入其中，表示我们有一些事情是以一种优雅的方式做的，带来欢乐。我猜托尔斯泰说过，然而，那就是它以出色的方式完成，不仅是与自然不同的，而且人类特别擅长的东西。当人们谈到人工智能时，他们试图模仿人类。

**问：** 但其中还有一些精美的元素和美感，你也是。

**答：** 这就是我尝试传达的，你可以编写程序并创作一件艺术品。


## Transformational surprises
Q: so now in terms
of surprising you know what ideas in
writing from sort and search to the combinatorial algorithms what ideas have
you come across that were particularly
surprising to you that that change the way you see a space of


A: I get a surprise every time I have a bug in my program but but that isn't really 

Q: what your transformational surprises for


A: example in volume for a I was especially surprised when I learned about data
structure called B BDD boolean decision diagram because I sort of had the
feeling that as an old-timer and you
know I've been programming since this since the 50s and bTW these weren't
invented until 1986 and here comes a brand new idea that revolutionized the
way to represent a boolean function and boolean functions are so basic to all
kinds of things in it I mean logically underlies it everything we can describe
all of what we know in terms of logic somehow and and here and and
propositional logic I thought that was cutting Dryden everything was known but
but but he but here comes a Randy Bryant
and oh and discovers that BDDs are incredibly powerful then then that's all
so I that mean means I have a whole new section to the book that I never would
have thought of until 1986 not until 1990s when I went when people started to got to use it for you know
billion dollar of applications and it was it was the standard way to design
computers for a long time until until sad solvers came along when in the year 2000 so that's another great big
surprise so uh a lot of these things have have totally changed the structure
of my book and the middle third of volume four B's is about that solvers
and that's 300 plus pages which is which is all
about material mostly about material that was discovered in this century and
I had to start from scratch and meet all the people in the field and right
I have 15 different sets Alvers that i wrote while preparing that seven of them
are described in the book others were for my own experience so newly invented
data structures or ways to represent a whole new class of algorithm calling you
classified yeah and the interesting thing about the BD DS was that the
theoretician started looking at it and started to describe all the things you
couldn't do with BD DS and so they were getting a bad they were getting a bad
name because you know okay they were they were useful but they didn't solve
everything I'm sure that the theoreticians are in the next 10 years are gonna show why machine learning
doesn't solve everything but I not only worried about the worst case I get a
huge delight when I can actually solve a problem that I couldn't solve before yeah even though I can't solve the
problem that's that it suggests as a further problem like I know that I'm Way
better than I was before and so I found out that BD DS could do all kinds of miraculous things and so I had been
quite a few years learning about the that territory so in general what brings
you more pleasure in proving or showing a worst case analysis of an algorithm or
showing a good average case or just showing a good case that you know
something good pragmatically can be done with this algorithm yeah I like a good case that that is maybe only a million
times faster than I was able to do before but and not worried about the fact that
and that is still that is still gonna take too long if I double the size of
the problem so that said you popularize the asymptotic notation for describing
running time obviously in the analysis of algorithms worst cases such as such
an important part do you see any aspects of that kind of analysis is lacking so
and notation - well the main purpose you have notations that that help us for the
problems we want to solve and so that they match our they match our intuitions and people who worked in number theory
had used asymptotic notation in what Ennis in a certain way but it was only
known to a small group of people and and I realized that in fact it was very
useful to be able to have a notation for something that we don't know exactly what it is but we only know partial
about it and so on stick so for example instead of Big O notation let's just
let's just take us a much simpler notation where I say 0 or 1 or 0 1 or 2
and suppose that suppose that when I had been in high school we would be allowed
to put in the middle of our formula x + 0 1 or 2 equals y okay and then then we
would learn how to multiply two such expressions together and and you know
deal with them well the same thing Big O notation says here's something that's I'm not sure
what it is but I know it's not too big I know it's not bigger than some constant times N squared or something like that
fine so I write Big O of N squared and now I learned how to add Big O of N squared to Big O of N cubed and I know
how to add Big O of N squared 2 plus 1 and square that and how to take
logarithms and Exponential's to have big O's in the middle of them and that turned out to be hugely valuable in all
of the work that I was trying to do is I'm trying to figure out how good so I have there been algorithms in your
journey that perform very differently in practice than they do in theory well the
worst case of a comet our logarithm is almost always horrible but but we have
sad solvers that are solving where one of the one of the last exercises in that
part of my book was to figure out a problem that has a hundred variables
that's that's difficult for us at solver but uh but you would think that a
problem with the hundred boolean variables has required to do 2 to the 100th operations because that's the
number of possibilities when you have 200 boolean variables in 2 to the 100th to the 100th is way bigger than then we
can handle 10 to the 17th is a lot you've mentioned over the past few years


## Algorithms
that you believe P may be equal to NP but that it's not really you know
somebody does prove that P equals NP it will not directly lead to an actual algorithm to solve difficult problems
can you explain your intuition here has it been changed and in general on the
difference between easy and difficult problems of P and NP and so on yes so the popular idea is if an algorithm
exists then somebody will find it and
it's just a matter of writing it down one point well but many more algorithms
exist than anybody can end understand or ever make you discover yeah because
they're just way beyond human comprehension of the total number of algorithms is more than mind-boggling
so so we have situations now where we know that algorithm exists but we don't
know we don't the foggiest idea what the algorithms are there's there are simple
examples based on on game playing where you have
where you say well there must be an algorithm that exists to win in the game of hex because for the first player to
win in the game of hex because hex is always either an a win for the first
player of the second player well what's the game of hack there's a game of hex which is which based on putting pebbles
onto a hexagonal board and and the white player tries to get a light path from
left to right and the black player tries to get a black path from bottom to top and how does capture occur just so and
and and there's no capture you just put levels down what one at a time but there's no drawers because they after
all the white and black are played there's either going to be a white path across from each to west or a black path
from from bottom to top so there's always you know it's the perfect
information game and people people play take turns like like tic-tac-toe and hex
or it can be different sizes but we there's no possibility of a draw and
player to move one at a time and so it's got to be either a first player win or a second player win
mathematically you follow out all the trees and and either either there's
always the win for the percolator second player okay and it's finite the game is finite so there's an algorithm
that will decide you can show it has to be one of the other because the second player could mimic the first player with
kind of a pairing strategy and so you can show that it has to be what it has
to be one or that but we don't know any algorithm no way there there a case
where you can prove the existence of the solution but we but nobody knows anyway
how to find it but more like the algorithm question there's a very
powerful theorem and graph theory by Robinson to see more that says that
every class of graphs that is closed under taking minors
has a polynomial time algorithm to determine whether it's in this class or not now a class of graphs for example
planar graphs these are graphs that you can draw in a plane without crossing lines and and a planar graph is close
taking minors means that you can shrink an edging into a point or you can delete
an edge and so you start with a planar graph and drink any edge to a point is
still planar deleting edges to a planner okay now but there are millions of
different ways to describe family of
graph that still is remains the same undertaking minor and Robertson Nassim
are proved that any such family of graphs there is a finite number of minimum graphs that are obstructions so
that if it's not in the family then then
it has to contain then there has to be a way to shrink it down and until you get
one of these bad minimum graphs that's not in the family for in plate case for
planar graph the minimum graph is a is a five-pointed star where there everything pointed to another and the minimum graph
consisting of trying to connect three utilities to three houses without crossing lines and so there are two
there are two bad graphs that are not planar and every every non planar graph
contains one of these two bad graphs by by shrinking and he said again so he
proved that there's a finite number of these bad guys always a finite know somebody says here's a family it's hard
to believe and they present its sequence of 20 papers I mean in there it's deep
work but it you know it's because that's for any arbitrary class so it's for any
arbitrary class that's closed under taking minors that's closed under maybe I'm not understanding because it seems
like a lot of them are closed taking minors almost all the important classes of graphs are there are tons of of such graphs but
also hundreds of them that arise in applications like I have a book over
here called classes of graphs and then and it it's amazing how many different
classes people have looked at so why do you bring up this theorem lower this
proof so you know there are lots of algorithms that that are known for special class of graphs for example if I
have a certain if I have a chordal graph then I can color it efficiently if I
have some kinds of graphs it'll make a great Network very soon like you'd like
to test you somebody gives you a graph that's always it in this family of grass if so then I hope then I can I can go to
the library and find an algorithm that's gonna solve my problem on that graph okay so we we have we want to have a
graph that says number than that says
give me a graph I'll tell you whether it's and whether it's in this family or not okay and so all I have to do is test
whether or not that does this given graph have a minor that's one of the bad ones a minor is is everything you can
get by shrinking and removing edges and given any minor there's a polynomial
time algorithm saying I can tell whether this is a minor of you and there's a
finite number of bad cases so I just tried you know does it have this bad case by polynomial time I got the answer
does he have this bad case probably time I got the answer a total polynomial time
and so I've solved the problem however all we know is that the number of minors
is finite we don't know what we might only know one or two of those minors but
we don't know that if we got it if we got 20 of them we don't know there might be 20 125 the Halloween all we know is
that is that it's finite so here we have a polynomial time algorithm that we don't know
mm-hm that's a really great example of what you worry about or why you think P
equals NP won't be useful but still why do you hold the intuition
that P equals NP because you have to
rule out so many possible algorithms have been not working you know you can
you can take the graph and you can represent it as in terms of certain
prime numbers and then you can multiply those together and then you can then you can take the bitwise and and and you
know and construct some certain constant in polynomial time and then that's you
know perfectly valid algorithm and that there's so many algorithms of that kind a lot of times we see random you take
data and and and we get coincidences that that that some fairly random
looking number actually is useful because because it god it happens to it
happens to self it happens to solve a problem just because you know there's
there's so many hairs on your head but it seems like unlikely that two
people are going to have the same number of hairs on their head but but they're
obvious but you can count how many people there are and how many hairs on there so there must be people walking
around in the country to have the same number of hairs on their head well that's the kind of a coincidence that
you might say also you know this this particular combination of operations just happens to prove that a graph is
has a Hamiltonian path and I see lots of cases where unexpected things happen
when you have enough enough possibilities but because the space of possibility is so huge I have to rule
them all out and so that's the reason for my intuition is good by no means approve I mean some people say you know
well P can't equal NP because you've had all these smart people you know the
smartest designers of algorithms that have been wrecking their brains for years and years and and there's million-dollar
prizes out there and you know none of them nobody has thought of the algorithm
so it must must be no such job on the other hand I can use exactly the same
logic and I can say well P must be equal to NP because there's so many smart people out here been trying to prove it
unequal to NP and they've all failed you know this kind of reminds me of the
discussion about the search for aliens they've been trying to look for them and we haven't found them yet therefore they
don't exist yeah but you can show that there's so many planets out there that they very possibly could exist yeah and right and
then there's also the possibility that that they exist but they they all
discovered machine learning or something and and and then blew each other up well
on that small quick danger let me ask do you think there's intelligent life out there in the universe I have no idea do you hope so
do you think about it it I I don't I don't spend my time thinking about
things that I could never know really and yet you do enjoy the fact that there are many things you don't know you do
enjoy the mystery of things I enjoy the fact that there that I have limits yeah
but I don't but but I don't take time to answer unsolvable questions I got it
well because you've taken on some tough questions that may seem unsolvable you
have taken on some tough questions and you seem unsolvable if there is because we are thrilled when I can get further
than I ever thought I could right yeah but but I don't what much like was religion these I'm glad the dirt that
that there are no proof that God exists or not I mean I think it would spoil the
mystery it it would be too dull yeah so
to quickly talk about the other art of artificial intelligence what is if you what's your view
you know artificial intelligence community has developed as part of computer science and in parallel with
computer science since the 60s what's your view of the AI community from the 60s to now so all the
way through it was the people who were inspired by trying to mimic intelligence
or to do things that that were somehow the greatest achievements of intelligence that had been inspiration
to people who have pushed the envelope of computer science maybe more than any
other group of people so it's all the way through it's been a great source of of good problems to to sink teeth into
and and getting getting partial answers
and then more and more successful answers over the year so this has this
has been the inspiration for lots of the great discoveries of computer science are you yourself captivated by the
possibility of creating of algorithms having echoes of intelligence in them
not as much as most of the people in the field I guess I would say but but that's
not to say that they're wrong or that it's just you asked about my own personal preferences and yeah but but
the thing that I that I worry about is
when people start believing that they've actually succeeded and because the seems
to me this huge gap between really understanding something and being able
to pretend to understand something and give these give the illusion of understanding something do you think
it's possible to create without understanding yeah so to uh I do that all the time to run I
mean that's why I use random members I like yeah but I but but there's there's
still what this great gap I don't know certain it's impossible but I'm like but I don't see a anything coming any closer
to really the the kind of stuff that I would
consider intelligence say you've mentioned something that on that line of thinking which I very much agree with so
the art of computer programming as the book is focused on single processor
algorithms and for the most part and you mentioned that's only because I set the
table of contents in 1962 you have to remember for sure there's no I'm glad I
didn't wait until 1965 or one book maybe
will touch in the Bible but one book can't always cover the entirety of everything so I'm glad yeah I'm glad the
the table of contents for the art of computer programming is what it is but
you did mention that that you thought that an understanding of the way ant colonies are able to perform incredibly
organized tasks might well be the key to understanding human cognition so these fundamentally distributed
systems so what do you think is the difference between the way Don Knuth
would sort a list and an ant colony would sort a list or performing algorithm sorting a list isn't same as
cognition though but but I know what you're getting at is well the advantage
of ant colony at least we can see what they're doing we we know which ant has
talked to which other ant and and and and it's much harder with the quick
brains to just to know how to what extent of neurons are passing signal so
I understand that aunt Connie might be a if they have the secret of cognition
think of an ant colony as a cognitive single being rather than as a colony of
lots of different ants I mean just like the cells of our brain are and and the
microbiome and all that is interacting entities but but somehow I consider
myself to be single person well you know aunt Connie you can say might be cognitive is
somehow and it's yeah I mean you know I okay I like I smash a certain aunt and
mmm that's stung what was that right you know but if we're going to crack the the
the secret of cognition it might be that we could do so by but my psyche note how
ants do it because we have a better chance to measure and they're communicating by pheromones and by
touching each other and sight but but not by much more subtle phenomenon Mike
electric currents going through but even a simpler version of that what are your thoughts of maybe Conway's Game of Life
okay so Conway's Game of Life is is able to simulate any any computable process
and any deterministic process is like how you went there I mean that's not its
most powerful thing I would say I mean
you can simulate it but the magic is that the individual units are
distributed yes and extremely simple yes we can we understand exactly what the
primitives are the permit is the just like with the anthology even simple but if we but still it doesn't say that I
understand I understand life I mean I understand it it gives me an it gives me
a better insight into what does it mean to to have a deterministic universe what
does it mean to to have free choice for example do you think God plays dice yes
I don't see any reason why God should be forbidden from using the most efficient ways to to to I mean we we know that
dice are extremely important and inefficient algorithms there are things like that couldn't be done well without
randomness and so I don't see any reason why my god should be prohibited but when the
when the algorithm requires it you don't see why the know the physics
should constrain it yeah so in 2001 you gave a series of lectures at MIT about religion and science
well that would 1999 but you published the book came out in Cooper so in 1999
you spent a little bit of time in Boston enough to give those lectures yeah and I
read in the 2001 version that most of it it's quite fascinating read I recommend
people its transcription of your lectures so what did you learn about how
ideas get started and grow from studying the history of the Bible sieve rigorously studied a very particular
part of the Bible what did you learn from this process about the way us human beings as a society develop and grow
ideas share ideas and I'm by those idea I I tried to summarize that I wouldn't
say that I that I learned a great deal of really definite things like right where I could make conclusions but I
learned more about what I don't know you have a complex subject which is really
beyond human understanding so so we give
up on saying I'm never going to get to the end of the road and I'm never going to understand it but you say but but maybe it might be good for me to to get
closer and closer and learn more about more and more about something and so you know oh how can I do that efficiently
and the answer is well use randomness and so to try a random subset of the
that that is within my grasp and and and and study that in detail instead of just
studying parts that somebody tells me to study or instead of studying nothing
because it's too hard so I I i decided
for my own amusement that one ones that I would I would take a subset of the of
the verses of the Bible and I would try to find out what the
best thinkers have said about that small subset and I had had about let's say 660
verses out of out of 3,000 I think it's one out of 500 or something like this and so then I went to the libraries
which which are well indexed uh you can you you know I spent for example at at
Boston Public Library I I would go once a week for a year and I went to I went I
have done time stuff and over Harvard library to look at this yes that weren't
in the Boston Public where they where scholars had looked at and you can call in the eight and you can go down the
shelves and and you can pretty you can look at the index and say oh there it is this verse I mentioned anywhere in this
book if so look at page 105 so I was like I could learn not only about the
Bible but about the secondary literature about the Bible the things that scholars have written about it and so that that
gave me a way to uh to zoom in on parts
of the things so that I could get more more insight and and so I look at it as
a way of giving me some firm pegs which
icon which I could hang pieces of information but not as as things where I would say and therefore this is true in
this random approach of sampling the Bible what did you learn about the the
most you know central oh one of the biggest accumulation of ideas you know
to me that the that the main thrust was not the one that most people think of as
saying you know you know don't have sex or something like this but that the main
thrust was to try to to try to figure
out how to live in harmony with God's wishes I'm assuming that God exists and I say I'm glad that I that
there's no way to prove this because that would that would I would run
through the proof once and then I'd forget it and and it would and and I would never just speculate about
spiritual things and mysteries otherwise and I think my life would be very
incomplete so I so I'm assuming that God
exists but it if but a lot of things the people say God doesn't exist but that's
still important to them and so in a way in a way that might still be other God
is there or not in some sense so it it guys important to them it's one of the
one of the verses I studied act is you can interpret as saying you know it's much better to be an atheist that not to
care at all so I would say it's yeah it's similar to the P equals NP
discussion yeah you you mentioned a mental exercise that I'd love it if you
could partake in yourself a mental exercise of being God and so how would
you if you were God dot Knuth how would you present yourself to the people of Earth you mentioned your love of
literature and there was it there's this book that would that really uh I can recommend to you if I can't think yeah
the title I think is blasphemy it talks about God revealing himself through a
computer in in in Los Alamos and and it
it's the only book that I've ever read where the punchline was really the very
last word of the book and it explained the whole idea of the book and so I
don't want to give that away but it but it's really very much about this question that that she raised
but but suppose God said okay that my
previous on means of communication with the world are and not the best for the
21st century so what should I do now and and and it's conceivable that that it
would that that God would choose the way that's described in this book and
another way to look at this exercise is looking at the human mind looking at the human spirit the human life in a
systematic way I think it mostly you want to learn humility you want to realize that once we solve one problem
that doesn't mean it worked at all so no other problems are going to drop out and and and and we have to realize that that
that there are there are things beyond our beyond our ability I see hubris all
around yeah well said if you were to run
program analysis on your own life how did you do in terms of correctness
running time resource use asymptotically speaking of course okay yeah well I
would say that question has not been asked me before and i i i started out
with library subroutines and and
learning how to be a automaton that was obedient and i had the great advantage
that i didn't have anybody to blame for my failures if I started getting not
understanding something I I knew that I should stop playing ping pong and that was that into it was my fault that I was
that I wasn't studying hard enough or something rather than that somebody was discriminating against me in some way
and I don't know how to avoid this the existence of biases in the world but i
but i but i know that that's an extra burden that i didn't have to suffer from
and and and then i I found the from from
parents I learned the idea of of altruist to other people as being more
important than then when I get out of
stuff myself I you know that I need to I need to be happy enough enough in order
to be able to speed up service but I thought but I you know but I I came to a philosophy for finally that that I
phrased as point eight is enough there
was a TV show once called hate is enough which was about a you know somebody had eight kids but but I I say point a is
enough which means if I can have a way of rating happiness I think it's good
design that to have to have an organism
that's happy about eighty percent of the time and if it was a hundred percent of
the time it would be like every like everybody's on drugs and and never and and and and everything collapses nothing
works because everybody's just too happy do you think you've achieved that point eight optimal work there are times when
I when I'm down and I you know and I think I mean I know that I'm chemically
right I know that I've actually been programmed to be I to be depressed a
certain amount of time and and and if that gets out of kilter and I'm more depressed and you know sometimes like
like I find myself trying to say now who should I be mad at today there must be a reason why
but I but then I realize you know it's just my it's just my chemistry telling
me that I'm supposed to be mad at somebody and so and so I triggered up say okay go to sleep and get better but
but if I'm but if I'm not a hundred percent happy that doesn't mean that I
should find somebody that that's screaming and and try to size them up but I'd be like I'm saying you know okay
I'm not 100% happy but but I'm happy enough to death to be a you know part of
a sustainable situation so so that's kind of the numerical analysis I do you
invert stores the human life is a point eight yeah I hope it's okay to talk
about as you talked about previously in two thousand six six you were diagnosed
with prostate cancer has that encounter with mortality changed you in some way
or the way you see the world the first encounter with mortality with Mike when
my dad died and I I went through a month when I sort of came to kink you know be
comfortable with the fact that I was going to die someday and during that month I don't know I I felt okay but I
couldn't sing and you know I and I and I couldn't do original research either
like tighten right I sort of remember after three or four weeks the first time
I started having a technical thought that made sense and was maybe slightly creative I could sort of feel they know
that and that something was starting to move again but that was you know so I
felt very empty for until I came to grips with the I yes I learned that this
is a sort of a standard grief process that people go through ok so then now I'm at a point in my life even more so
than in 2006 where where all of my go have been fulfilled except for finishing
narrative computer programming i I I had one made unfulfilled goal that
I'd wanted all my life to write a piece of a piece piece of music that and I had
an idea for for a certain kind of music that I thought ought to be written at
least somebody ought to try to do it and I and I felt that it was a that it
wasn't going to be easy but I wanted to I wanted it proof of concept I wanted to
know if it was going to work or not and so I spent a lot of time and finally I finished that piece and we had the we
had the world premiere last year on my 80th birthday and we had another premiere in Canada and there's talk of
concerts in Europe and various things so that but that's done it's part of the world's music now and it's either good
or bad but I did what I was hoping to do so the only thing that I know that that
I have on my agenda is to is to try to do as well as I can with the art of
computer programming until I go see now do you think there's an element of point eight that might point eight yeah well I
look at it more that I got actually took 21.0 with when that concert was over
with I mean I you know I so in 2006 I
was at point eight um so when I was diagnosed with prostate cancer then I
said okay well maybe this is yet you know I've I've had all kinds of good
luck all my life and there's no I'm nothing to complain about so I might die now and we'll see what happened and so
so it's quite seriously I went and I didn't I had no expectation that I
deserved better I didn't make any plans for the future I
had my surgery I came out of the surgery and and spend some time learning how to
walk again and so on is painful for a while but I got home and I realized I
hadn't really thought about what what to do next I hadn't I hadn't any expectation and I'm still alive okay now
I can write some more books but it but I didn't come with the attitude that you know I you know this was this was
terribly unfair and and I just said okay I was accepting whatever it turned out
you know I look like I gotten I got more
than my shirt already so why should I
and I didn't and I really when I got home I read I realized that I had really
not thought about the next step what I would do after I would doubt after I would be able to work and I had sort of
thought of it as if as this might you know I was comfortable with with the
fact that it was at the end but but I was hoping that I would still you know
be able to learn about satisfiability
and and also someday even write music I
didn't start I didn't started seriously on the music project until 2012 so I'm
gonna be in huge trouble if I don't talk to you about this in in the 70s you've
created the tech typesetting system together with meta font language for font description and computer modern
family of typefaces that has basically defined the methodology in the aesthetic
of the countless research fields right math physics well beyond design and so
on okay well first of all thank you I think I speak for a lot of people in saying that but question in terms of
beauty there's a beauty to typography that you've created and yet beauty is
hard to five right how does one create beautiful
letters and beautiful equations like what what so I mean perhaps there's no words to be
describing you know be described in the process but so the great Harvard
mathematician Georg deeper cut wrote a book in the 30s called the aesthetic
measure rate where he would have pictures of vases and underneath would be a number and this was how beautiful
the vase was and he had a formula for this and and he actually also right over
brought about music and so he could he could you know so I thought maybe I would part of my musical composition I
would try to program his algorithms and and you know so that I would I would
write something that had the highest number by his score well it wasn't quite rigorous enough work for a computer to
to do but anyway people have tried to put numerical value on beauty but and
and he did probably the most serious attempt and and George Gershwin's
teacher also wrote two volumes where he talked about his method of of composing
music but but you're talking about another kind of beauty and beauty and letters and letter fell against and
whatever that overture is right so so and so that's the beholder as they say
but kinder striving for excellence in whatever definition you want to give to beauty then you try to get as close to
that as you can somehow with it I guess I guess I'm trying to ask and there may
not be a good answer what loose definitions were you're operating under with the community of
people that you're working on oh the loose definition I wanted I wanted it to
appeal to me to me I knew you personally yeah that's a good start yeah no and it failed that test went
when I got volume two came out with this with the new printing and I was expecting to be the happiest day
of my life and I felt like burning like
how angry I was that I opened the book and it it was in the same beige covers
and and but but it didn't look right on the page the number two was particularly
ugly I couldn't stand any page that had a to in his page number and I was
expecting that it was you know I spent all this time making measurements and I and I had Kent had looked at dolphins in
different different ways and I hate I had great technology but but it did you
know but I but I wasn't done I had I had to retune the whole thing after 1961
has it ever made you happy finally oh oh yes
or is it appointing oh no no and so many books have come out that would never
have been written without this I just didn't just draw it's just it's a joy but I could but now I I mean all these
pages that are sitting up there I don't have a it if I didn't like him I would
change him like that's my nobody else has this ability they have to stick with
what I gave them yes so in terms of the other side of it there's the typography so the look of
the top of the type and the curves and the lines what about the spacing but
what about the spacing because you know the white space you know it seems like
you could be a little bit more systematic about the layout or oh yeah you can always go further
III I didn't I didn't stop at point eight I stopped I stopped about point
nine eight seems like you're not following your own rule for happiness or
is no no no I there's okay the course there's just
what is the Japanese word wabi-sabi or something they wear the
the most beautiful works of art are those that have flaws because then the person who who perceives them as their
own appreciation and that gives the viewer more satisfaction or a so on but but I
but no no with typography I wanted it to look as good as I could in in the vast
majority of cases and then when it doesn't then I I say okay that's 2% more
work for the wrote for the author but but I didn't want to I didn't want to
say that my job was to get 200% with and take all the work away from the author
that's what I meant by that so if you were to venture a guess how much of the
nature of reality do you think we humans understand so you mentioned you
appreciate mystery how much of the world about us is shrouded in mystery are we
are we if you were to put a number on it what what percent of it all do we
understand oh we totally how many leading zeroes any point zero point zero zero there I don't know now I think it's
infinitesimal how do we think about that what do we do about that do we continue one step at a time yeah we muddle
through I mean we do our best we realized that one that nobody's perfect
then we and we try to keep advancing but we don't spend time saying we're not
there we're not all the way to the end some some mathematicians that that would
be in the office next to me when I was in the math department they would never think about anything smaller than
countable infinity and I never you know we intersect that countable infinity because I really got up to countable
infinity I was always talking about finite stuff but but even even limiting to finite stuff which was which is which
the universe might be there's no way to really know what whether the universe is
in isn't just made out of capital in
whenever you want to call them quarks or whatever where capital n is some fun a
number all of the numbers that are comprehensible are still way smaller than most almost all finite numbers III
I got this one paper called supernatural
numbers where I what I guess you've probably ran into something called Knuth arrow notation did you ever run into
that where anyway so you take the number I think it's like I and I called it
super K but I named it after myself but it's it's but in arrow notation is
something like ten and then four arrows and a three or something might not okay no the arrow notation if you have if you
have no arrows that means multiplication XY means x times X times X times X Y
times if you have one arrow that means exponentiation so x one arrow Y means X
to the X to the X to the X to the X Y times so I find out by the way that this
is notation was invented by a guy in 1830 and and he was like he was a a a
[Music] one of the English nobility who who spent his time thinking about stuff like
this and it was exactly the same concept that I that I'm that I used arrows and
he used a slightly different notation but anyway this and then this Ackerman's function is is based on the same kind of
ideas but Ackerman was 1920s but anyway you got this number 10
quadruple arrow 3 so that's that says well we take you know we take 10 to the
10 to the 10 to the 10 to the 10 to the 10th anyway how many times do we do that oh Ken double arrow two times or
something I mean how tall is that stack but but but then we do that again because that was the only 10 triple
quadruple arrow to we take quadruple three large number it
gets way beyond comprehension okay yeah and and and so but it's so small
compared to what finite numbers really are because I want to using four arrows and you know in ten and a three I mean
let's have that let's have that many number arrows I mean the boundary
between infinite and finite is incomprehensible for us humans anyway
infinity is a good is a useful way for us to think about extremely large
extremely large things and and and and
we we can manipulate it but but we can never know that the universe is actually
and we're near that so it just so I
realize how little we know but but but
what we we found an awful lot of things
that are too hard for any one person to know even with even in our small universe yeah and we did pretty good so
when you go up to heaven and meet God and get to ask one question that would
get answered what question would you ask
what kind of browser do you have up here [Laughter]
[Music]
okay and then oh that's beautiful actually Don thank you so much it was a
huge honor to talk to you I really well thanks for the gamut of questions yeah
it was fun thanks for listening to this conversation with donald knuth thank you
to our presenting sponsor cash app downloaded use cold Luck's podcast you'll get ten dollars and ten dollars
will go to first a stem education nonprofit that inspires hundreds of thousands of young minds to learn and to
dream of engineering our future if you enjoy this podcast subscribe on YouTube
give it five stars an apple podcast supported on patreon or connect with me on Twitter and now let me leave you with
some words of wisdom from donald knuth we should continually be striving to
transform every art into a science and in the process we advance the art thank
you for listening and hope to see you next time
you