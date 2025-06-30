

## Introduction

### What is Amp?

Amp is an agentic coding tool built by [Sourcegraph](https://sourcegraph.com). It runs in [VS Code](https://marketplace.visualstudio.com/items?itemName=sourcegraph.amp) (and compatible forks like Cursor, Windsurf, and VSCodium) and as a [command-line tool](https://www.npmjs.com/package/@sourcegraph/amp). It’s also multiplayer — you can share threads and collaborate with your team.

### Principles

1. Amp is unconstrained in token usage (and therefore cost). Our sole incentive is to make it valuable, not to match the cost of a subscription.
2. No model selector, always the best models. You don’t pick models, we do. Instead of offering selectors and checkboxes and building for the lowest common denominator, Amp is built to use the full capabilities of the best models.
3. We assume that you want to access the raw power these models have to offer. In a sense, when you’re using Amp, you aren’t using Amp — you’re talking directly to a model and Amp is the shell around your conversation with the model.
4. Built to change. Products that are overfit on the capabilities of today’s models will be obsolete in a matter of months.

## Getting Started

Sign in to [ampcode.com](https://ampcode.com) and follow the instructions to install Amp in [VS Code](https://marketplace.visualstudio.com/items?itemName=sourcegraph.amp) (or compatible forks like Cursor, Windsurf, and VSCodium) and the [CLI](https://www.npmjs.com/package/@sourcegraph/amp).

## Using Amp

### How to Prompt

Amp currently uses Claude Sonnet 4 for most tasks. For the best results, follow these guidelines:

- Be explicit with what you want. Don’t try to make the model guess.
- In Amp, you need to press Cmd/Ctrl+Enter to submit a message, not just Enter, to remind you to be deliberate with your requests.
- Break very large tasks up into smaller sub-tasks, one per thread.
- Use a project `AGENT.md` file to guide Amp on how to run your tests and build steps and to avoid doing inappropriate things.

Here are some examples of prompts we’ve used with Amp:

- “Look at src/my/file.ext and extend it so that it sends the requests only every 200ms. Add tests in the existing test file.”
- “Run `<build command>` and fix all the errors”
- “Look at `<local development server url>` to see this UI component. Then change it so that it looks more minimal. Frequently check your work by screenshotting the URL.”
- “Run git blame on the file I have open and figure out who added that new title”
- “Run `git diff` to see the code someone else wrote; review the code thoroughly and point out any potential edge cases that were missed”
- “Run `git diff` to see the current changes, remove debug statements”
- “Find the commit that added this using git log, look at the whole commit, then help me change this feature”
- “Explain the relationship between class AutoScroller and ViewUpdater using a diagram”
- “Use `psql` to connect to my local database, then rewire all uploads in the image uploads table to be owned by my user, [bob@example.com](mailto:bob@example.com)”

Also see Thorsten Ball’s [How I Use Amp](https://ampcode.com/how-i-use-amp).

If you’re on a team, use Amp’s [thread sharing](https://ampcode.com/manual#teams) to learn from each other.

### `AGENT.md`

An `AGENT.md` file in your workspace gives Amp information about your project’s codebase structure, development practices, and coding standards. Amp offers generate an `AGENT.md` for you if none exists.

_Planned: Support for scoped `AGENT.md` files in subdirectories and other more granular agent guidance._

### Uploading Images

Amp supports image uploads, allowing you to share screenshots, diagrams, and visual references with the AI. Images can provide important context for debugging visual issues or understanding UI layouts.

To upload images, you can:

- Copy and paste directly into the input area
- Hold Shift while dragging files over the input area

### Mentioning Files

You can mention files directly in your prompts by typing @ followed by a pattern to fuzzy-search. It can help speed up responses by avoiding the need to search the codebase.

### Shortcuts

Amp uses different shortcuts depending on the operating system and editor you’re using.

Operating System:

Editor:

|Command|Shortcut|
|---|---|
|New Thread|CmdL|
|Toggle Agent Visibility|CmdI|
|Go to Next Thread|CmdShift]|
|Go to Previous Thread|CmdShift[|

## Threads

Threads are conversations with the agent, containing all your messages, context, and tool calls. Your threads are synced to ampcode.com. If you’re on a team, your threads are also shared with your team by default, just like Git branches on a shared remote repository.

Including links to Amp threads with your changes when submitting for code review helps provide context. Reading and searching your team’s threads can help you see what’s going on and how other people are using Amp.

### Privacy & Permissions

Threads can be public (visible to anyone on the internet with the link), team-shared (visible to your team members), or private (visible only to you).

If you’re on a team, your threads are shared by default with your team members.

If you are not on a team, your threads are only visible to you by default.

You can change a thread’s visibility at any time through the

sharing menu at the top of the thread.

### Managing Context

As you work with Amp, your thread accumulates context within the model’s context window. Amp shows your context window usage and warns when approaching limits.

When approaching the thread context limit, you can hover over the context window indicator and use the following:

- Compact Thread — Summarizes the existing conversation to reduce context usage while preserving important information
- New Thread with Summary — Creates a new thread that starts with a summary of the current conversation

### File Changes

Amp tracks changes that the agent makes to files during your conversation, which you can track and revert:

- Hover over the files changed indicator (located just above the message input) to see which files were modified and by how much
- Revert individual file changes, or all changes made by the agent

Editing a message in a thread automatically reverts any changes the agent made after that message

## Amp Tab

Amp Tab is our new in-editor completion engine, designed to anticipate your next actions and reduce the time spent manually writing code.

It uses a custom model that was trained to understand what you are trying to do next, based on your recent changes, your language server’s diagnostics, and what we call semantic context.

Amp Tab can suggest regular single or multi-line edits to change entire code blocks, next to your cursor or farther away, somewhere else in your current document.

### Enabling

Enable Amp Tab by adding the the following to your VS Code settings:

```json
{
	"amp.tab.enabled": true
}
```

### How to Use

- Begin typing in your editor. Amp Tab automatically presents relevant suggestions.
- Press the Tab key to accept and apply the suggested edits.
- Press the Tab key again to instantly jump to additional edits further from your cursor.
- To ignore suggestions, simply continue typing or press Esc.

Currently, Amp Tab is freely available as a research preview to all Amp users.

## Teams

Teams provide collaborative workspaces where knowledge can be shared across your organization. Create a team from the [settings page](https://ampcode.com/settings). To join a team, you need an invitation from an existing team member.

### Sharing

Team threads are visible to all team members by default, making it easy to learn from others and build on their work.

### Team Usage

Teams provide pooled billing of usage, making it easier to manage costs across your organization. If a member of your team joins with free personal usage available, their free usage will be used before the paid team usage.

### Leaderboard

Each team includes a leaderboard that tracks thread activity and contributions from team members, encouraging engagement and highlighting active participants.

## Tools

Tools are what the underlying model uses to assist with tasks. For the highest quality results we recommend you use a curated set of tools, with prompts adjusted to fit the underlying model.

### Built-in Tools

Amp comes with a curated set of built-in tools specifically designed for coding. You can find the list of built-in tools inside Amp’s extension settings.

### Custom Tools

You can extend Amp’s capabilities through the Settings interface by adding MCP servers. These servers provide additional tools for specific needs. For best results, use MCP servers that expose a small number of high-level tools with high-quality descriptions.

#### JetBrains

You can connect the Amp CLI or VS Code extension to JetBrains IDEs using MCP. This gives Amp access to JetBrains IDE diagnostics, which help the the agent iterate against compiler errors and other information provided by the JetBrains IDE.

To use Amp with JetBrains IDEs:

1. Install the [JetBrains MCP Server plugin](https://plugins.jetbrains.com/plugin/26071-mcp-server) into the JetBrains IDE. Ensure the JetBrains IDE is running with the plugin installed.
    
2. Add `npx -y @jetbrains/mcp-proxy` as an MCP server to Amp. In VS Code, you can add this in the MCP Servers settings panel in the editor or add the following to VS Code settings. In the CLI, add the following to your [configuration file](https://ampcode.com/manual#configuration-paths):
    
    ```json
    "amp.mcpServers": {
        "jetbrains": {
            "command": "npx",
            "args": ["-y", "@jetbrains/mcp-proxy"]
        }
    }
    ```
    

### Command Allowlisting

Amp has a built-in safety system specifically for terminal commands that determines which commands require explicit permission before execution.

By default, Amp automatically allows certain read-only and safe commands like `ls`, `cat`, and `git status`. Common development commands like `go test`, `cargo build`, and `pnpm run build` are also pre-approved. For all other commands, Amp will prompt for permission before execution to protect your system.

You can configure Amp to execute additional commands without prompting for permission each time by adding them to the `"amp.commands.allowlist"` array in your extension or CLI settings:

```json
"amp.commands.allowlist": [
    "pnpm exec tsc --build",
    "pnpm -C web check",
    "pnpm -C server test"
]
```

Both the Amp extension and CLI use this same setting format. You can use simple command patterns like `make build` or wildcards like `npm run * --test` to allow multiple similar commands.

## Configuration

Amp can be configured through settings in VS Code (`.vscode/settings.json`) and the CLI configuration file. All settings use the `amp.` prefix.

### CLI Configuration Paths

The CLI configuration file location varies by operating system:

Windows `path`

%APPDATA%\amp\settings.json

Example:

`C:\Users\USERNAME\AppData\Roaming\amp\settings.json`

macOS `path`

~/.config/amp/settings.json

Example:

`/Users/USERNAME/.config/amp/settings.json`

Linux `path`

~/.config/amp/settings.json

Example:

`/home/USERNAME/.config/amp/settings.json`

### Corporate Networks

The Amp CLI supports proxy servers and custom certificates commonly required in corporate environments through standard Node.js environment variables:

HTTP_PROXY `environment variable`

HTTP proxy server URL for non-HTTPS requests

Example:

`http://proxy.company.com:8080`

HTTPS_PROXY `environment variable`

HTTPS proxy server URL for HTTPS requests

Example:

`https://proxy.company.com:8080`

NODE_EXTRA_CA_CERTS `environment variable`

Path to additional CA certificates file for custom/internal CAs

Example:

`/path/to/company-ca-bundle.pem`

These environment variables are automatically respected by the CLI’s HTTP client without requiring additional configuration. Set them in your shell profile or CI environment as needed.

> **Note:** This configuration is not needed for Visual Studio Code (and compatible forks like Cursor, Windsurf, and VSCodium) as they handle corporate network settings automatically.

### Core Settings

amp.url `string`

VS Code & CLI

URL to the Amp server, usually `https://ampcode.com/`

Example:

`https://ampcode.com/`

amp.notifications.enabled `boolean` `default: true`

VS Code

Play notification sound when done or blocked

amp.anthropic.thinking.enabled `boolean` `default: true`

VS Code & CLI

Enable Claude's extended thinking capabilities

amp.todos.enabled `boolean` `default: true`

VS Code & CLI

Enable TODOs tracking for managing tasks

amp.tools.disable `array` `default: "[]"`

VS Code & CLI

Disable specific tools by name. Use 'builtin:toolname' to disable only the builtin tool with that name (allowing an MCP server to provide a tool by that name).

Example:

`["read_file", "create_file", "edit_file", "undo_edit", "list_directory", "glob", "format_file", "Grep", "codebase_search", "Bash", "read_web_page", "web_search", "get_diagnostics", "think", "mermaid", "todo_write", "todo_read", "Task", "run_routine", "builtin:edit_file"]`

amp.tools.stopTimeout `number` `default: 300`

VS Code & CLI

How many seconds to wait before canceling a running tool

amp.debugLogs `boolean` `default: false`

VS Code

Enable debug logging in the Amp output channel

### Terminal & Environment

amp.terminal.commands.hide `boolean` `default: true`

VS Code

Whether to hide the integrated VS Code terminal by default when starting commands

amp.terminal.commands.environment `string` `default: "vscode-terminal"`

VS Code & CLI

What environment to use when running terminal commands

Options: `vscode-terminal`,`node-spawn`

amp.terminal.commands.vscodeTerminal.detachTimeout `number` `default: 90`

VS Code

How many seconds to wait before detaching a running command to continue the conversation. The command continues to run in the background. This setting only has an effect when using the `vscode-terminal` environment

amp.terminal.commands.nodeSpawn.loadProfile `string` `default: "always"`

VS Code & CLI

Before running commands (including MCP servers), whether to load environment variables from the user's profile (`.bashrc`, `.zshrc`, `.envrc`) as visible from the workspace root directory

Options: `always`,`never`,`daily`

### Advanced Settings

amp.mcpServers `object`

VS Code & CLI

Model Context Protocol servers that expose tools. See [Custom Tools documentation](https://ampcode.com/manual#custom-tools).

amp.commands.allowlist `array` `default: "[]"`

VS Code & CLI

Run specific terminal commands without waiting for user confirmation. See [Command Allowlisting documentation](https://ampcode.com/manual#terminal-command-allowlisting).

Example:

`["pnpm exec tsc --build", "pnpm -C web check", "pnpm -C server test"]`

## Account

### Security

See the [Amp Security Reference](https://ampcode.com/security) document.

### Support & Community

Join the [Amp Discord](https://ampcode.com/discord) to connect with the Amp team and other Amp users, share tips and tricks, and get help from the community.

For billing questions, contact [amp-billing-help@sourcegraph.com](mailto:amp-billing-help@sourcegraph.com).

## Pricing

### Usage

Upon signing up, most users get $10 USD in free usage. You can purchase more as an individual or for your team. Unused credits expire after one year of account inactivity.

Usage is consumed based on LLM usage and usage of certain other tools (like web search) that cost us to serve. We pass these costs through to you directly with no markup, for individuals and non-enterprise teams.

### Enterprise

Enterprise usage is 50% more expensive than individual and team usage, and includes SSO (Okta, SAML, etc.) and zero data retention for text inputs in LLM inference. See [Amp Security Reference](https://ampcode.com/security) for more information.

To start using Amp Enterprise, go to [your team](https://ampcode.com/team) and click “Upgrade to Enterprise” under “Team Usage”. This requires a special one-time $1,000 USD purchase, which grants your team $1,000 USD of Amp Enterprise usage and upgrades your team to Enterprise.

With Amp Enterprise Premium, invoice payments are offered for purchases of $5,000+ USD, and volume discounts are available for purchases of $25,000+ USD. Contact [amp-devs@sourcegraph.com](mailto:amp-devs@sourcegraph.com) for access to these purchasing options and for general information about Amp Enterprise.

## Appendix

### Share Thread with Support

We may ask you to share your thread with authorized Sourcegraph staff members to help diagnose quality issues:

1. In the Amp sidebar in VS Code or when viewing the thread on ampcode.com, open the

- sharing menu.
- Select

1. Share Thread with Support.

You can also share your thread via the CLI:

```bash
amp threads share --support <thread-id>
```

This will allow authorized Sourcegraph staff members to view your thread for debugging purposes.

### Support Bundles

We may ask you to generate a support bundle and share it directly with authorized Sourcegraph staff members to help diagnose quality issues. You can email support bundles to [amp-devs@sourcegraph.com](mailto:amp-devs@sourcegraph.com).

**To generate a support bundle:**

1. Open your terminal
2. Run `npx @sourcegraph/amp doctor`
3. The bundle will be saved as a timestamped `.json.gz` file in your current directory

**What’s included in a support bundle:**

- **System Information**: Operating system, hardware specs, Node.js version, available memory and disk space
- **Amp Installation**: Version detection, installation method (npm/pnpm/yarn), package manager, recent logs (last 1000 entries)
- **Network Diagnostics**: Connectivity tests to Amp services, DNS resolution, proxy configuration detection
- **SSL Analysis**: Certificate chains, trusted root certificates, TLS configuration for corporate environments
- **Environment Variables**: Only variables with the `AMP_` prefix

Support bundles are automatically redacted using Amp’s [built-in secret detection patterns](https://ampcode.com/security#secret-redaction) but we recommend manually reviewing the information before sharing support bundles as log files gathered may contain sensitive information.

### Visual Studio Code Developer Console

We may ask you to share information from your Visual Studio Code Developer Console.

**To open the Developer Console:**

**macOS:**

- Press `Cmd+Shift+P` to open the Command Palette
- Type “Developer: Toggle Developer Tools” and press Enter
- Or use the keyboard shortcut: `Cmd+Option+I`

**Windows:**

- Press `Ctrl+Shift+P` to open the Command Palette
- Type “Developer: Toggle Developer Tools” and press Enter
- Or use the keyboard shortcut: `Ctrl+Shift+I`

**Linux:**

- Press `Ctrl+Shift+P` to open the Command Palette
- Type “Developer: Toggle Developer Tools” and press Enter
- Or use the keyboard shortcut: `Ctrl+Shift+I`

The Developer Console will open as a separate window or panel, showing the Console, Network, and other debugging tabs that can help authorized Sourcegraph staff members diagnose quality issues.

### Service Status

Check [ampcodestatus.com](https://ampcodestatus.com) for service status and to sign up for alerts via email, RSS, Slack. Alternatively, follow [@ampcodestatus](https://x.com/ampcodestatus) on X.

### News

Follow Amp's [News](https://ampcode.com/news) for the changelog and other updates from the Amp team.

### Frequently Ignored Feedback

See Amp's [Frequently Ignored Feedback](https://ampcode.com/fif) for the most common valid feedback that we've chosen to not address.