

# Claude Code：智能体编程的最佳实践

- 原文链接：[Claude Code Best Practices \ Anthropic](https://www.anthropic.com/engineering/claude-code-best-practices)
- 发布日期：2025 年 4 月 18 日

![](https://www-cdn.anthropic.com/images/4zrzovbb/website/6295100fcf8952bed666ba69536c581af87eef15-2554x2554.svg)



Claude Code 是一款用于智能体编程的命令行工具。本文介绍了一些在各种代码库、语言和环境下使用 Claude Code 的有效技巧。

我们最近[发布了 Claude Code](https://www.anthropic.com/news/claude-3-7-sonnet)，这是一款用于智能体编程的命令行工具。作为一项研究项目开发，Claude Code 为 Anthropic 的工程师和研究人员提供了一种更原生、更紧密地将 Claude 集成到他们的编码工作流程中的方式。

Claude Code 特意设计成低层级且不强制特定工作流程，提供接近原始模型的访问，而不是强制用户遵循特定的方式。这种设计理念创造了一个灵活、可定制、可脚本化且安全的强大工具。虽然功能强大，但这种灵活性也给新接触智能体编程工具的工程师带来了学习曲线——至少在他们摸索出自己的最佳实践之前是这样。

本文概述了一些已被证明有效的通用模式，无论是在 Anthropic 内部团队，还是在使用 Claude Code 的外部工程师，跨越各种代码库、语言和环境。本文列表中的建议并非一成不变，也并非普遍适用；请将这些建议视为起点。我们鼓励您进行实验，找出最适合您的方式！

_寻找更详细的信息？我们位于[claude.ai/code](https://claude.ai/code)的全面文档涵盖了本文提到的所有功能，并提供了更多示例、实现细节和高级技术。_

## 1. 定制您的设置

Claude Code 是一款智能体编程助手，它会自动将上下文拉入提示词中。这种上下文收集会消耗时间和 token，但您可以通过环境调优来优化它。

### a. 创建 CLAUDE.md 文件

CLAUDE.md 是一种特殊文件，Claude 会在开始对话时自动将其拉入上下文。这使其成为以下内容的理想记录位置：

- 常用 bash 命令
- 核心文件和实用函数
- 代码风格指南
- 测试说明
- 仓库规范（例如，分支命名、合并 vs. rebase 等）
- 开发者环境设置（例如，pyenv 使用、哪些编译器可用）
- 项目中任何意外的行为或警告
- 其他您希望 Claude 记住的信息

CLAUDE.md 文件没有强制的格式。我们建议保持其简洁易懂。例如：

```
# Bash commands
- npm run build: Build the project
- npm run typecheck: Run the typechecker

# Code style
- Use ES modules (import/export) syntax, not CommonJS (require)
- Destructure imports when possible (eg. import { foo } from 'bar')

# Workflow
- Be sure to typecheck when you’re done making a series of code changes
- Prefer running single tests, and not the whole test suite, for performance
```

您可以将 CLAUDE.md 文件放置在几个位置：

- **仓库的根目录**，或您运行 `claude` 的位置（最常用）。将其命名为 CLAUDE.md 并提交到 git，以便在不同会话和团队成员之间共享（推荐），或者将其命名为 CLAUDE.local.md 并添加到 .gitignore。
- **您运行 `claude` 目录的任何父目录**。这在 monorepos 中最有用，您可能在 `root/foo` 中运行 `claude`，并在 `root/CLAUDE.md` 和 `root/foo/CLAUDE.md` 中都有 CLAUDE.md 文件。这两者都会自动被拉入上下文。
- **您运行 `claude` 目录的任何子目录**。这与上面相反，在这种情况下，当您处理子目录中的文件时，Claude 会按需拉入 CLAUDE.md 文件。
- **您的主文件夹**（`~/.claude/CLAUDE.md`），这会应用于您的所有 `claude` 会话。

当您运行 `/init` 命令时，Claude 会自动为您生成一个 CLAUDE.md。

### b. 调优您的 CLAUDE.md 文件

您的 CLAUDE.md 文件成为 Claude 提示词的一部分，因此应该像任何常用的提示词一样进行优化。一个常见的错误是添加大量内容而不迭代其有效性。花时间实验并确定什么能让模型更好地遵循指令。

您可以手动向 CLAUDE.md 添加内容，或者按下 `#` 键给 Claude 一个指令，它会自动将其合并到相关的 CLAUDE.md 中。许多工程师在编码时频繁使用 `#` 来记录命令、文件和风格指南，然后将 CLAUDE.md 的更改包含在提交中，以便团队成员也能受益。

在 Anthropic，我们偶尔会将 CLAUDE.md 文件通过 [prompt improver](https://docs.anthropic.com/en/docs/build-with-claude/prompt-engineering/prompt-improver) 运行，并经常调整指令（例如，使用 "IMPORTANT" 或 "YOU MUST" 添加强调）以提高依从性。

![Claude Code tool allowlist](https://www.anthropic.com/_next/image?url=https%3A%2F%2Fwww-cdn.anthropic.com%2Fimages%2F4zrzovbb%2Fwebsite%2F6961243cc6409e41ba93895faded4f4bc1772366-1600x1231.png&w=3840&q=75)
*Claude Code 工具允许列表*

### c. 策划 Claude 的允许工具列表

默认情况下，Claude Code 会对任何可能修改您系统的操作请求许可：文件写入、许多 bash 命令、MCP 工具等。我们将 Claude Code 设计为这种刻意保守的方法，以优先考虑安全性。您可以自定义允许列表，以允许您知道是安全的其他工具，或者允许易于撤销的潜在不安全工具（例如，文件编辑、`git commit`）。

有四种方式管理允许的工具：

- 在会话提示时选择**“总是允许”**。
- 在启动 Claude Code 后使用 **`/allowed-tools` 命令**，从允许列表中添加或移除工具。例如，您可以添加 `Edit` 来始终允许文件编辑，添加 `Bash(git commit:*)` 来允许 git 提交，或者添加 `mcp__puppeteer__puppeteer_navigate` 来允许使用 Puppeteer MCP 服务器进行导航。
- **手动编辑**您的 `.claude/settings.json` 或 `~/.claude.json`（我们建议将前者提交到源代码控制以与团队共享）。
- 使用 **`--allowedTools` CLI 标志**进行特定会话的权限设置。

### d. 如果使用 GitHub，请安装 gh CLI

Claude 知道如何使用 `gh` CLI 与 GitHub 交互，例如创建 issue、打开 pull request、阅读评论等。即使没有安装 `gh`，如果您安装了 GitHub API 或 MCP 服务器，Claude 仍然可以使用它们。

## 2. 给 Claude 更多工具

Claude 可以访问您的 shell 环境，您可以在其中为它构建一套便利脚本和函数，就像您自己一样。它还可以通过 MCP 和 REST API 利用更复杂的工具。

### a. 将 Claude 与 bash 工具结合使用

Claude Code 继承了您的 bash 环境，使其能够访问您的所有工具。虽然 Claude 知道常见的实用工具，如 unix 工具和 `gh`，但如果没有指令，它将不知道您的自定义 bash 工具：

1. 告诉 Claude 工具名称并提供使用示例。
2. 告诉 Claude 运行 `--help` 查看工具文档。
3. 在 CLAUDE.md 中记录常用工具。

### b. 将 Claude 与 MCP 结合使用

Claude Code 既可以作为 MCP 服务器，也可以作为 MCP 客户端。作为客户端，它可以连接到任意数量的 MCP 服务器，通过三种方式访问其工具：

- **在项目配置中**（在 해당 目录下运行 Claude Code 时可用）。
- **在全局配置中**（在所有项目中可用）。
- **在提交的 `.mcp.json` 文件中**（供在您的代码库中工作的任何人使用）。例如，您可以将 Puppeteer 和 Sentry 服务器添加到您的 `.mcp.json` 中，这样每个在您的仓库中工作的工程师都可以开箱即用地使用这些工具。

在使用 MCP 时，使用 `--mcp-debug` 标志启动 Claude 也很有帮助，可以帮助识别配置问题。

### c. 使用自定义斜杠命令

对于重复的工作流程——调试循环、日志分析等——将提示词模板存储在 `.claude/commands` 文件夹下的 Markdown 文件中。当您键入 `/` 时，这些模板将通过斜杠命令菜单可用。您可以将这些命令提交到 git，以便团队其他成员也可以使用。

自定义斜杠命令可以包含特殊关键字 `$ARGUMENTS` 来传递命令调用时的参数。

例如，这是一个您可以用来自动拉取和修复 GitHub issue 的斜杠命令：

```
Please analyze and fix the GitHub issue: $ARGUMENTS.

Follow these steps:

1. Use `gh issue view` to get the issue details
2. Understand the problem described in the issue
3. Search the codebase for relevant files
4. Implement the necessary changes to fix the issue
5. Write and run tests to verify the fix
6. Ensure code passes linting and type checking
7. Create a descriptive commit message
8. Push and create a PR

Remember to use the GitHub CLI (`gh`) for all GitHub-related tasks.
```

将上述内容放入 `.claude/commands/fix-github-issue.md` 中，即可在 Claude Code 中将其作为 `/project:fix-github-issue` 命令使用。然后，您可以例如使用 `/project:fix-github-issue 1234` 让 Claude 修复 issue #1234。同样，您可以将自己的个人命令添加到 `~/.claude/commands` 文件夹中，以便在您的所有会话中都可以使用。

## 3. 尝试常见工作流程

Claude Code 不强制特定工作流程，让您灵活地按自己的方式使用它。在这种灵活性下，我们用户社区涌现出几种成功模式，可有效利用 Claude Code：

### a. 探索、计划、编码、提交

这种通用工作流程适用于许多问题：

1. **让 Claude 阅读相关文件、图片或 URL**，可以提供一般性指导（“阅读处理日志记录的文件”）或具体文件名（“阅读 logging.py”），但明确告诉它暂时不要编写任何代码。
    1. 这是工作流程中应该认真考虑使用子智能体的部分，特别是对于复杂问题。指示 Claude 使用子智能体验证细节或调查它可能有的特定问题，尤其是在对话或任务早期，往往可以保持上下文的可用性，而不会损失太多效率。
2. **要求 Claude 针对特定问题制定一个计划**。我们建议使用“思考 (think)”这个词来触发扩展思考模式，这为 Claude 提供了额外的计算时间来更彻底地评估替代方案。这些特定短语直接映射到系统中思考预算的增加级别：“思考 (think)” < “努力思考 (think hard)” < “更努力思考 (think harder)” < “超思考 (ultrathink)”。每个级别都会分配逐步增加的思考预算供 Claude 使用。
    2. 如果此步骤的结果看起来合理，您可以让 Claude 创建一个文档或一个 GitHub issue，包含其计划，以便在实现（步骤 3）不符合您的要求时可以回到此点。
3. **要求 Claude 在代码中实现其解决方案**。这也是一个好时机，可以要求它在实现解决方案的各个部分时，明确验证其解决方案的合理性。
4. **要求 Claude 提交结果并创建 pull request**。如果相关，这也是一个好时机，让 Claude 更新任何 README 或 changelog，说明它刚刚做了什么。

步骤 #1-#2 至关重要——没有它们，Claude 往往会直接跳到编写解决方案的代码。虽然有时这就是您想要的，但要求 Claude 先进行研究和计划，对于需要前期深入思考的问题，能显著提高性能。

### b. 编写测试，提交；编码，迭代，提交

这是一种 Anthropic 最喜欢的工作流程，适用于易于通过单元测试、集成测试或端到端测试验证的更改。测试驱动开发 (TDD) 与智能体编程结合变得更加强大：

1. **要求 Claude 根据预期的输入/输出对编写测试**。明确说明您正在进行测试驱动开发，以便它避免创建模拟实现，即使功能在代码库中尚不存在。
2. **告诉 Claude 运行测试并确认它们失败**。明确告诉它在此阶段不要编写任何实现代码通常很有帮助。
3. 当您对测试满意时，**要求 Claude 提交测试**。
4. **要求 Claude 编写通过测试的代码**，指示它不要修改测试。告诉 Claude 继续进行，直到所有测试通过。Claude 通常需要几次迭代才能编写代码、运行测试、调整代码并再次运行测试。
    1. 在此阶段，请它通过独立的子智能体验证实现没有对测试过度拟合可能会有所帮助。
5. 当您对更改满意时，**要求 Claude 提交代码**。

当 Claude 有一个清晰的目标可以迭代时，它的表现最佳——一个可视化模型、一个测试用例或另一种输出。通过提供像测试这样的预期输出，Claude 可以进行更改、评估结果并逐步改进，直到成功。

### c. 编写代码，截图结果，迭代

类似于测试工作流程，您可以为 Claude 提供视觉目标：

1. **为 Claude 提供截取浏览器截图的方法**（例如，使用 [Puppeteer MCP 服务器](https://github.com/modelcontextprotocol/servers/tree/c19925b8f0f2815ad72b08d2368f0007c86eb8e6/src/puppeteer)，一个 [iOS 模拟器 MCP 服务器](https://github.com/joshuayoes/ios-simulator-mcp)，或手动复制/粘贴截图到 Claude 中）。
2. **通过复制/粘贴或拖放图片，或提供图片文件路径，为 Claude 提供一个可视化模型**。
3. **要求 Claude 在代码中实现设计**，截取结果的截图，并迭代直到结果与模型匹配。
4. 当您满意时，**要求 Claude 提交**。

像人类一样，Claude 的输出通常通过迭代显著改善。虽然第一个版本可能不错，但在经过 2-3 次迭代后，它通常会看起来好得多。为 Claude 提供查看其输出的工具，以获得最佳结果。

![Safe yolo mode](https://www.anthropic.com/_next/image?url=https%3A%2F%2Fwww-cdn.anthropic.com%2Fimages%2F4zrzovbb%2Fwebsite%2F6ea59a36fe82c2b300bceaf3b880a4b4852c552d-1600x1143.png&w=3840&q=75)
*安全 YOLO 模式*

### d. 安全 YOLO 模式

您可以不监督 Claude，而是使用 `claude --dangerously-skip-permissions` 来绕过所有权限检查，让 Claude 不受打断地工作直到完成。这对于修复 lint 错误或生成模板代码等工作流程非常有效。

让 Claude 运行任意命令是有风险的，可能导致数据丢失、系统损坏，甚至数据泄露（例如，通过提示注入攻击）。为了将这些风险降至最低，请在没有互联网访问的容器中使用 `--dangerously-skip-permissions`。您可以参考此[参考实现](https://github.com/anthropics/claude-code/tree/main/.devcontainer)，使用 Docker Dev Containers。

### e. 代码库问答

当您加入一个新的代码库时，可以使用 Claude Code 进行学习和探索。您可以问 Claude 与您与项目中的另一位工程师进行结对编程时会问的相同类型的问题。Claude 可以智能地搜索代码库来回答一般性问题，例如：

- 日志记录是如何工作的？
- 我如何创建一个新的 API 端点？
- `foo.rs` 第 134 行的 `async move { ... }` 是什么意思？
- `CustomerOnboardingFlowImpl` 处理了哪些边缘情况？
- 为什么我们在第 333 行调用 `foo()` 而不是 `bar()`？
- `baz.py` 第 334 行在 Java 中的等效代码是什么？

在 Anthropic，以这种方式使用 Claude Code 已成为我们的核心入门工作流程，显著提高了上手时间和减轻了其他工程师的负担。无需特殊提示！只需提问，Claude 就会探索代码以找到答案。

![Use Claude to interact with git](https://www.anthropic.com/_next/image?url=https%3A%2F%2Fwww-cdn.anthropic.com%2Fimages%2F4zrzovbb%2Fwebsite%2Fa08ea13c2359aac0eceacebf2e15f81e8e8ec8d2-1600x1278.png&w=3840&q=75)
*使用 Claude 与 git 交互*

### f. 使用 Claude 与 git 交互

Claude 可以有效处理许多 git 操作。许多 Anthropic 工程师使用 Claude 处理 90% 以上的 `git` 交互：

- **搜索 `git` 历史**来回答诸如“v1.2.3 中包含了哪些更改？”、“这个特定功能的所有者是谁？”或“为什么这个 API 是这样设计的？”等问题。明确提示 Claude 查看 git 历史来回答此类查询很有帮助。
- **编写提交消息**。Claude 会自动查看您的更改和近期历史，并考虑到所有相关上下文来撰写提交消息。
- **处理复杂的 git 操作**，例如撤销文件、解决 rebase 冲突以及比较和应用补丁。

这消除了记住 `gh` 命令行语法的需要，同时自动化了常规任务。

### g. 使用 Claude 与 GitHub 交互

Claude Code 可以管理许多 GitHub 交互：

- **创建 pull request**：Claude 理解速记“pr”，并会根据 diff 和周围上下文生成适当的提交消息。
- **为简单的代码审查评论实现一次性解决方案**：只需告诉它修复您的 PR 上的评论（可选地，给予更具体的指令），并在完成后推送到 PR 分支。
- **修复失败的构建**或 linter 警告。
- **通过要求 Claude 遍历开放的 GitHub issues**来分类和分派开放的 issues。

这消除了记忆 `gh` 命令行语法的需要，同时自动化了常规任务。

### h. 使用 Claude 处理 Jupyter notebooks

Anthropic 的研究人员和数据科学家使用 Claude Code 读取和编写 Jupyter notebooks。Claude 可以解释输出，包括图片，提供了一种快速探索和与数据交互的方式。没有强制的提示或工作流程，但我们推荐的一个工作流程是在 VS Code 中同时打开 Claude Code 和一个 .ipynb 文件。

您还可以要求 Claude 在您将其展示给同事之前清理或美化您的 Jupyter notebook。明确告诉它使 notebook 或其数据可视化“具有美感”通常有助于提醒它正在为人类观看体验进行优化。

## 4. 优化您的工作流程

以下建议适用于所有工作流程：

### a. 在您的指令中具体化

Claude Code 的成功率随着指令的更加具体而显著提高，尤其是在首次尝试时。前期给出清晰的指示可以减少后期修正方向的需要。

例如：

|差|好|
|---|---|
|给 foo.py 添加测试|给 foo.py 添加一个新的测试用例，涵盖用户注销的边缘情况。避免使用模拟。|
|ExecutionFactory 的 API 为什么这么奇怪？|查看 ExecutionFactory 的 git 历史并总结其 API 是如何形成的。|
|添加一个日历小部件|查看首页上现有小部件的实现方式，了解其模式以及代码和接口是如何具体分离的。HotDogWidget.php 是一个很好的示例可以先看。然后，遵循该模式实现一个新的日历小部件，允许用户选择月份并前后翻页选择年份。从头开始构建，不使用代码库中已有的库之外的任何库。|

Claude 可以推断意图，但无法读懂您的想法。具体性会更好地与预期对齐。

![Give Claude images](https://www.anthropic.com/_next/image?url=https%3A%2F%2Fwww-cdn.anthropic.com%2Fimages%2F4zrzovbb%2Fwebsite%2F75e1b57a0b696e7aafeca1ed5fa6ba7c601a5953-1360x1126.png&w=3840&q=75)
*给 Claude 图片*

### b. 给 Claude 图片

Claude 在处理图片和图表方面表现出色，可以通过几种方法实现：

- **粘贴截图**（专业提示：在 macOS 中按 `cmd+ctrl+shift+4` 将截图复制到剪贴板，然后按 `ctrl+v` 粘贴。请注意，这与您通常在 Mac 上使用的 `cmd+v` 粘贴不同，并且远程不起作用。）
- **将图片直接拖放到提示输入框中**。
- **提供图片的 文件路径**。

这在处理设计模型作为 UI 开发参考点，以及分析和调试的可视化图表时特别有用。如果您没有将视觉效果添加到上下文，明确告诉 Claude 结果视觉吸引力的重要性仍然会有所帮助。

![Mention files you want Claude to look at or work on](https://www.anthropic.com/_next/image?url=https%3A%2F%2Fwww-cdn.anthropic.com%2Fimages%2F4zrzovbb%2Fwebsite%2F7372868757dd17b6f2d3fef98d499d7991d89800-1450x1164.png&w=3840&q=75)
*提及您希望 Claude 查看或处理的文件*

### c. 提及您希望 Claude 查看或处理的文件

使用 tab 补全快速引用仓库中的任何文件或文件夹，帮助 Claude 找到或更新正确的资源。

![Give Claude URLs](https://www.anthropic.com/_next/image?url=https%3A%2F%2Fwww-cdn.anthropic.com%2Fimages%2F4zrzovbb%2Fwebsite%2Fe071de707f209bbaa7f16b593cc7ed0739875dae-1306x1088.png&w=3840&q=75)
*给 Claude URL*

### d. 给 Claude URL

在提示词旁边粘贴特定 URL，让 Claude 获取并阅读。为避免对相同域（例如 docs.foo.com）的权限提示，使用 `/allowed-tools` 将域添加到您的允许列表中。

### e. 尽早且经常进行修正

虽然自动接受模式（shift+tab 切换）允许 Claude 自主工作，但通常通过积极协作和指导 Claude 的方法可以获得更好的结果。您可以通过在开始时彻底向 Claude 解释任务来获得最佳结果，但您也可以随时修正 Claude。

这四种工具可帮助进行修正：

- **让 Claude 在编码前制定计划**。明确告诉它在您确认计划看起来不错之前不要编码。
- 在任何阶段（思考、工具调用、文件编辑）按下 **Escape 键中断** Claude，保留上下文，以便您可以重定向或扩展指令。
- **双击 Escape 键跳回历史记录**，编辑先前的提示并探索不同的方向。您可以编辑提示并重复，直到获得您想要的结果。
- **要求 Claude 撤销更改**，通常与选项 #2 结合使用以采取不同的方法。

尽管 Claude Code 偶尔会在第一次尝试时完美解决问题，但使用这些修正工具通常能更快地产生更好的解决方案。

### f. 使用 /clear 保持上下文聚焦

在长时间的会话中，Claude 的上下文窗口可能会充满不相关的对话、文件内容和命令。这会降低性能，有时还会分散 Claude 的注意力。在任务之间频繁使用 `/clear` 命令来重置上下文窗口。

### g. 对于复杂工作流程，使用清单和草稿本

对于包含多个步骤或需要详尽解决方案的大型任务（例如代码迁移、修复大量 lint 错误或运行复杂的构建脚本），通过让 Claude 使用 Markdown 文件（甚至是 GitHub issue！）作为清单和工作草稿本来提高性能：

例如，要修复大量 lint 问题，您可以执行以下操作：

1. **告诉 Claude 运行 lint 命令**，并将所有产生的错误（包括文件名和行号）写入 Markdown 清单。
2. **指示 Claude 逐一处理每个问题**，修复并验证后再打勾并继续下一个。

### h. 向 Claude 传递数据

有几种方法可以向 Claude 提供数据：

- **复制并粘贴**直接到您的提示中（最常见的方法）。
- **通过管道输入到 Claude Code 中**（例如，`cat foo.txt | claude`），这对于日志、CSV 和大型数据特别有用。
- **告诉 Claude 通过 bash 命令、MCP 工具或自定义斜杠命令拉取数据**。
- **要求 Claude 读取文件**或获取 URL（也适用于图片）。

大多数会话会结合使用这些方法。例如，您可以管道输入一个日志文件，然后告诉 Claude 使用一个工具拉取额外的上下文来调试日志。

## 5. 使用无头模式自动化您的基础设施

Claude Code 包含[无头模式](https://docs.anthropic.com/en/docs/agents-and-tools/claude-code/overview#automate-ci-and-infra-workflows)，用于非交互式上下文，例如 CI、预提交钩子、构建脚本和自动化。使用 `-p` 标志加上提示来启用无头模式，并使用 `--output-format stream-json` 进行流式 JSON 输出。

请注意，无头模式不会在会话之间持久化。您必须在每次会话中触发它。

### a. 使用 Claude 进行 issue 分类

无头模式可以驱动由 GitHub 事件触发的自动化，例如在您的仓库中创建新 issue 时。例如，公共的 [Claude Code 仓库](https://github.com/anthropics/claude-code/blob/main/.github/actions/claude-issue-triage-action/action.yml) 使用 Claude 在新 issue 进入时对其进行检查并分配适当的标签。

### b. 使用 Claude 作为 linter

Claude Code 可以提供[主观代码审查](https://github.com/anthropics/claude-code/blob/main/.github/actions/claude-code-action/action.yml)，超越传统 linting 工具的检测范围，识别拼写错误、陈旧评论、误导性的函数或变量名等问题。

## 6. 通过多 Claude 工作流程提升水平

除了独立使用，一些最强大的应用涉及并行运行多个 Claude 实例：

### a. 让一个 Claude 编写代码；使用另一个 Claude 进行验证

一个简单但有效的方法是让一个 Claude 编写代码，而另一个对其进行审查或测试。类似于与多个工程师协作，有时分离上下文是有益的：

1. 使用 Claude 编写代码。
2. 运行 `/clear` 或在另一个终端中启动第二个 Claude。
3. 让第二个 Claude 审查第一个 Claude 的工作。
4. 启动另一个 Claude（或再次 `/clear`），阅读代码和审查反馈。
5. 让这个 Claude 根据反馈编辑代码。

您可以使用测试执行类似的操作：让一个 Claude 编写测试，然后让另一个 Claude 编写代码以使测试通过。您甚至可以让您的 Claude 实例相互通信，方法是给它们分配单独的工作草稿本，并告诉它们写入哪个草稿本以及从哪个读取。

这种分离通常比让一个 Claude 处理所有事情产生更好的结果。

### b. 使用多个仓库副本

与其等待 Claude 完成每一步，许多 Anthropic 工程师会这样做：

1. **创建 3-4 个 git 仓库副本**，放在不同的文件夹中。
2. **在单独的终端标签页中打开每个文件夹**。
3. **在每个文件夹中启动 Claude**，分配不同的任务。
4. **循环查看**进度并批准/拒绝权限请求。

### c. 使用 git worktrees

这种方法对于多个独立任务非常有效，提供了比多个副本更轻量级的替代方案。Git worktrees 允许您从同一个仓库将多个分支检出到不同的目录中。每个 worktree 都有自己的工作目录，文件相互隔离，同时共享相同的 Git 历史和 reflog。

使用 git worktrees 可以让您在项目的不同部分同时运行多个 Claude 会话，每个会话专注于自己的独立任务。例如，您可能让一个 Claude 重构您的身份验证系统，而另一个正在构建一个完全不相关的数据可视化组件。由于任务不重叠，每个 Claude 都可以全速工作，无需等待另一个的更改或处理合并冲突：

1. **创建 worktrees**：`git worktree add ../project-feature-a feature-a`
2. **在每个 worktree 中启动 Claude**：`cd ../project-feature-a && claude`
3. 根据需要**创建额外的 worktrees**（在新终端标签页中重复步骤 1-2）。

一些技巧：

- 使用一致的命名约定。
- 每个 worktree 维护一个终端标签页。
- 如果您在 Mac 上使用 iTerm2，[设置通知](https://docs.anthropic.com/en/docs/agents-and-tools/claude-code/overview#notification-setup)，以便在 Claude 需要注意时收到提醒。
- 为不同的 worktrees 使用单独的 IDE 窗口。
- 完成后清理：`git worktree remove ../project-feature-a`

### d. 使用无头模式与自定义 Harness

`claude -p`（无头模式）将 Claude Code 以编程方式集成到更大的工作流程中，同时利用其内置工具和系统提示。使用无头模式有两种主要模式：

1. **扇出（Fanning out）**处理大型迁移或分析（例如，分析数百个日志中的情感或分析数千个 CSV）：

2. 让 Claude 编写一个脚本来生成任务列表。例如，生成一个需要从框架 A 迁移到框架 B 的 2k 个文件列表。
3. 循环处理任务，为每个任务以编程方式调用 Claude，并给它一个任务和一组它可以使用的工具。例如：`claude -p “migrate foo.py from React to Vue. When you are done, you MUST return the string OK if you succeeded, or FAIL if the task failed.” --allowedTools Edit Bash(git commit:*)”`
4. 多次运行脚本并优化您的提示词以获得所需的结果。

5. **流水线（Pipelining）**将 Claude 集成到现有的数据/处理流水线中：

6. 调用 `claude -p “<您的提示>” --json | your_command`，其中 `your_command` 是您处理流水线的下一步。
7. 就这样！JSON 输出（可选）可以帮助提供结构，以便更轻松地进行自动化处理。

对于这两种用例，使用 `--verbose` 标志有助于调试 Claude 调用。我们通常建议在生产环境中关闭 verbose 模式，以获得更清晰的输出。

您在使用 Claude Code 方面有哪些技巧和最佳实践？请标记 @AnthropicAI，以便我们了解您正在构建什么！

## 致谢

作者：Boris Cherny。本文借鉴了更广泛的 Claude Code 用户社区的最佳实践，他们的创新方法和工作流程不断激励着我们。特别感谢 Daisy Hollman、Ashwin Bhat、Cat Wu、Sid Bidasaria、Cal Rueb、Nodir Turakulov、Barry Zhang、Drew Hodun 以及许多其他 Anthropic 工程师，他们宝贵的见解和使用 Claude Code 的实践经验帮助形成了这些建议。