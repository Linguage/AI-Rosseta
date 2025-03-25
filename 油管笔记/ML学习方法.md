# Machine Learning 的学习方法

## 内容梗概
文章的核心思想是教授学习机器学习的六个关键步骤，帮助初学者更高效地掌握这一领域。这六个步骤涵盖了从学习Python编程语言和基础工具，到深入了解数学概念、学习机器学习框架，最终实践项目的全过程。作者强调了按步骤学习的重要性，建议初学者注重实践和项目经验，通过挑战和重新实现论文结果来加深理解，最终在机器学习领域取得更好的表现。文章还提到了多个机器学习工具和学习资源，为学习者提供了具体的指导和推荐。

文章提到了学习机器学习的六个关键步骤：

1. **学习Python基础知识：** 从掌握基本的Python编程开始，包括了解列表、字典、条件语句和循环等。

2. **学习基础数学：** 虽然许多任务可以由Python库自动化处理，但仍需要理解微积分、线性代数和概率等基础数学概念。

3. **了解ML开发者堆栈：** 掌握Python基础后，学习使用Jupyter笔记本以及Pandas、NumPy和Matplotlib等库，这对机器学习至关重要。

4. **学习机器学习和深度学习：** 推荐通过免费的机器学习专业化课程学习基本概念，然后深入了解深度学习，包括使用PyTorch等框架。

5. **实践项目：** 在Kaggle上解决挑战，并尝试重新实现论文并重现结果，这将提升实际技能。

6. **巩固知识并脱颖而出：** 学习并尝试一些更高级的概念，以在机器学习应用中脱颖而出，例如利用Kaggle竞赛、重新实现论文等。

作者建议不要匆忙学习所有课程，而是以有趣和实用为导向，随时根据需要查阅基础知识。最终目标是建立实际项目经验，提高机器学习应用技能。

在文章中，提到了以下机器学习工具和学习资源：

1. **Python：** 建议从学习基础的Python编程开始，作为机器学习的编程语言基础。

2. **Jupyter笔记本：** 用于学习和实践Python代码的工具。

3. **Pandas、NumPy、Matplotlib：** Python库，用于处理和可视化数据，是机器学习开发者堆栈的重要组成部分。

4. **PyTorch：** 一种深度学习框架，推荐用于学习深度学习。

5. **Kaggle：** 提供机器学习挑战和竞赛的平台，用于实践和应用学到的知识。

6. **Hugging Face：** 用于自然语言处理（NLP）的库，建议用于学习和实践。

7. **Coursera上的机器学习专业化课程（Andrew Ng）：** 提供机器学习基础概念的免费课程。

8. **Andrej Karpathy的神经网络系列：** 介绍了神经网络的实现和背后的数学概念。

9. **Deep Learning专业化课程：** 重点放在实现和训练神经网络上，包括对Hugging Face的应用。

这些工具和资源涵盖了从Python基础、数学知识、机器学习基础到深度学习的学习过程。

## 视频与文稿翻译
https://www.youtube.com/watch?v=gUmagAluXpk&list=WL&index=22

导言：
2024年学习机器学习所需的一切就是一台笔记本电脑和一份步骤清单。我是一名学生研究员，曾为前Meta教授工作，并与Google DeepMind、亚马逊等知名公司进行了面试，但我花了超过3年的时间才达到这一点。因此，今天我将分享如果我能重新开始学习机器学习，我将如何通过揭示六个关键步骤来学习。让我们开始吧。

总的来说，所有这些步骤不必严格按照任何特定的顺序完成，但我不会从最终且可以说是最重要的步骤开始。话虽如此，我强烈建议从学习Python的基础知识开始。Python是几乎每个人都用来进行机器学习和这个清单上的其他步骤的编程语言。这主要适用于不知道列表或字典是什么，不知道如何编写简单的if-else语句或for循环的初学者。

我甚至会说，你需要了解列表理解和类继承是什么。老实说，我不知道说什么，除了在YouTube或Google上键入“Python教程”或“课程”并开始学习。有很多令人惊叹的免费内容，但你始终要保持主动跟随教程进行编码。享受使用Python进入机器学习的乐趣，但不要深入研究。这让你从一个有趣的经验开始，因为在某个时候，你还必须学习数学。

现在，你可以争辩说你不需要数学，因为很多东西已经被酷炫的Python库自动化和处理了，这是对的。但你需要了解微积分、线性代数和概率论的所有基础知识，以理解几乎任何机器学习方法。话虽如此，你真的不需要复杂的数学。大多数数学都是高中或大学入门数学，比如你只需要理解函数的导数及其计算方法，了解矩阵是什么以及点积是如何工作的。

