🌍 [English](README.md) | [Türkçe](README.tr.md) | [Español](README.es.md)

# 🤖 Claude Code — General User Guide

> **The terminal-based coding assistant developed by Anthropic that runs in your local shell.**

<div align="center">

![Version](https://img.shields.io/badge/version-latest-blue)
![License](https://img.shields.io/badge/license-Proprietary-red)
![Platform](https://img.shields.io/badge/platform-Anthropic%20Claude-darkgreen)

**⭐ Write, edit, and navigate code directly from your terminal.**

</div>

---

## 📚 Table of Contents

- [What is Claude Code?](#what-is-claude-code)
- [Installation](#installation)
- [Getting Started](#getting-started)
- [Interactive Mode (TUI)](#interactive-mode-tui)
- [Configuration](#configuration)
- [Slash Commands](#slash-commands)
- [Essential Keyboard Shortcuts](#essential-keyboard-shortcuts)
- [Tips & Tricks](#tips--tricks)
- [Resources](#resources)
- [Quick Reference Card](#quick-reference-card)

---

## What is Claude Code?

**Claude Code** is a developer-centric command-line interface (CLI) tool created by Anthropic. It allows you to interact with Claude directly inside your terminal to write, edit, and refactor code, inspect files, run terminal commands, and perform Git operations.

Claude Code runs in your local workspace and has access to shell tools, enabling it to execute commands and modify code directly with your permission.

---

## Installation

Install the Claude Code CLI globally depending on your operating system:

### 🪟 Windows (PowerShell)
```powershell
irm https://claude.ai/install.ps1 | iex
```

### 🍎 macOS / 🐧 Linux
```bash
curl -fsSL https://claude.ai/install.sh | bash
```

### 🪟 Windows (Command Prompt / CMD)
```cmd
curl -fsSL https://claude.ai/install.cmd -o install.cmd && install.cmd && del install.cmd
```

### 🪟 Windows (WinGet)
```powershell
winget install Anthropic.ClaudeCode
```

---

## Getting Started

### 1. Launch the TUI

To start an interactive session with Claude Code in your current directory, run:

```bash
claude
```

### 2. Enter Your Prompts

Describe the task you want Claude Code to perform:

```
> Create a unit test file for auth.js
> Find all occurrences of the deprecated api endpoint and replace them
> Build the project and tell me if there are any linting issues
```

### 3. Exit the Session

To exit the interactive session:
* Type `/quit` or `/exit` in the prompt box.
* Or press **Ctrl+D** in the terminal.

---

## Interactive Mode (TUI)

### prompt box features

- **Reference Files:** Type `@` followed by a file name to search and inject the file contents into the agent's context.
- **Insert a Newline:** Press `Ctrl+J` inside the prompt box to start a new line without submitting the prompt.

---

## Configuration

You can customize the behavior, models, and safety profiles of Claude Code.

- **Configure Settings:** Type `/config` inside the TUI to open the settings interface.
- **Change Settings Directly:** Run `/config key=value` (e.g. `/config theme=light`) to modify settings instantly.

---

## Slash Commands

Type `/` in the prompt box to open the command menu, or `/help` to see the full list of options.

| Command | Description |
|---------|-------------|
| `/new` | Clear the prompt area and start a new session |
| `/clear` | Wipe current conversation history and start fresh |
| `/compact` | Compress conversation history to save context window tokens |
| `/model <name>`| Switch active model mid-session |
| `/config` | Manage settings and configuration options |
| `/quit` | Exit Claude Code |

---

## Essential Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| **Ctrl + C** | Interrupt current operation / clear input (first press), exit (second press) |
| **Ctrl + D** | Exit the active session |
| **Ctrl + G** | Open the current prompt in your default external text editor |
| **Ctrl + J** | Insert a newline in the editor without submitting |
| **Ctrl + L** | Redraw the terminal screen |
| **Ctrl + O** | Toggle the transcript viewer (shows tool usage details) |
| **Ctrl + R** | Reverse search command history |

---

## Tips & Tricks

- **One-Shot Mode:** Run a prompt directly from your terminal shell and exit immediately after execution:
  ```bash
  claude "Summarize the changes in the latest git commit"
  ```
- **Session Resuming:** If you exit a session, you can resume it using:
  ```bash
  claude --resume <session-id>
  ```
- **Option Key (macOS):** For keyboard shortcuts using the Option/Alt key on macOS, ensure your terminal is set up to treat Option as "Meta" (e.g., in iTerm2 keys profile settings).

---

## Resources

- **Official Documentation:** [docs.anthropic.com](https://docs.anthropic.com)
- **Anthropic Claude Home:** [claude.ai](https://claude.ai)

---

## Quick Reference Card

```
┌──────────────────────────────────────────────────────────┐
│                🤖 Claude Code Quick Reference            │
├──────────────────────────────────────────────────────────┤
│                                                          │
│  START                     MANAGE                        │
│  claude          .......  Launch TUI      /new           │
│  claude "..."    .......  With prompt     /clear         │
│  claude --resume .......  Resume          /compact       │
│                                           /quit          │
│                                                          │
│  EDITOR                    KEYBINDINGS                   │
│  Ctrl+J          .......  New line        Ctrl+C         │
│  Ctrl+G          .......  External edit   Ctrl+D         │
│  Ctrl+R          .......  Search history  Ctrl+O         │
│                                           Ctrl+L         │
│                                                          │
│  CONFIG                                                  │
│  /config         .......  Settings Panel                 │
│  /model          .......  Change model                   │
│                                                          │
└──────────────────────────────────────────────────────────┘
```

---

> **Claude Code** — Proprietary — Developed with ❤️ by Anthropic
