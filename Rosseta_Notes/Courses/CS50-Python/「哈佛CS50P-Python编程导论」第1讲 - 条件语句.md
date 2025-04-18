# 「哈佛CS50P-Python编程导论」第1讲 - 条件语句

- 视频链接：[CS50P - Lecture 1 - Conditionals](https://www.youtube.com/watch?v=_b6NgY_pMdw&list=PLhQjrBD2T3817j24-GogXmWqO5Q5vYy0V&index=3)
- 官方频道：[CS50](https://www.youtube.com/@cs50)
- 课程官网：[https://cs50.harvard.edu/python/2022/](https://cs50.harvard.edu/python/2022/) 提供有详细的学习资料，包括课程视频、讲稿、程序代码等。
- 注意：本文内容由视频脚本生成，仅供辅助参考，具体的学习应以官方内容为准。
---

### 内容介绍

本篇内容整理自CS50的Python编程入门课程（CS50P）第一讲的视频脚本，主题为“条件语句”。条件语句是编程中的基石，它允许程序根据特定条件的真假来执行不同的指令序列，从而实现逻辑判断和决策。在本讲中，主讲人David Malan将引导初学者逐步了解Python中实现条件逻辑的各种方式。

讲座首先介绍了条件判断的基本概念以及Python中用于比较（如 ` == `, `<`, `>=`）和逻辑组合（`and`, `or`）的运算符。随后，重点讲解了核心的条件控制结构：`if` 语句用于开始一个条件检查，`elif` 语句用于在前一条件不满足时检查下一个互斥条件，而 `else` 语句则作为所有条件都不满足时的默认执行路径。通过 `compare.py` 和 `grade.py` 等实例，讲座不仅演示了这些语句的用法，还探讨了代码设计中的效率和可读性问题，例如，如何通过 `elif` 和 `else` 避免不必要的计算，以及如何使用链式比较简化代码。

此外，讲座还引入了模运算符（`%`）及其在判断奇偶性（`parity.py`）中的应用，并借此讨论了布尔（`bool`）数据类型和如何编写返回布尔值的函数。讲座进一步探讨了何为“Pythonic”的代码风格，展示了如何将条件逻辑写得更为简洁优雅。最后，介绍了Python较新的 `match` 语句，作为处理多分支值匹配的一种更结构化的替代方案，并通过 `house.py` 示例进行了说明。

### 内容纲要

```
CS50P - 讲座 1 - 条件语句
├── 1. 条件语句基础
│   ├── 定义：根据条件执行不同代码路径的能力
│   ├── 比较运算符：>, >=, <, <=, == (等于), != (不等于)
│   └── 赋值运算符：= (赋值) vs == (比较)
├── 2. `if` 语句
│   ├── 关键字 `if`
│   ├── 布尔表达式 (True/False)
│   ├── 语法：条件、冒号 `:`、缩进
│   └── 示例：`compare.py` (获取x, y并比较)
├── 3. 控制流与代码设计
│   ├── 流程图 (Flowchart) 可视化逻辑
│   ├── 问题：多个独立 `if` 的低效与重复检查
│   └── Q&A：重复 `if` 的设计问题 (Khalid)
├── 4. `elif` 语句
│   ├── 定义："else if"，用于互斥条件
│   ├── 作用：提高效率，避免不必要检查
│   └── 示例：改进 `compare.py` (if-elif-elif)
├── 5. `else` 语句
│   ├── 定义：处理所有前面条件为False的情况
│   ├── 作用：提供默认路径，简化逻辑
│   ├── 示例：最终 `compare.py` (if-elif-else)
│   └── Q&A：为何需要/何时使用 `else` (Speaker 1, Speaker 2)
├── 6. 逻辑运算符
│   ├── `or`：至少一个为 True 则为 True (示例: `x < y or x > y`)
│   ├── `and`：所有都为 True 才为 True (示例: `grade.py` 分数范围)
│   └── Q&A：语法细节 - 缩进和冒号的必要性 (Speaker 4)
├── 7. 优化条件逻辑
│   ├── 链式比较：`90 <= score <= 100`
│   ├── 利用 `elif` 顺序简化判断 (示例: `grade.py` 优化)
│   ├── 错误辨析：误用 `if` 替代 `elif` 导致 Bug
│   └── Q&A：误用 `if` 的后果 (Speaker 4), 能否更简化 (Speaker 5)
├── 8. 模运算与布尔函数
│   ├── 模运算符 `%`：计算余数
│   ├── 应用：`parity.py` 判断奇偶性 (`n % 2 == 0`)
│   ├── 布尔类型 `bool`：`True`, `False`
│   ├── 创建布尔函数 `is_even(n)`
│   └── Q&A：Java地址传递 vs Python (Speaker 6), 自定义函数调用方法 (Speaker 7)
├── 9. Pythonic (优雅的) 表达方式
│   ├── 定义：符合Python社区风格的简洁、易读代码
│   ├── 示例 (is_even):
│   │   ├── 条件表达式：`return True if ... else False`
│   │   └── 直接返回布尔表达式：`return n % 2 == 0`
│   └── 讨论：简洁性 vs 清晰度
├── 10. `match` 语句
│   ├── 定义：结构化模式匹配，类似 `switch`
│   ├── 语法：`match`, `case`, `|` (或), `_` (通配符/默认)
│   ├── 示例：`house.py` (哈利波特学院分配)
│   └── 优点：特定场景下比 `if/elif/else` 更紧凑、可读
└── 11. 总结
    ├── 回顾：条件语句赋予程序决策能力
    └── 展望：即将学习循环 (loops)
```



# CS50P - 讲座 1 - 条件语句

## 1. 条件语句基础

大家好，这里是CS50的Python编程入门课。我是 David Malan，这周我们重点关注条件语句。

条件语句（Conditionals），在Python和其他语言中，是一种能够提出问题并根据答案来做决策的能力，以此决定是执行这行代码，还是那行代码，或者是另外一行代码？它们允许你在自己的代码逻辑中，走上那条众所周知的“岔路口”。

那么，我们该如何做出这些决策呢？

事实证明，Python内置了很多语法来实现这一点。例如，这里有一些你可以在Python中用来提问的符号。诚然，这些主要是数学问题，但我们就从这里开始，主要是为了让早期的例子保持简单。

第一个符号，你可能从数学中认识，代表**大于** (`$>`）。
第二个符号可能看起来不太熟悉，因为我们通常在纸上会把它写成一个整体。但在键盘上，如果你想表示**大于或等于**，你会使用这个符号 (`$>=`）。
这个，当然，意味着**小于** (`<`）。
这个表示**小于或等于** (`<=`）。
而这一个有点特别。在我们之前学习函数和变量时，我们看到了如何使用**单个等号** (` = `) 来给变量赋值。但那个等号并不代表**相等**，它代表的是**赋值**，从右到左。这很好，因为它解决了赋值的问题。但这给我们留下了一个小难题，那就是我们现在如何比较左右两边的东西是否相等呢？在Python和许多其他语言中，你实际上使用**两个等号** (`$==$`)。所以，两个等号表示**相等性**，比较左右两边的东西。而一个等号，始终表示**赋值**，将右边的东西复制到左边。
最后，这个符号表示**不等于** (`$!=$`)。所以，感叹号（或称bang）后跟一个等号，意味着不等于它旁边的某个值。

## 2. `if` 语句

要使用这些符号或其他符号来提问，我们需要Python中的另一个关键字。这个关键字，很简单，就像在英语中一样，就是 `if`。你可以在Python代码中这样提问：如果这个问题的答案是**真 (True)**，那么就继续执行这段代码。

现在，让我们来编写一些这样的例子。我将切换到VS Code。我们先创建一个名为 `compare.py` 的程序，目的就是编写比较值并基于这些值做出决策的代码。

我们来输入 `code compare.py`，创建一个名为 `compare` 的新文件，我们将在其中开始表达这种逻辑。

那么，我们想比较什么呢？假设为了讨论方便，我们只想比较几个整数。但我们希望这些整数来自用户输入，这样我们就可以根据事先不知道具体值的数字来做决策。

好的，我们这样做。像过去一样，我们声明一个变量，比如 `x`。我们将它赋值为 `int` 函数的返回值，而传递给 `int` 函数的是 `input` 函数的返回值，向用户提问，比如，“x 是多少？”（`What's x?`），就像我们以前做的那样。我们对 `y` 再做一次同样的操作，向用户询问 `y` 的值，并且同样，最终也将其转换为 `int`。

```python
# compare.py (初始版本)
x = int(input("What's x? "))
y = int(input("What's y? "))
```

到目前为止，我们有了两个变量，`x` 和 `y`，它们各自都有了值。理想情况下，我们现在应该能够比较这些值了。假设我想根据这些变量的值来做决策。

我将使用关键字 `if`。并且我会使用一些数学符号来实际提出问题本身。比如这样：`if x < y:`，那么我们就把这个情况打印出来：`"x is less than y"`。

```python
# compare.py (添加第一个 if)
x = int(input("What's x? "))
y = int(input("What's y? "))

if x < y:
    print("x is less than y")
```

这还不是一个非常有趣的程序。我基本上只是根据数学运算陈述了一个显而易见的事实。但这让我得以引入一些新的语法。

具体是什么语法呢？就是这个——不仅仅是我在第四行开头添加的关键字 `if`，还有我在这里提出的问题 `x < y`。`x` 是左边的一个变量，`y` 是右边的一个变量。当然，小于号 (`<`) 表达了我提出的数学问题。

我高亮显示的这部分，技术上称为**布尔表达式 (Boolean expression)**。布尔表达式，以数学家布尔 (Boole) 的名字命名，简单来说就是一个只有“是”或“否”答案，或者严格来说，只有**真 (True)** 或 **假 (False)** 答案的问题。这很好，因为如果只有两种可能的答案，那么对我来说（以及对计算机来说）做决策就非常容易——要么做这件事，要么不做。

注意，如果你来自其他编程语言，你可能会注意到我没有输入任何括号。在Python中，至少在这种情况下，括号实际上不是必需的。但我**在行尾输入了一个冒号 (`:`)**。更重要的是，在**下一行，我用了一些缩进**开始了我的代码行，按了四次空格键，或者只按一次Tab键（它会自动转换成同样的效果）。这个**缩进**告诉Python，第五行代码**仅在**第四行问题的答案确实是**真 (True)** 的情况下才应该被执行。所以，如果 `x` 小于 `y`，那么这句短语随后就会被打印出来。

好的，我们再加几行代码。再来一个问题怎么样？`if x > y:`，那么我们就打印出来：`"x is greater than y"`。

```python
# compare.py (添加第二个 if)
x = int(input("What's x? "))
y = int(input("What's y? "))

if x < y:
    print("x is less than y")
if x > y:
    print("x is greater than y")
```

我们再做最后一个问题：`if x = y:`，然后——等等，我这里做错了什么？眼神不错。我不想把 `y` 赋值给 `x`。`if x == y:` 这才是我表达相等的方式。好的，我们打印出 `"x is equal to y"`。

```python
# compare.py (完整 if-if-if 版本)
x = int(input("What's x? "))
y = int(input("What's y? "))

if x < y:
    print("x is less than y")
if x > y:
    print("x is greater than y")
if x == y:
    print("x is equal to y")
```

所以，我现在有三个条件（conditions），如果你愿意这么称呼的话。一个问题问 `x < y`，一个问 `x > y`，一个问 `x == y`。

我们来运行代码。好的，在我的终端窗口里，我将运行 `python compare.py` 并按回车。x 是多少？我们输入 1。y 是多少？我们输入 2。这当然应该执行第一行代码，并告诉我，确实，`x is less than y`。完全符合我的预期。

## 3. 控制流与代码设计

不过，刚才在代码里到底发生了什么？

也许，让我们用可视化的方式来看看同样的代码，特别是如果你是更偏向视觉学习的人，我敢说，这就是刚才发生的事情。我们现在看到的是一个**流程图 (flow chart)**。它是这个程序逻辑的图示。更技术性地说，它展示了程序的**控制流 (control flow)**。也就是说，你在代码中控制程序流程的能力，通常是从上到下。

事实上，让我放大这个流程图的顶部。你会看到最顶端有一个椭圆形，上面写着，很直白，“开始 (Start)”。也就是说，无论图表的形状或布局如何，当你试图理解这个程序时，你的思考和逻辑都应该从这里开始。

注意从“开始”有一个箭头指向这个菱形。菱形内部是一个问题，一个布尔表达式：`x < y`。这个形状就意味着，根据这个问题的答案，向左走或向右走。具体来说，如果答案是**真 (True)**，向左走；如果答案是**假 (False)**，向右走。

我输入的分别是 1 和 2，对应 `x` 和 `y`。所以，当然，1 小于 2。这就是为什么我的程序打印出了 `"x is less than y"`。

但是，回想一下代码。代码接着问了两个更多的问题：`x > y` 吗？`x == y` 吗？流程图也描绘了这些问题。注意，无论第一个问题的答案是真是假，箭头都汇聚到下面这个第二个菱形这里。第二个菱形问第二个问题：`x > y`。这同样有真或假的答案。所以我们要么走这条路，要么走那条路。但如果 `x` 是 1，`y` 是 2，那么答案是否定的，是假。1 不大于 2（这里原文说y，应为2）。所以逻辑上，在流程图中，你这次沿着标有“假 (False)”的箭头走。注意，沿着这条假的箭头，你这次什么也没打印。这就是为什么我们屏幕上只看到一行输出。

现在，还有第三个问题。这个流程图也捕捉到了这一点。第三个菱形问 `x == y`。在这种情况下，答案同样是假，因为 1 当然不等于 2 (原文说y，应为2)。所以我们再次沿着第三个标有“假 (False)”的分支走。这就引导我们，当然，到达“停止 (Stop)”。而“停止”就表示程序结束了。

所以我认为这是正确的。那个特定的流程图确实代表了我实际编写的代码。它是正确的。它做了它应该做的事。它通过在屏幕上打印 `x is less than y` 正确地回答了问题。

但是，它在设计上可能有什么不好的地方呢？让我们做第一个区分。你写的代码仅仅做到正确并符合你的意图，这未必就足够了。从长远来看，特别是当我们的程序变得更长、更复杂、更精密时，我们也会希望它们设计得**良好 (well-designed)**。

**问：** （Khalid）关于这个程序在哪方面可以说设计得不好，尽管它是正确的，有什么想法吗？

**答：** （Khalid）我觉得 `if` 太多了，有点重复。我们或许可以把代码写得更简洁一些。

**答：** （David Malan）是的，看起来有点重复。我问，如果这样，如果那样，如果这样。然而，逻辑上讲，一旦我弄清楚了其中一个问题的答案，我应该就能知道后面一些问题的答案。简而言之，如果你看这张图，注意无论我是向左走还是向右走，我**总是**问三个问题。无论如何，所有的箭头都导向第一个、第二个和第三个菱形。所以我总是在问三个问题，不管这些答案是真是假。

## 4. `elif` 语句

那我该如何改进呢？我建议我们在Python词汇表中引入另一个关键字，即 `elif`。

这个词也有点简洁。它是英语中 "else if" 的缩写，它允许我们问一个问题，并且这个问题会**考虑**到前一个问题的答案是真是假。

这是什么意思呢？让我回到我的代码这里。我建议我们现在改进一下，通过自问，最终我们如何能问更少的问题？我建议，与其问 `if, if, if`，不如让这些条件可能变得**互斥 (mutually exclusive)**。也就是说，一旦我们得到了一个真的答案，就不要再继续回答问题了。

我将这样修改我的代码。与其问 `if, if, if`，我要说：`if x < y`，`elif x > y`，`elif x == y`。

```python
# compare.py (使用 if-elif-elif)
x = int(input("What's x? "))
y = int(input("What's y? "))

if x < y:
    print("x is less than y")
elif x > y:
    print("x is greater than y")
elif x == y:
    print("x is equal to y")
```

所以，我将隐含地，就像在英语中一样，考虑到只有在我还没有得到真响应的情况下，我才会继续问自己这些问题。思考一下这里的逻辑，英语的逻辑。如果第四行的 `x < y` 为真，打印出 `x is less than y`。如果是这样，逻辑上你就完成了。因为如果英语说的是 "if x is less than y, else if x is greater than y"，那么如果第一个问题的答案是真的，这两个条件就是互斥的。你不需要继续问那些你逻辑上已经知道答案的问题了。

现在让我运行这个程序。我认为行为会是一样的。`python compare.py`，x 是多少？输入 1。y 是多少？输入 2。`x is less than y`。老实说，我运行程序时并没有真正注意到差异。而且说实话，我的 Mac、我的 PC、我的手机现在都快得要命，以至于这类改进在我们编写更大、更快的程序之前，未必会感觉快多少。但这为长期编写更好的代码打下了基础。

那我刚刚做了什么改进呢？如果说之前的图表是这样的，它有问题在于无论如何我都要问三个问题，即使我已经弄清楚了我想在屏幕上打印什么。那么这个使用了 `if, elif, elif` 的新版程序，可能看起来更像这样。现在它变得更宽了一点。这只是因为我们把箭头画得更宽了些。但让我们关注到底问了多少个问题。

让我像之前一样放大顶部。我建议我们注意，“开始”椭圆在最顶端，它让我们先问第一个问题。`x < y`，1 小于 2 吗？但是注意这里，让我缩小，如果 1 确实小于 2，我们沿着这条标有“真 (True)”的较长箭头向下走。我们打印出 `"x is less than y"`。但随后我们立即沿着下一条箭头向下，到达标有“停止 (Stop)”的图标。这就是 `if, elif, elif` 所隐含的意思。如果我们马上从第一个 `if` 得到一个真答案，我们将打印出 `x is less than y` 然后停止。逻辑上我们到达了程序的终点。所以这张图只是图形化地表示了代码实际在做什么。

但假设我输入了别的东西。假设我的代码实际运行时，我输入了 `x` 为 2，`y` 为 1。也就是说，第一个问题的答案现在是假了。但第二个问题的答案现在是真的了。因为，当然，2 大于 1。

我们回到图表。和之前一样，我们从最顶部的“开始”出发。现在这里的第一个问题，`x < y`，答案是假，因为 2 不小于 1。所以我们沿着这条箭头到下一个问题，这个菱形。`x > y` 吗？是的，2 大于 1。所以现在我们沿着左边的箭头，标着“真 (True)”。我们打印出 `"x is greater than y"`，然后停止。

那么改进在哪里呢？在第一种情况下，我们很幸运，只需要问一个问题，然后砰，就结束了。这次，我们不得不问两个问题，但然后砰，也结束了。只有当 `x` 恰好等于 `y` 时，我们才会在逻辑上发现自己一直走到了我代码中的最后一个 `elif`。而在图示上，也只有当 `x` 等于 `y` 时，我们才会一直走到第三个菱形，第三个问题，问它是否等于 `y`。

希望到那时答案不是假。我们包含了一个假的箭头只是为了让程序本身定义完整。但逻辑上，我们不应该真的走到那里，因为在这种情况下，它必须是小于、大于或等于。

## 5. `else` 语句

**问：** （Speaker 1）我们不是应该在最后放一个 `else` 吗？

**答：** （David Malan）好问题。是的——这将是我的第三种也是最后一种方法。如果你不介意，我们马上转到那里。识别出Python中确实存在的第三个关键字，它能让我们更好地表达这种逻辑，从而更好地设计这个程序。这将解决一个特定的问题。

如果我们回到这里的代码，注意到我之前高亮的部分，`elif x == y`。问这个问题并没有错。事实上，如果你想特别周全，检查 `x` 是否小于 `y`、大于 `y` 或等于 `y` 是完全合理的。但为什么我不需要问这第三个也是最后一个问题呢？

**问：** （Speaker 2）我们不再需要问 `x` 是否等于 `y` 了，因为逻辑上，如果前两个条件都评估为假，那么只有一个条件会评估为真。那就是 `x` 等于 `y`。

**答：** （David Malan）完全正确。如果我们对数学和这里的比较都很熟悉，那么 `x` 当然要么小于 `y`，要么大于 `y`，要么等于 `y`。但一旦你排除了前两种情况，逻辑上，必然是 `x` 必须等于 `y`。如果不是这样，那么它就应该是小于或大于。

所以 Hope（指之前的提问者 Speaker 1）建议我们使用另一个关键字，`else`。我们如何使用它呢？就像我们在英语中可能做的那样。让我回到我的代码。与其费力去问第三个也是最后一个问题，我们干脆根本不问问题了。我们只用这个“包罗万象”的，可以这么说，最后一行代码，它说，`else` 就假设 `x` 等于 `y`。因此，也打印出来。

```python
# compare.py (最终 if-elif-else 版本)
x = int(input("What's x? "))
y = int(input("What's y? "))

if x < y:
    print("x is less than y")
elif x > y:
    print("x is greater than y")
else:
    print("x is equal to y")
```

这样做的好处是什么？我的代码仍然会完全一样地工作。而且，我的电脑实在太快了，我甚至注意不到它比以前工作得更快了。但如果我们做更多的工作，编写更大的程序，我们就会注意到这类事情。

但让我运行 `python compare.py`。比如，输入 1 和 2。对于这种情况仍然有效。输入 2 和 1。对于这种情况也仍然有效。输入 1 和 1。现在对于这种情况确实也有效了。

但在这些情况下，现在，让我们思考一下我们刚刚走过的路径。之前，当我们使用 `if, elif, elif` 时，我们的图表看起来有点像这样。注意，它们开始时，我们可能问一个问题，或者两个，或者最坏情况下，整整三个问题。但我们可以做得更好，使用 Hope 建议的 `else`，我们可以把这个图表精简成这样。尽管看起来图表变大了，但注意它内部的构建块变少了。这张图里的箭头和节点都更少了。

我们现在从顶部开始。“开始”引导我们到第一个问题，仍然是：`x < y`？如果答案是真的，很好。我们可以这样说，`x is less than y`，然后我们可以停止。如果不是真的，如果是假的，我们可以问下一个问题：`x > y`，真还是假？如果是真的，很好。我们可以打印 `x is greater than y`，然后停止。否则（Else），如果 `x > y` 的情况不成立，答案是假的。我们可以立即，逻辑上，断定 `x is equal to y`。我们根本不需要添加第三个问题。我们可以直接得出结论。

这里的含义是什么？通过这些图片，你可以看到程序复杂性的相对降低。第一个非常冗长和曲折，有很多最终不必要的问题。下一个变得短了一些。而这个甚至更短。而且，通常来说，你写的代码行数越少，你犯错的可能性就越小。别人读起来也更容易。所以，总的来说，这种可读性、这种简化，确实是件好事。

### 关于语法的问答

**问：** （Speaker 4）我有几个问题。如果不使用缩进会怎么样？

**答：** （David Malan）如果不使用缩进，你的程序将无法工作。Python与许多语言有点不同，它强制要求缩进。你们中一些已经编程多年的人可能不一定有正确缩进代码的最佳习惯。而Python的一个特点，可以说，就是它**强制**你缩进代码，否则它就无法工作。

**问：** （Speaker 4）嗯，冒号是必需的吗？

**答：** （David Malan）冒号是必需的吗？是的，冒号也是必需的。对于Python，你看到的就是你得到的。确实，它需要缩进，并且冒号也是必需的。Python不像C、C++和Java那样按照惯例使用花括号来表示代码块。相反，它确实依赖于这种缩进。

## 6. 逻辑运算符

好的，让我们为Python添加另一种能力，那就是这个：`or`。

就像在英语中，你可以问这个问题**或 (or)** 那个问题，你可以在Python中使用字面上的这个词 `or` 来表达同样的意思。

让我回到我的Python代码。我们来设想一下这次如何能同时问几个问题，也许这次考虑一下我们如何不关心它是大于还是等于，不关心精确的答案。让我们采取一种更粗略的方法。我们只尝试确定 `x` 是否等于 `y`？

好的，让我删除一些代码，并改变我们要问的问题。让我这样做——如果我关心它是否相等，让我们检查可能的情况。`if x < y or x > y:`，我们打印出 `"x is not equal to y"`。

```python
# compare.py (使用 or 判断不等)
x = int(input("What's x? "))
y = int(input("What's y? "))

if x < y or x > y:
    print("x is not equal to y")
else:
    print("x is equal to y")
```

为什么会这样呢，不是双关语？如果 `x` 小于 `y`，那么它显然不相等。如果 `x` 大于 `y`，它显然也不相等。所以我们可以得出结论 `x` 不等于 `y`。因此，如果我们想确保它是相等的，我们可以只使用 Hope 的 `else`，用 `print("x is equal to y")`。

再次强调，为什么是这样？如果 `x < y` 或者 `x > y`，它们显然不相等。否则，逻辑上，它们必须实际上是相等的。

我们来运行这个。运行 `python compare.py`。x 是多少？1。y 是多少？2。好的，`x is not equal to y`。再来一次，`x` 输入 2，`y` 输入 1。`x is not equal to y`。第三次，`x` 是 1，`y` 是 1。现在 `x is equal to y`。

现在，如果我们也想直观地比较一下，我建议图片看起来有点像这样。再次说明，这在逻辑上是完全相同的事情，但这只是它的图形化表示。第一个问题是什么？如果 `x < y`，那么我们沿着标有“真 (True)”的箭头走。我们说 `"x is not equal to y"`。然后我们停止。

但如果 `x` 不小于 `y` 呢？如果它大于 `y` 呢？如果是 2 和 1 呢？那么第一个问题 `x < y` 的答案就是假。所以我们走到这里。我们问第二个问题，因为有 `or`，它问的是 `x > y` 吗？如果是，注意这点，我们可以某种程度上复用这张图的相同部分，直接说 `x is not equal to y`。我们不需要不必要地添加箭头和方框。我们可以复用代码行，就像复用图的部分一样。然后我们停止。

最后，我们有以下情况。如果我们知道 `x` 不小于 `y`，我们知道 `x` 不大于 `y`，那么必然是 `x` 等于 `y` 的情况。我们不需要问第三个问题，不需要另一个菱形。我们可以直接打印出这个结果，然后也说停止。

我在这里能做什么呢？我敢打赌我可以稍微改进一下这段代码。如果我们真的想吹毛求疵，我会认为这现在真的只是一个微小的改进，但这是一种值得养成的思考习惯：我的代码能更好吗？我的代码能更简单吗？我能进一步改进这段代码吗？这很微妙，但我能改进设计吗？我能问更少的问题吗？我能把它收紧一些，可以这么说吗？大家怎么看？

**问：** （Speaker 3）你可以问 `x` 是否就等于 `y`。然后如果你打印 `x is equal to y`，否则 `x is not equal to y`。
**答：** （David Malan）完美。回想一下我们之前看到的可用符号列表中的另一个。我们不仅可以检查小于、大于或等于。我们可以直接问这个问题：它**不等于 (not equal to)** 吗 (`$!=$`)？我们为什么要浪费时间问它是否小于或者是否大于呢？如果你只关心它是否不等于，我认为我们完全可以这样做。让我们只问我们关心的那一个简单问题。

所以让我回到这里。让我只说，不是这两个问题，去掉 `or`。就说 `if x != y:`，那么就打印 `"x is not equal to y"`。

```python
# compare.py (使用 != 判断不等)
x = int(input("What's x? "))
y = int(input("What's y? "))

if x != y:
    print("x is not equal to y")
else:
    print("x is equal to y")
```

我认为这也会完全一样地工作。但是现在的图表看起来有点不同了。注意，这是我们之前的流程图，代表了相同的逻辑。它有点复杂。你得根据这两个问题的答案向左走，向右走。如果我们现在考虑这个版本的程序看起来是怎样的，它甚至更简单，也许是我们见过的最简单的。当我们启动程序时，我们只问一个，且仅一个问题：`x != y` 吗？如果是，答案为真，我们打印出 `x not equal to y`。如果答案是假，那么，当然，它必须等于 `y`，所以我们打印那个。

如果我们真的愿意，我们可以反转这个逻辑。如果我回到我的代码，并且，出于某种原因，你就是更喜欢从等于或不等于的角度思考，而不是不等于或等于，这完全取决于你。我们可以把这个改成 ` == `。但我将不得不把我 `print` 语句的顺序反过来。所以，现在让我把这两个反转一下，把第二个移到前面，第一个移到后面。

```python
# compare.py (使用 == 判断相等优先)
x = int(input("What's x? "))
y = int(input("What's y? "))

if x == y:
    print("x is equal to y")
else:
    print("x is not equal to y")
```

所以现在，当我执行这段代码时，我仍然只问一个问题。所以它仍然同样好，同样简洁。但现在的图表，不再是像之前那样，而是将 `!=` 改为 ` == `。我们只需要确保相应地打印出正确的东西。再次强调，就像代码变得越来越紧凑，字符越来越少一样，这些图表，这些流程图，也捕捉到了每个程序相对简化的过程。

好的，让我在这里暂停一下，看看现在对这些代码版本是否有任何问题。

现在，让我们引入Python中的另一个关键字，来看看我们如何能结合更多的想法。那就是字面上的 `and` 这个词，连接我们可能想一次性问的一个、两个或更多问题。

我建议我们通过一个全新的程序来探索这种逻辑，在VS Code中，我现在将创建一个新程序，比如叫做 `grade.py`。我们来考虑一下，根据学生在考试、测验或其他类似作业上的分数，他应该得到什么等级。

我将运行 `code grade.py` 来给自己创建一个新文件。我将首先获取用户的分数，同样是在某个作业或测试等上面的分数。我将把它存储在一个名为 `score` 的变量中，等于 `int` 函数的返回值，它将转换用户在被提示输入分数 (`Score:`) 时输入的任何内容。同样，用户应该配合地给我一个数字，比如 0, 1, 2，或者希望是远高于这些的，比如 97, 98, 99, 100，假设测试或评估是满分100分。

```python
# grade.py (获取分数)
score = int(input("Score: "))
```

现在，我该如何给学生的分数评定等级呢？在美国，通常情况下，如果你得到 90 到 100 分之间，那就是 A。如果在 80 到 89 分之间，是 B。如果是 70 到 79 分，是 C，以此类推，一直到 F（这里应该跳过 E，但我们会看到这里有点跳跃）。

那我该如何表达这个呢？我可以使用条件语句。我可以问几个问题，然后相应地打印出学生的等级。让我这样表达：`if` 学生的分数大于或等于 90 (`$score >= 90$`) **并且 (`and`)** 学生的分数小于或等于 100 (`$score <= 100$`)，所以它在那个范围内，我们就打印出他们的等级应该是 A。因为他们在 90 分以上这个等级范围。

`elif` 分数大于或等于 80 (`$score >= 80$`) **并且 (`and`)** 分数小于或等于，比如说，89 (`$score <= 89$`)，但这里我有一些选择。逻辑上，我其实可以用很多种方式来表达。也许为了更清晰一点，我会说分数小于 90 (`$score < 90$`)。所以我用了小于而不是小于或等于。这样我确保了这些等级之间的界限是正确的。然后，如果在 80 多分，我将给学生一个 B。

`elif` 分数大于或等于 70 (`$score >= 70$`) **并且 (`and`)** 分数小于 80 (`$score < 80$`)，我将给他们一个 C。

`elif` 分数大于或等于 60 (`$score >= 60$`) **并且 (`and`)** 分数小于 70 (`$score < 70$`)，我将给他们一个 D。

而这里有点反常，至少在我这边的一些学校是这样，`else` 我将给他们一个 F。所以我们完全跳过了 E，我们将给一个 F 作为等级。这就是那个“包罗万象”的情况。

```python
# grade.py (使用 and 定义范围)
score = int(input("Score: "))

if score >= 90 and score <= 100:
    print("Grade: A")
elif score >= 80 and score < 90:
    print("Grade: B")
elif score >= 70 and score < 80:
    print("Grade: C")
elif score >= 60 and score < 70:
    print("Grade: D")
else:
    print("Grade: F")
```

我认为，逻辑上，我做对了，至少是基于我从小到大上学的地方的情况，它会给出 A、B、C 或 D，否则就假定你得到了 F。

我们来试几个。运行 `python grade.py`。我的分数是，我们从高的开始，100。我得到了 A。下次没考好，也许是 95——仍然是 A。开始进一步下滑，下次我得了 89 分。那现在就是，比如说，B。假设我真的度过了糟糕的一周，现在是 71 分。那就是 C。或者我根本没提交，那就是 F。所以它看起来是有效的。这算不上详尽的测试，但至少基于一些抽样，我的代码似乎按预期工作。

## 7. 优化条件逻辑

但我们看看是否能把它精简一下。它没有错。它是正确的。而且，确实，根据我自己的规范，我敢说这段代码是正确的。但我们能把它收紧吗？我们能减少现在或将来出现 bug 的概率吗？我们能提高它的可读性吗？我们能提高它的效率吗？我们能让计算机回答更少的问题而得到相同的结果吗？

我们看看能做些什么。让我换个方式，仅仅是为了演示我们可以用不同的方式使用这些符号。我可以像我刚才那样说，`if score >= 90`。但我其实可以这样做，我可以把它反过来。与其说大于或等于，不如说 `90 <= score`。这里，我们说 `if 80 <= score`。这里，`70 <= score`。然后，最后，`60 <= score`。

```python
# grade.py (调整比较顺序)
score = int(input("Score: "))

if 90 <= score and score <= 100: # 注意这里and后面也改一下顺序会更自然，但保持原意
    print("Grade: A")
elif 80 <= score and score < 90:
    print("Grade: B")
elif 70 <= score and score < 80:
    print("Grade: C")
elif 60 <= score and score < 70:
    print("Grade: D")
else:
    print("Grade: F")
```

这在逻辑上是一回事。我只是把顺序换了一下，就像你如果真想在纸笔上也可以做的那样。

但现在注意这个技巧。这对于那些用 C、C++、Java 或其他语言编程过的人来说，是不可能的。注意我在这里实际上可以做的是合并这些范围。注意我问了两个问题，两个布尔表达式：`90 <= score` 吗？**并且** `score <= 100` 吗？

Python 允许你像这样嵌套这些东西，并将它们**链接 (chain)** 在一起。就像你在现实世界中用纸笔写的那样，你可以在 Python 中编码成这样：`if 90 <= score <= 100:`。这只是更简洁一些。它稍微收紧了代码。敲键盘次数更少。输入更快。向前看更容易阅读。所以这可以说是更好的。

```python
# grade.py (使用链式比较)
score = int(input("Score: "))

if 90 <= score <= 100:
    print("Grade: A")
elif 80 <= score < 90: # 保持和之前一致，这里还没优化掉 < 90
    print("Grade: B")
elif 70 <= score < 80:
    print("Grade: C")
elif 60 <= score < 70:
    print("Grade: D")
else:
    print("Grade: F")
```

这是一个改进。在这种情况下，很大程度上是美学上的。它仍然问同样数量的问题，但它做得更简洁一些。

接下来我还能做什么呢？你知道吗？每次我决定这些等级时，我不认为我必须问两个问题。我不必问，它是否大于 90 **且**小于 100？它是否大于 80 **且**小于 90？如果我重新思考我的逻辑，我或许可以做得更好。

我建议我们进一步简化它，只这样做。如果我们知道输入，暂时来说，会在 0 到 100 之间，我们可以做一些假设。我们可以说，类似这样：`if score >= 90`，那么，学生得到 A。`elif score >= 80`，学生得到 B。`elif score >= 70`，他们得到 C。`elif score >= 60`，他们得到 D，`else` 他们得到 F。

```python
# grade.py (最终优化版本)
score = int(input("Score: "))

if score >= 90:
    print("Grade: A")
elif score >= 80:
    print("Grade: B")
elif score >= 70:
    print("Grade: C")
elif score >= 60:
    print("Grade: D")
else:
    print("Grade: F")
```

我在这里做了什么？与其每次都问两个问题，检查范围的下限和上限，我在这里更聪明了一点，通过问 `if score >= 90`，那么，他们显然得到了 A 或更好。如果你的分数大于 80 (`score >= 80`)，那么，你要么应该得 A（如果分数真的很高），要么应该得 B（如果只是刚过 80）。但**因为 `elif` 的逻辑**，我们已经检查了学生的分数是否大于 90。如果不是，那么我们才问这个问题，它是否大于 80？所以你隐含地知道它在 80 到 89 的范围内。否则，你知道它在 70 到 79 的范围内，否则，它在下一个更低的范围内。

这是一个微小的优化，让我们能问更少的问题。但再次强调，它使得代码，可以说，更易读，当然更简洁，然后，希望长期来看更易于维护。

**问：** （Speaker 4）如果我们根本不用 `elif` 呢？如果我们用 `if` 来写代码会怎样？
**答：** （David Malan）是的，这是个好问题，因为它实际上会产生意想不到的效果。让我暂时去掉 F，只关注 A 到 D。如果我们回到今天故事开始的地方，关于条件语句，说 `if, if, if, if`，那么我们刚才使用更粗略的笔触并且不使用上下限范围的聪明做法，现在就会反过来成为一个缺点。

```python
# 错误示例 (grade.py 使用 if-if-if 导致 bug)
score = int(input("Score: "))

if score >= 90:
    print("Grade: A")
if score >= 80: # 错误：应该用 elif
    print("Grade: B")
if score >= 70: # 错误：应该用 elif
    print("Grade: C")
if score >= 60: # 错误：应该用 elif
    print("Grade: D")
# else: (暂时移除)
#     print("Grade: F")
```

让我运行 `python grade.py`。假设我的分数是 95。我非常兴奋。我想要我的 A，但是，不。我刚刚得到了 A、B、C 和 D。所以逻辑上，这破坏了程序。因为如果你不让这些条件互斥，那么每一个问题都会被问到，因此也会被回答。即使你的分数高于 90，逻辑上它也高于 80，高于 70，高于 60，如果我把 F 留在那儿，我也会得到 F 而不及格。非常好的问题。

**问：** （Speaker 5）有没有更好的方法来清理，即便是像我们之前那个简单的语句，就是你之前那个带有 `elif` 的版本？
**答：** （David Malan）我喜欢你对进一步简化事物的热情。我冒昧地说，至少只使用条件语句的话，这大概是最好的了。如果我的思绪飘远，我能想到一个稍微更聪明的方法来做这个，也许用一种叫做**循环 (loop)** 的东西，或者另一种编程结构。我们的词汇表中还没有那个。但是，是的，绝对有其他方法可以做到。但我认为，如果我们想把自己限制在只使用像 `if`, `and`, `or`, `else`, `elif`, `and` 等词语，那么目前还没有更好的方法。

## 8. 模运算与布尔函数

好的，我建议我们现在转向另一种方法，它使用了另一个我们到目前为止还没怎么用过的符号。我建议我们实现一个程序，我们称之为 `parity.py`。

在数学中，**奇偶性 (parity)** 可以指一个数是偶数还是奇数。这是一个有趣的问题。事实证明，在其他应用中，仅仅问一个给定的数是偶数还是奇数（也许是用户输入的数）也可能很有用。

让我编写一个名为 `parity.py` 的新程序，在我的终端输入 `code parity.py`。我建议我们以此为契机，介绍那些算术符号中的最后一个，至少是我们熟悉的绝大多数：加法、减法、乘法、除法。但之前在这个列表上，还有最后一个，一个百分号 (`%`)。在这种情况下，当它作为Python编程中的运算符使用时，它并不意味着百分比。相反，它代表所谓的**模运算符 (modulo operator)**，用于模运算。或者，至少在我们的例子中，我们将用它来计算一个数除以另一个数后的**余数 (remainder)**。

这是什么意思呢？如果你取像 1 除以 3 这样的数，3 不能整除 1。所以你得到余数 1 (`$1 % 3 = 1$`)。2 除以 3 的余数是 2 (`$2 % 3 = 2$`)。3 除以 3 的余数是 0 (`$3 % 3 = 0$`)，因为它能整除。4 除以 3 的余数是 1 (`$4 % 3 = 1$`)，因为你可以把它除一次，但还剩下 1，所以余数是 1。最后，像 5 除以 3，当然余数是 2 (`$5 % 3 = 2$`)。这就是我们所说的余数，一个数除以另一个数后剩下多少。

好的，如果我现在回到我的代码，考虑我该如何实现“这个数是偶数还是奇数？”这个问题。我们来考虑一下如何实现它，因为它可能不那么明显我们如何能使用这个额外的构建块。但事实证明它在长期来看会非常有用。

首先，我们还是从用户那里获取一个数字，存入名为 `x` 的变量中。我将把它设为对用户输入（在询问“x 是多少？”`What's x?` 之后）进行 `int` 转换的结果。我们之前已经做过很多次了。

```python
# parity.py (获取输入)
x = int(input("What's x? "))
```

我现在如何确定 `x` 是偶数还是奇数？事实证明，如果我能访问一个能告诉我余数的程序运算符，我想我能做到。

**问：** （David Malan 提问观众）事实上，让我问问大家。这只是来自小学数学，也许，一个数是**偶数 (even)** 是什么意思？说清楚点，像 0, 2, 4, 6, 8, 10, 12, 14, 16 这些都是偶数。但这到底意味着什么？Elena，如果我没念错你的名字？

**答：** （Elena）偶数就是可以被 2 整除的数。例如，2, 4, 6, 8, 10，还有...

**答：** （David Malan）完美。我们可以这样一直说下去，字面意义上一整天，因为偶数有无限多个。但很好的是，你用一个我们可以非常清楚地问的问题来表述它：这个数能被 2 **整除 (cleanly divided by two)** 吗？也就是说，我们能用 2 除它而**没有余数**，余数为 0 吗？

这太完美了，因为如果我们有这个运算符，这个百分号 (`%`)，它允许我们回答 justamente 那个问题，余数是多少，那么我们大概可以检查余数是 0 还是 1？我们是没有任何剩余，还是剩下了 1？

好的，我们来问问。如果 `x` 除以 2 的余数是 0 (`$x % 2 == 0$`)，正如 Elena 建议的，我们就打印出类似 `"even"` 的东西。并直接告诉用户。`else`，我想我们可以假设，如果一个数不是偶数，那它（如果确实是整数的话）就将是奇数 (`odd`)。所以我将打印出 `"odd"`。

```python
# parity.py (基本判断奇偶)
x = int(input("What's x? "))

if x % 2 == 0:
    print("Even")
else:
    print("Odd")
```

现在运行 `python parity.py`。x 是多少？我们从 2 开始。2 确实是偶数。我们从 4 开始。4 确实是偶数。我们来个有趣的，3。3 现在是奇数。我想我们可以一直这样做下去，希望能得到确实就是那个答案。

但我们还能在这里做什么呢？我们如何改进这个？回想一下，我们有能力**发明我们自己的函数**。为了讨论方便，我建议，我们最终会发现能够判断一个数是偶数还是奇数是很有用的。所以我们希望内置这个功能。我不认为Python有一个函数专门告诉我这个。但我可以用像刚才那样的代码来**发明**它。

让我回到我之前的版本。我建议我们这样做。我将编写一个 `main` 函数。我将重新养成定义 `main` 函数来代表程序主要部分的习惯。我将做我之前做过的事。我将从用户输入中获取一个整数，问他们 “x 是多少？” (`What's x?`)。

然后我将问这个问题。暂时，我将天真地假设这个函数已经存在，但这是一种有用的解决问题的技巧。即使我还不知道我要往哪里去，不知道我将如何发明一个判断数字是否为偶数的函数，我只假设有一个名为 `is_even` 的函数，然后我盲目地调用它，像这样：`if is_even(x):`，那么就打印出 `"Even"`。

```python
# parity.py (使用函数结构 - 初稿)
def main():
    x = int(input("What's x? "))
    if is_even(x):
        print("Even")
    else:
        print("Odd")

# is_even 函数尚未定义

main() # 调用 main 函数
```

所以，如果这个叫做 `is_even` 的神奇函数返回**真 (True)** 作为它的返回值，我将打印出它是偶数。`else`，否则，我将假设它当然是奇数。

现在这个程序的一个问题，即使我在这里调用了 `main`，是 `is_even` **不存在**。如果我现在运行它，这个程序会崩溃。但这没关系。我有能力，回想一下，发明我自己的函数。

所以我用 `def` 来**定义 (define)** 一个名为 `is_even` 的函数。我希望这个函数接受一个参数。我将称它为 `n`，只是泛指一个数字。我也可以叫它 `x`。但同样，我不想把自己搞糊涂哪个 `x` 是哪个。所以我给它一个不同的名字，这没关系。我只是更通用地叫它 `n`，代表数字 (number)。

```python
# parity.py (定义 is_even - if/else 版本)

def is_even(n):
    if n % 2 == 0:
        # 如果是偶数，返回 True
        pass # 稍后填充
    else:
        # 如果是奇数，返回 False
        pass # 稍后填充

def main():
    x = int(input("What's x? "))
    if is_even(x):
        print("Even")
    else:
        print("Odd")

main()
```

然后我这样做。我说 `if n % 2 == 0:`，就像之前一样，然后，魔法来了，你，作为程序员，实际上可以**返回 (return)** 所谓的**布尔值 (Boolean values)**。

我们已经在Python中看到，Python有 `str` (字符串)、`int` (整数)、`float` (浮点数)，所有这些都是Python中不同类型的数据。Python还有第四种数据类型叫做 **`bool`**，代表布尔值。尽管这只是给我们的列表增加了内容，但关于 `bool` 的好处是它们**只能是 `True` 或 `False`**。一个 `int` 可以是无限多个可能值中的任意一个。一个 `bool` 只能是 `True` 或 `False`。并且如果你自己写，它必须是**大写的 T 和大写的 F**。

所以如果我现在回到我的代码，考虑我到底想在这里返回什么。如果 `n % 2 == 0`，也就是说，如果 `n` 除以 2 的余数是 0，那么，我认为它是偶数，根据 Elena 你的定义。所以我们 `return True`，大写 T。`else`，如果它的余数不是 0，我很确定，数学上，它的余数必然是 1。但这不重要。我知道它不是偶数，所以我将 `return False`。我们 `return False`，大写 F。

```python
# parity.py (完整定义 is_even - if/else 版本)

def is_even(n):
    if n % 2 == 0:
        return True
    else:
        return False

def main():
    x = int(input("What's x? "))
    if is_even(x):
        print("Even")
    else:
        print("Odd")

main()
```

现在我们定义了 `main` 和 `is_even`，并且我在底部调用了 `main`，我想我做对了。`python parity.py`，回车。x 是多少？我们试试简单的，比如 2。它是偶数。再来一次。x 是多少？比如 4？偶数。再来一次，x 是多少？比如 3？它是奇数。

我在这里做了什么？我只是阐明了这一点：如果我想创建我自己的名为 `is_even` 的函数，它为我回答这个问题，那么我现在可以在这个程序中使用它，甚至可能在我将来编写的程序中使用。我现在有了一个**没有人给我，而是我自己给自己的**函数，我可以复用。我甚至可以，也许，分享给别人。我现在在第三行使用那个函数，只是为了做决策。我在那里使用了一个条件语句。我的布尔表达式，某个结果是真或假的东西，将不是像 `x < y` 或 `y > x` 或类似的显式表达式。它将是一个**函数调用**。我用一个函数作为我的布尔表达式。但这没关系，因为我知道，因为是我写的，那个 `is_even` 函数要么返回 `True`，要么返回 `False`。而这正是我在条件语句中做决策（打印 "Even" 或打印 "Odd"）所需要的全部。

**问：** （Speaker 6）你好，David。首先，非常感谢前天和今天的精彩课程。我只有一个基于Java背景的疑问。在Java中，当我们传递参数时，我们也可以传递变量的地址。Python中有类似的概念吗？

**答：** （David Malan）简短回答：没有。对于不熟悉Java或其他语言，或C、C++的人来说，通常有不同的机制来传递值，这些机制允许或不允许你改变它们。在Python中，没有。我们将看到的一切实际上都是对象。但这点以后再详细说。

**问：** （Speaker 7）我实际上有一个关于定义函数的问题，如果可以的话。

**答：** （David Malan）当然。

**问：** （Speaker 7）如果你在你的代码中定义了一个函数，就像你自己编造的那样，你是否被允许使用点运算符，就像我们用 `name.strip()` 那样，并像那样使用它？

**答：** （David Malan）好问题。如果你创建了自己的函数，你能否使用其他函数，比如我们过去见过的 `.strip()`, `.title()`, `.capitalize()`？你可以在**字符串 (strings)** 上使用那些函数。那些函数是字符串自带的。你未必能在你自己的函数上使用它们，**除非**你的函数返回一个字符串（对于你给出的例子来说）。我返回的是一个 `bool`。布尔值没有左右空白的概念。你不能调用 `strip`，不能调用 `capitalize`。但如果你在写一个返回字符串的不同函数，那绝对可以。你也可以使用那些函数。

### Pythonic (优雅的) 表达方式

好的，如果可以的话，让我把注意力转回到这个例子上，并像我们现在经常做的那样，考虑一下：我们能否改进这段代码的设计？我能让这个特定的程序变得更好吗？

我可以。这里有几种方法。我将向你展示一些现在通常被称为**Pythonic**的东西。在Python世界里，实际上有这样一个术语，如果某件事是“Pythonic”的，那它就是你在Python中做事的方式。也就是说，我们已经看到解决某些问题有如此多的不同方法。而在Python程序员社区中，有些方法往往比其他方法更受欢迎。它们往往与那些可能只有Python有，而其他语言没有的特性有关。

这里有一些语法，如果你以前用Java、C或C++编程过，你可能没见过。如果你从未编程过，这也将是新的。与其像这样用四行代码问一个 `if-else` 问题，在Python中，你实际上可以把它压缩成更优雅的一行，如果你愿意这么说的话。

与其问 `if n % 2 == 0:`，返回 `True`，`else` 返回 `False`。让我删除所有这些，只说这个：`return True if n % 2 == 0 else False`。

```python
# parity.py (is_even 使用条件表达式)

def is_even(n):
    return True if n % 2 == 0 else False

def main():
    x = int(input("What's x? "))
    if is_even(x):
        print("Even")
    else:
        print("Odd")

main()
```

现在，你们中那些确实有编程经验的人可能会觉得这挺酷的。你可以把同样的想法从四行压缩到一行。Python之所以受欢迎的原因之一是它确实读起来很像英语。它不像大多数英语或大多数人类语言那样用户友好。但注意，现在这行代码确实很能表达你的意思了：`return True if n` 除以 2 的余数是 0, `else False`。这非常接近你在英语中可能说的话，无论是关于奇偶性还是其他任何事情。

所以那个程序会完全一样地工作。`python parity.py`，我输入 2。它仍然是偶数。我输入 3。它仍然是奇数。

但我可以进一步精炼这个。再次强调，与不仅要写正确的代码，而且要写越来越好的代码，同时还要保持其可读性的想法一致，我可以做得比这更好。

注意这个值这里：`n % 2 == 0`。这是我的**布尔表达式**。它将评估为 `True` 或 `False`。`n` 除以 2 的余数是 0 吗？这，根据定义，就是一个布尔表达式。它有一个是/否的答案，一个真/假的答案。

那么，如果你的布尔表达式本身就有一个真或假的答案，你一开始为什么要问一个问题呢？为什么要问 `if`？为什么要说 `else`？**直接返回你自己的布尔表达式的值就行了。**

```python
# parity.py (is_even 最 Pythonic 版本)

def is_even(n):
    return n % 2 == 0

def main():
    x = int(input("What's x? "))
    if is_even(x):
        print("Even")
    else:
        print("Odd")

main()
```

也许最紧凑、最简洁，并且仍然可读的版本是删除这整行（尽管它很Pythonic），然后只 `return n % 2 == 0`。如果对你有帮助，让我暂时加上括号 (`return (n % 2 == 0)`)，因为括号里的会先发生。`n` 除以 2 要么余数是 0，要么不是。如果是，答案是 `True`。如果不是，答案是 `False`。所以，就返回这个“问题”本身，如果你愿意这么称呼的话。你不需要用 `if` 和 `else` 来明确地包装它。事实上，由于运算顺序，你甚至不需要括号。所以现在这也许是实现相同想法的最优雅的方式了。

那么，哪个更好？这个（`return n % 2 == 0`）相当不错。很难挑剔它，因为它非常简洁。但是，拥有一个 `if` 然后一个 `else` 也是完全可以接受的，并且同样正确。即使它可能总共有四行，如果那能帮助你更清晰地思考你的代码，并且也帮助其他人理解它。

## 9. `match` 语句

事实证明，还有另一种语法可以用来实现条件语句的相同思想，即根据某个布尔表达式的答案来选择性地做某事。你现在可以在较新版本的Python中使用的关键字叫做这个：`match`。

`match` 是一种机制，如果你以前编程过，它在精神上类似于其他语言中的 `switch`。

例如，让我关闭 `parity.py`。我来创建一个名为 `house.py` 的新文件。在 `house.py` 中，我想我们将尝试实现一个程序，提示用户输入他们的名字，然后只输出他们在哈利波特世界中所在的学院。

例如，让我这样做。我给自己一个名为 `name` 的变量，将其设置为 `input` 函数的返回值。我会问类似，“你叫什么名字？” (`What's your name?`)。之后，我将只使用传统的 `if, elif, else` 结构来决定这个人属于哪个学院。

```python
# house.py (if/elif/else 初始版本)
name = input("What's your name? ")

if name == "Harry":
    print("Gryffindor")
elif name == "Hermione":
    print("Gryffindor")
elif name == "Ron":
    print("Gryffindor")
elif name == "Draco":
    print("Slytherin")
else:
    print("Who?")
```

所以，我说 `if name == "Harry"`，就像哈利波特里的哈利，我们就打印出哈利的学院，在哈利波特世界里是格兰芬多 (Gryffindor)。`elif` 名字是赫敏 (Hermione)，那么也打印出格兰芬多，因为她也在同一个学院。`elif name == "Ron"`，我们同样打印出格兰芬多。现在让这个更有趣一点。`elif name == "Draco"`？德拉科·马尔福 (Draco Malfoy)，在书里——我们打印出斯莱特林 (Slytherin)。以防万一输入了其他人的名字，暂时，我们就假设我们不认识他们，默认情况下，`else` 打印出 `"Who?"`，只是为了传达我们实际上没有对那个特定名字的硬编码响应。

现在让我运行这个程序 `python house.py`。我会输入类似 "Harry"。瞧，我们看到哈利确实在格兰芬多。再运行一次，`python house.py`。这次输入 "Draco"。斯莱特林。现在，让我们输入一个无法识别的名字。我们重新运行 `python house.py`。输入 "Padma"，回车。Who? 因为我们实际上没有在这种情况下用 `elif` 条件硬编码 Padma 应该在哪个学院。

事实证明，还有其他方法可以实现这一点。确实，这里有些冗余，我们检查了哈利、赫敏或罗恩是否都在格兰芬多。我觉得我们至少可以用我们已经见过的技术把这段代码收紧一点。

让我这样做。我回到上面，做类似这样的事情。去掉赫敏和罗恩的这两个 `elif` 块，暂时只留下哈利的。然后我们再次使用那个 `or` 关键字，说 `or name == "Hermione"`，`or name == "Ron"`，从而把所有三种情况合并到只用一个 `if` 语句中。

```python
# house.py (使用 or 合并条件)
name = input("What's your name? ")

if name == "Harry" or name == "Hermione" or name == "Ron":
    print("Gryffindor")
elif name == "Draco":
    print("Slytherin")
else:
    print("Who?")
```

然后我们仍然为德拉科保留一个单独的 `elif`，因为他确实不在格兰芬多。最后是 `else` 来捕捉其他任何人。

现在让我运行这个版本的程序，`python house.py`。这次我输入 "Hermione"。她也仍然在格兰芬多。我再用 "Ron" 试试。那似乎也仍然是正确的。

事实证明，还有另一种完全不同的方法，或许能让你的代码不那么冗长。你可以想象，如果我们不仅有哈利、赫敏和罗恩，还有一大堆其他名字，对应格兰芬多、斯莱特林以及所有其他霍格沃茨学院，这段代码会变得多么复杂。所以你可以想象代码很快就会变得相当笨重。

事实证明，你可以使用的另一种技术，确实是这个叫做 `match` 的关键字，它在精神上非常相似，但语法不同。它允许你更紧凑地表达相同的想法。

所以我回到 `house.py`。我建议我去掉我当前的 `if, elif, else` 方法，改为这样做。字面上使用关键字 `match`，然后输入我们想要匹配的**变量**或值的名称。然后我将包含一个冒号 (`:`)。在其下方，我将包含一个字面上的关键字 `case`。我想要考虑的第一个情况 (`case`) 将是 `"Harry"`。我把 "Harry" 放在引号里，因为它是一个字符串 (`str`)。在这行末尾我将有另一个冒号。在其下方缩进的地方，我现在将打印出 `"Gryffindor"`，这当然是哈利的学院。

否则，我将有另一个 `case` 用于 `"Hermione"`。类似地，在其下方缩进，我将打印 `"Gryffindor"`。现在我将有另一个 `case` 用于 `"Ron"`，同样在引号中，带有冒号。现在打印 `"Gryffindor"`。现在我将有另一个 `case` 用于，比如说，`"Draco"`。这个变得更有趣一些，因为德拉科，当然，现在在斯莱特林。然后我现在就先这样。

```python
# house.py (match 语句初始版本)
name = input("What's your name? ")

match name:
    case "Harry":
        print("Gryffindor")
    case "Hermione":
        print("Gryffindor")
    case "Ron":
        print("Gryffindor")
    case "Draco":
        print("Slytherin")
    # 缺少默认情况
```

让我保存这个文件，回到我的终端窗口，运行 `python house.py`。我们试试 "Harry"。他似乎仍然在格兰芬多。我们再为 "Hermione" 运行一次。格兰芬多。我们跳到 "Draco"，输入德拉科的名字。他确实在斯莱特林。现在我们试试另一个我们没有处理 `case` 的名字，比如再次输入 "Padma"。我们被直接忽略了。没有任何输出，因为没有针对 "Padma" 的 `case`。

我们当然可以回去显式地为 Padma 添加一个。但如果我们想像 `else` 结构那样，只想要一个“包罗万象”的情况来处理任何名字没有被明确指定的人呢？事实证明，使用这个新的 `match` 语句，这样做的语法是仍然拥有另一个 `case`，但随后使用这个**单个下划线字符 (`_`)**，它在Python的其他上下文中也有使用。但在这里，它的意思是**任何尚未被处理的 case**，继续执行，例如，像我们之前做的那样，打印出 `"Who?"`。

```python
# house.py (match 语句带默认情况)
name = input("What's your name? ")

match name:
    case "Harry":
        print("Gryffindor")
    case "Hermione":
        print("Gryffindor")
    case "Ron":
        print("Gryffindor")
    case "Draco":
        print("Slytherin")
    case _: # 默认 case
        print("Who?")
```

现在让我们重新运行 `python house.py`。我再次输入 Padma 的名字。这次，我想我们至少会得到一个明确的响应，指示 "Who?"，而之前我们没有等效的东西。

现在，我认为我们有点退步了。我们之前通过把哈利、赫敏和罗恩都放在同一个 `if` 语句的同一行来精简了代码。但在这里，我们现在又有了三个 `case` 语句，对应他们三人。

我们可以同样精简这段代码。但语法会有点不同。我将删除赫敏和罗恩的这两个中间 `case`。然后在哈利名字旁边，冒号之前，我将使用一个**单个竖线 (`|`)**，然后是 `"Hermione"`。然后另一个单个竖线，然后是 `"Ron"`。

```python
# house.py (match 语句最终版本)
name = input("What's your name? ")

match name:
    case "Harry" | "Hermione" | "Ron": # 使用 | 合并 case
        print("Gryffindor")
    case "Draco":
        print("Slytherin")
    case _:
        print("Who?")
```

这就是如何使用这个相对较新的 `match` 语句来表达相当于 "Harry 或 Hermione 或 Ron" 的意思，但比我们之前实现的单独使用 `if` 语句更简洁。

所以现在，最后一次运行程序 `python house.py`。我们确保哈利仍然在格兰芬多。我们确保赫敏仍然在格兰芬多。我们确保罗恩仍然在格兰芬多。确实，他们三个都在。

现在，就像Python和更普遍的编程一样，总会有不同的方法来解决这些问题。这只是你工具箱里的又一个工具。可以说，它确实精简了代码。可以说，它也许更易读一些，因为语法少了一点，等号和 `elif`, `elif`, `elif` 的重复也少了一些。但最终，这对于同样的问题来说，将是一种同样正确的方法。

但事实证明，通过 `match` 语句，你还可以进行更强大的模式匹配。在这里，我们只是用它来实现与 `if, elif, else` 结构相同的思想。值得注意的是，如果你用其他一些语言编程过，这里的语法确实是正确的。你不需要，例如，像其他语言中散布的那样需要 `break` 语句。你也不需要像 `default` 或其他明确的东西。你确实只需要使用这个下划线 (`_`) 作为 `match` 结尾的“包罗万象”情况。

## 总结

仅仅通过加入一些新的关键字，如 `if`, `elif`, `else`, 以及 `and`, `or`, `match`，我们现在就有了提问关于值的能力。我们有了分析用户输入并最终对其做出决策的能力。这些，就是我们的条件语句。

接下来摆在我们面前的将是不仅能使用函数、变量和这些条件语句，而且还有，下一步，**循环 (loops)**——现在能够一次又一次地做某事的能力。

---

# 要点回顾

**CS50P - 讲座 1 - 条件语句：框架与要点**

**1. 条件语句基础**
- 条件语句（Conditionals）允许代码根据问题的答案（真或假）来决定执行哪部分代码路径，实现逻辑上的“岔路口”。
- **比较运算符**:
    - `$>` : 大于
    - `$>=` : 大于或等于
    - `<` : 小于
    - `<=` : 小于或等于
    - ` $==$ ` : 等于（比较左右两边是否相等）
    - `$!=$` : 不等于（由感叹号 `!` 和等号 ` = ` 组成）
- **赋值运算符**:
    - ` = ` : 赋值（将右边的值赋给左边的变量），不同于 ` $==$ `（相等比较）。

**2. `if` 语句**
- 使用 `if` 关键字来提出问题（条件）。
- **基本结构**: `if condition:`，其中 `condition` 是一个布尔表达式（Boolean Expression），其结果必须是 `True` 或 `False`。
- **语法要点**:
    - 条件表达式后必须跟冒号 `:`。
    - 在 `if` 语句下方的代码块必须进行 **缩进**（通常是4个空格），表示这部分代码只有在条件为 `True` 时才执行。
    - Python 中，`if` 条件两边通常不需要括号（除非为了运算优先级或可读性）。
- **示例 (compare.py)**: 获取用户输入的 x 和 y，然后使用 `if` 比较它们的大小。
- **布尔表达式**: 一个结果为真（True）或假（False）的问题。

**3. 控制流与代码设计**
- **流程图 (Flowchart)**: 可视化程序逻辑和控制流（代码执行路径）的工具，常用菱形代表判断（问题）。
- **设计问题**: 使用多个独立的 `if` 语句（`if... if... if...`）虽然可能在逻辑上正确，但效率低下，因为即使第一个条件满足，后续的 `if` 条件仍然会被检查。

**4. `elif` 语句**
- `elif` 是 "else if" 的缩写，用于在前一个 `if` 或 `elif` 条件为 `False` 时，检查另一个条件。
- **作用**: 构建互斥的条件分支，一旦某个 `if` 或 `elif` 条件为 `True`，其对应的代码块执行后，整个 `if-elif-else` 结构后续的 `elif` 和 `else` 将被跳过。
- **优点**: 提高了代码效率和设计的清晰度，避免了不必要的检查。
- **示例 (改进 compare.py)**: 使用 `if x < y: ... elif x > y: ... elif x == y: ...` 结构。

**5. `else` 语句**
- `else` 用于处理所有前面的 `if` 和 `elif` 条件都为 `False` 的情况。
- **作用**: 提供一个默认的代码执行路径，无需再指定条件。
- **优点**: 进一步简化代码，提高效率，尤其是在处理完所有特定情况后，剩余的就是唯一一种可能时（例如，比较数字大小，如果不小于且不大于，则必然等于）。
- **示例 (最终 compare.py)**: 使用 `if x < y: ... elif x > y: ... else: ...` 结构，`else` 部分隐含了 `x == y` 的情况。

**6. 逻辑运算符**
- **`or`**: 连接两个或多个条件，如果 **至少一个** 条件为 `True`，则整个表达式为 `True`。
    - 示例: `if x < y or x > y:` 用于判断 `x` 不等于 `y`。
- **`and`**: 连接两个或多个条件，只有当 **所有** 条件都为 `True` 时，整个表达式才为 `True`。
    - 示例 (grade.py): `if score >= 90 and score <= 100:` 判断分数是否在90到100之间（包含边界）。

**7. 优化条件逻辑**
- **利用 `if-elif-else` 的顺序性**: 在某些情况下（如评分），可以通过条件的顺序来简化判断。例如，检查 `$score >= 90$` 后，在 `elif score >= 80:` 中就不必再检查 `$score < 90$`，因为如果能执行到这个 `elif`，分数必然已经小于90。
- **避免错误**: 如果将互斥条件的 `elif` 误用为 `if`，会导致逻辑错误（Bug），因为多个 `if` 会被独立检查，可能导致多个代码块被错误地执行（如高分学生同时被评为A、B、C、D等级）。
- **链式比较**: Python 允许将比较运算符链接起来，使代码更简洁易读。
    - 示例: `$90 <= score <= 100` 等同于 `$score >= 90 and score <= 100$`。

**8. 模运算与布尔函数**
- **模运算符 (`%`)**: 计算除法的 **余数**。
    - 示例: `$4 % 3$` 结果是 1； `$3 % 3$` 结果是 0。
- **应用 (parity.py - 判断奇偶性)**: 通过检查一个数除以 2 的余数是否为 0 来判断其是否为偶数 (`if x % 2 == 0:`）。
- **布尔类型 (`bool`)**: Python 中的一种数据类型，只有两个值：`True` 和 `False`（注意首字母大写）。
- **创建布尔函数**: 可以定义返回 `bool` 值的函数（例如 `is_even(n)`），使代码更具可读性。
    - 示例: `def is_even(n): if n % 2 == 0: return True else: return False`

**9. Pythonic (优雅的) 表达方式**
- "Pythonic" 指的是符合 Python 社区推崇的、简洁、易读、高效的代码风格。
- **简化布尔返回**:
    - **条件表达式 (类三元)**: `return True if n % 2 == 0 else False` 可以将之前的 `if-else` 结构压缩到一行。
    - **直接返回布尔表达式**: 最简洁的方式是直接返回条件表达式的结果，因为表达式本身就会评估为 `True` 或 `False`。
        - 示例: `def is_even(n): return n % 2 == 0`
- **选择**: 虽然简洁通常是好的，但如果更明确的 `if/else` 结构有助于理解，也是完全可以接受的。

**10. `match` 语句 (结构化模式匹配)**
- `match` 语句提供了一种替代复杂 `if/elif/else` 链的结构，特别适用于根据变量的 **具体值** 来执行不同操作的场景（类似于其他语言的 `switch`）。
- **基本结构**:
    ```python
    match variable:
        case pattern1:
            # 当 variable 匹配 pattern1 时执行的代码
        case pattern2:
            # 当 variable 匹配 pattern2 时执行的代码
        case pattern3 | pattern4: # 使用 '|' 合并多个模式
            # 当 variable 匹配 pattern3 或 pattern4 时执行的代码
        case _: # 通配符，匹配任何未被前面 case 捕获的情况 (类似 else)
            # 默认情况下执行的代码
    ```
- **示例 (house.py)**: 根据输入的学生名字（"Harry", "Hermione", "Ron", "Draco"等）匹配并输出对应的霍格沃茨学院。
- **优点**: 对于值匹配的场景，通常比 `if/elif` 链更紧凑、可读性更高，且无需像某些语言那样显式使用 `break`。

**总结**
- 条件语句（`if`, `elif`, `else`, `match`）赋予了程序根据不同情况执行不同代码的能力，是构建复杂逻辑的基础。
- 通过结合比较运算符、逻辑运算符、模运算以及良好的代码结构设计，可以编写出高效且易于理解的条件逻辑。
- Python 提供了多种实现条件判断的方式，包括一些更简洁、更“Pythonic”的表达。