有很多免费的优秀资源，比如这里的课程或一个名为Khan Academy的网站。我是说，你甚至可以在Brilliant.org上学到大多数你需要的东西，可惜这并非赞助。或者你只是上大学，修读任何工程专业的强制性数学课程。在我们讨论下一个重要步骤之前，我会告诉你我学习神经网络基础数学的最喜爱资源。这已经显示出在一开始不需要匆忙通过所有的课程。实际上，我甚至不建议这样做，因为当你在一些数学上不理解的时候，这可能会令人沮丧且不有趣。

以后，你可以随时通过谷歌搜索“学习基础知识”来重新学习，然后继续下一个有趣的步骤：了解ML开发者堆栈。现在你已经掌握了Python的基础知识，如果你还没有，学习一些基本的工具，比如Jupyter笔记本和诸如Pandas、NumPy和Matplotlib之类的库。NumPy是一个用于在矩阵或数组中执行数学运算的库。这是一个很好的起点，因为现在你可以实现刚刚学到的数学，看看计算两个矩阵的点积有多简单。

Matplotlib是一个用于可视化数据和图形的工具，只需看看你在做什么数学。在我看来，至少可视化东西是有趣而且非常有用的。最后，Pandas是一个处理表格格式数据的强大工具。许多机器学习问题涉及表格数据，Pandas让你很容易地操作和可视化这些表格。所有这些库在Jupyter笔记本中都能很好地工作，并且是学习机器学习的重要组成部分，你将看到通过了解这些框架，你将自动提高你的整体实际Python和ML技能。

但再次强调，只关注基础知识，通过跟随一些教程。稍后在项目中工作时，你将真正了解这些库。那么现在让我们回到一些理论，并最终真正了解机器学习和深度学习。好吧，到目前为止，一切都不会太久，也许几周，这取决于你投入多少时间以及你已经达到了什么水平。但我现在要推荐的ML课程确实需要一些时间。

最好且可能最著名的机器学习课程或一系列课程是由Andrew Ng提供的机器学习专业化课程。很酷的是，你在这里已经了解到了一些机器学习框架，比如scikit-learn和TensorFlow。嗯，我必须承认我个人更喜欢并推荐PyTorch。但学习一个框架几乎让你迅速适应另一个

框架。这门课程是非常宝贵的，而且是免费的，尽管这是初学者课程，但它仍然非常重要。在这里，他们教授许多经典的机器学习概念，这些是你需要能够相对轻松回答在机器学习面试中经常问到的问题的东西。

现在记住，当我展示我在神经网络中学习数学的最喜爱资源时，当在Andrew的课程中学到这些东西后，我会观看Andrej Karpathy的神经网络系列。在这里，他从零开始实现了一个简单的NLP模型，并一直到一个transform模型。他还详细介绍了反向传播等方面的所有数学知识。我不能推荐这个系列的学习足够了，因为在Andrew Ng和Andrej Karpathy的课程中，你已经获得了一些关于教授的机器学习概念的实际经验。然后，我会继续进行下一个更高级且实际的课程——深度学习专业化。这门课程更侧重于实现和训练新的神经网络。

这里绝对令人惊叹的一点是，他们还包括了Hugging Face，这是一个你几乎无法回避的库。它真的很惊人，如果你觉得这门课程没有教你足够有关Hugging Face的知识，你也可以直接参加Hugging Face NLP课程。在那里，你还会学到更多NLP方面的高级概念，如果你对NLP感兴趣的话。所以，这就是我会参加并推荐的两门或甚至三门课程。

到现在为止，你已经学到了很多，还做了几个较小的项目或教程。现在是时候真正动手，做一些真实的项目了。我真的认为你在这里学到了最多，有两件事我会首先去做。我会去Kaggle，只是解决一些挑战。有许多适合各个水平的挑战，尽量不要低估复杂性，从简单的挑战开始，这样你不会感到沮丧和丧失动力。如果你确实感到沮丧，那么就尝试一些更困难、带有奖金的挑战吧。不要指望赢得其中一个，这真的很难达到那个水平，而且你还需要很多计算资源。

好的，在解决Kaggle挑战之后，我要说的最后并且是我最喜欢的项目类型是：重新实现一篇论文并重现结果。这是具有挑战性的，你将学到很多东西，最重要的是，这类项目肯定会帮助你在ML应用程序中脱颖而出。话虽如此，在学习过程中，有一些其他更简单的方法可以脱颖而出，你现在就可以开始尝试。因此，我确信你可能想观看这个视频，其中我揭示了这些技术和技巧。再见。

All you need to learn machine learning in 2024 is a laptop and a list of the steps you need to take. I'm a student researcher working for an ex-meta professor and have had interviews with Google DeepMind, Amazon, and other cool companies, but it took me over 3 years to get to this point. So today, I will share how I would learn machine learning if I could start over by revealing the six key steps you need to take. Let's get going.

In general, all these steps don't have to be strictly completed in any particular order, but I would not start with the final and arguably most important step. That said, what I do highly recommend is to start with learning the basics of Python. Python is the programming language used by pretty much everyone to work on machine learning, and every other step on this list builds on top of it. This mainly applies to beginners that don't know what a list or a dictionary are and that don't know how to write a simple if-else statement or a for loop.

I would even go as far as saying you need to learn what a list comprehension and what class inheritance are. Honestly, I don't know what else to say than just type in "Python tutorial" or "course" on YouTube or Google and get started. There's so much amazing free content out there, but you should always keep in mind to actively code along the tutorial. Enjoy getting into machine learning with Python, but don't go too in-depth. This lets you start with a fun experience because at some point, you will also have to learn maths.

Now, you could argue that you don't need maths because so much is already automated and taken care of by cool Python libraries, which is true. But you will need to know all the fundamentals of calculus, linear algebra, and probability theory to understand pretty much any machine learning approach. That said, you really don't need complex maths. Most of the maths is high school or entry-level college maths. Like, you just need to understand what the derivative of a function is and how to compute it. You need to know what a matrix is and how the dot product works.

There are amazing resources out there that are free, like these courses right here or a website called Khan Academy. I mean, you can even learn most of what you need on Brilliant.org. Sadly not sponsored. Or you just go to college and take the mandatory maths classes for any engineering major. I'll tell you about my absolute favorite resource for learning the fundamental maths for neural networks after we cover the next important steps. This already shows you that you don't need to hustle through all the courses there are in the beginning. In fact, I wouldn't even recommend that because it can be very frustrating and just not fun whenever you don't understand some maths.

Later on, you can always revisit it by just Googling "learn the basics" and then continue on to the next fun step: learning about the ML developer stack. Now you know the basics of Python, and if you haven't already, learn some basic tools like Jupyter notebooks and libraries like Pandas, NumPy, and Matplotlib. NumPy is a library for doing maths with matrices or arrays. It's a great starting point because you can now implement the maths that you just learned about and see how simple it is to compute a dot product between two matrices. Matplotlib is a tool for visualizing data and graphs, and just seeing what maths you are doing. And in my opinion at least, visualizing stuff is fun and just very useful.

Finally, Pandas is a great tool for dealing with data that is in tabular format. A lot of machine learning problems deal with tabular data, and Pandas lets you again very easily manipulate those and visualize the tables. All those libraries also work very well with Jupyter notebooks and are an essential part of learning machine learning, as you will see. By getting to know those frameworks, you will automatically improve your overall practical Python and ML skills. But again, only focus on the basics by following a few tutorials. Later when working on projects, you'll really get to know the libraries.

So now let's get back to some theory and finally actually learn about machine learning and deep learning. Okay, up until now, everything should honestly not take too long, perhaps a few weeks depending on how much time you put in and at what level you already are. But the ML courses I will now recommend do take some time. The best and probably most famous machine learning course or collection of courses is the machine learning specialization by Andrew Ng.

The cool thing is that you here already get to know some machine learning frameworks like scikit-learn and TensorFlow. Well, I do have to admit I personally prefer and would recommend PyTorch. But learning one framework pretty much lets you already quickly adapt to the other one. This course is absolute gold, and it's free. Although this is the beginner course, it is still very important. They here teach a lot of classical ML concepts, and those are the things you need to be able to answer quite easily in ML interviews.

Now remember when I teased my favorite resource for learning maths in neural networks? Well, after learning about those in Andrew's course, I would watch Andrej Karpathy's neural network series. He here implements a simple NLP model from the ground up and goes all the way up to a transformer model. He also goes through all the maths of backpropagation and so on. I cannot recommend this series enough. Since in Andrew's and Andrej Karpathy's courses, you already get some practical experience with the taught ML concepts, I would then continue on to the next more advanced and practical course: the deep learning specialization.

This course focuses more on implementing

 and training new nets, and the absolutely amazing thing here is that they also include Hugging Face, which is a library that you pretty much cannot avoid. It's really amazing, and if you feel like this course doesn't teach you enough about Hugging Face, you can also just go through the Hugging Face NLP course directly. There you also learn even more advanced concepts in NLP, well, if you are interested in NLP, that is. So yeah, those are the two or perhaps even three courses I would take and recommend.

By now, you have learned a lot and worked on several smaller projects or rather tutorials. Now it's time to actually get your hands dirty and work on real projects. I honestly think you here learn the most, and there are two things I would work on first. I would go to Kaggle and just work on challenges. There are many available for any level. Try not to underestimate the complexity and start with simpler challenges so you don't get frustrated and demotivated. And if you do, take on more difficult ones that also come with prize money. Don't expect to win one; it's really difficult to get to that point, and you also need a lot of compute.

So okay, after working on Kaggle challenges comes my final and favorite type of project to work on: re-implementing a paper and recreating the results. This is challenging, and you will learn a lot. And most importantly, this type of project will definitely help you stand out on your ML application. That said, there are a few other simpler ways to stand out that you can already get started during your learning process. So I'm sure you might want to watch this video right here where I reveal those techniques and tips. Bye-bye.

