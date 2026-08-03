<div align="center">

# ⚡ PyCode

### 🖥️ AI-powered coding assistant in your terminal

**Chat with LLMs, run tools, and write code — all without leaving your command line.**

[![Website](https://img.shields.io/badge/🌐_Website-pycode.kozow.com-6366f1)](https://pycode.kozow.com/)
[![WhatsApp](https://img.shields.io/badge/💬_WhatsApp-@hellocodelinux-25D366)](https://wa.me/5491112345678)
[![Email](https://img.shields.io/badge/📧_Email-hellocodelinux@gmail.com-EA4335)](mailto:hellocodelinux@gmail.com)

---

🚀 **Lightweight** • 🎨 **Beautiful** • 🔧 **Powerful** • 🆓 **Free**

</div>

---

<div align="center">

## 📥 Download & Project

### 🌐 **Website:** [pycode.kozow.com](https://pycode.kozow.com/)

### 📦 **Binary available on the website**

</div>

---

## ✨ Features

### 🧠 Core

| Feature | Description |
|---------|-------------|
| 🔀 **Build / Plan / Chat Modes** | Full access, read-only, or web search only — switch with `Ctrl+B`. Chat mode uses only web tools for conversational queries. |
| 💬 **Chat Sessions** | Persistent conversations with history. Revisit, rename, or delete anytime. |
| 📦 **Context Compaction** | Auto-summarizes when context fills. Preserves decisions, file changes, and tasks. |
| 🎨 **Theme Picker** | Multiple built-in themes, switchable at runtime (`Ctrl+P`). |
| 🤖 **Model Picker** | Fetch and switch models on the fly (`Ctrl+O`). Auto-detects free models. |

### 🛠️ Tools

| Tool | Description |
|------|-------------|
| 📝 `bash` | Execute shell commands |
| 📄 `read` | Read file contents |
| ✏️ `write` | Write/create files |
| 🔍 `edit` | Edit files with exact string replacement |
| 📁 `glob` | Find files by glob pattern |
| 🔎 `grep` | Search file contents with regex |
| 🩹 `apply_patch` | Apply aider-style patches |
| 🌐 `webfetch` | Fetch and extract text from a URL |
| 🔍 `websearch` | Search the web for current information |
| ✅ `todowrite` | Create and manage a structured task list |
| ❓ `question` | Ask the user a multiple-choice question |
| 🤖 `task` | Spawn sub-agents for delegated research |
| 🏷️ `set_title` | Set session title (auto-generated) |

### 🎯 UI & Experience

| Feature | Description |
|---------|-------------|
| 🎨 **Beautiful TUI** | Powered by [Textual](https://textual.textualize.io/). Rich colors, themes, responsive. |
| 📊 **Context Usage Bar** | Real-time token usage and percentage in the status bar. |
| 🧠 **Reasoning Display** | Shows model "thinking" process with elapsed time. |
| 📊 **Diff Rendering** | Colored diffs for `apply_patch` results. |
| 🕘 **Persistent Input History** | Your previous prompts are saved to disk and recalled in any new session with `↑/↓`. |
| ⚙️ **Settings Modal** | Configure API endpoint, key, and model (`Ctrl+S`). |
| ❓ **Help Screen** | Keyboard shortcuts reference (`F1`). |
| 📋 **Copy Messages** | Copy assistant responses to clipboard (`Ctrl+Y`). |
| 🛡️ **Error Dialogs** | Friendly handling for rate limits, auth failures, server errors. |

### 🤖 Agents

| Agent | Type | Description |
|-------|------|-------------|
| `build` | Primary | Default agent — full tool access, executes commands and edits files. |
| `plan` | Primary | Read-only agent — cannot edit files or run commands. Good for analysis. |
| `explore` | Subagent | Fast codebase exploration — finds files, searches code, answers questions about structure. |
| `general` | Subagent | General-purpose research and multi-step task execution. |

Agents are used by the `task` tool to delegate work to specialized sub-agents. Primary agents (`build`, `plan`) are selectable via `Ctrl+B`. Sub-agents (`explore`, `general`) are spawned automatically when the model uses the `task` tool.

### 🔧 Advanced

| Feature | Description |
|---------|-------------|
| 🌐 **Web Browser Mode** | Run `pycode web` to serve the TUI in your browser via [textual-serve](https://github.com/Textualize/textual-serve). |
| 💻 **CLI Subcommands** | `pycode` (TUI), `pycode web` (browser), `pycode run TEXT` (one-shot), `pycode help` (version + usage). |
| 🔁 **Session Resume** | `pycode -s SESSION_ID` resumes a previous session by ID. |
| 🔍 **Auto Update Check** | `pycode help` checks for newer versions and shows an update notice. |
| 🔄 **Models.dev Integration** | Auto-fetches real context windows from models.dev catalog. |
| 🌐 **Proxy Support** | Respects `HTTPS_PROXY` / `HTTP_PROXY` / `ALL_PROXY` (upper or lower case) and honors `NO_PROXY` — applied only to the LLM API. |
| 📬 **Message Queue** | Type while the model is processing — messages are queued automatically. |
| ⚡ **Non-blocking Tools** | All tools execute in background threads. UI stays responsive. |
| 📁 **File References** | Reference files with `@path` — PyCode reads them on demand. |
| 🖥️ **Shell Integration** | Run shell commands inline with `!command` or `/shell command`. |

---

## 🚀 Quick Start

### 📦 Install (Linux x86_64)

```bash
curl -L https://pycode.kozow.com/bin/pycode -o pycode && chmod +x ./pycode
```

### ▶️ Run

```bash
./pycode                  # 🖥️  Start the TUI
./pycode -s SESSION_ID    # 🔁  Resume a previous session
./pycode web              # 🌐  Serve in browser
./pycode web --port 8080  # 🌐  Serve on custom port
./pycode help             # ℹ️  Show version and usage
./pycode run TEXT         # 🚀  One-shot prompt
```

---

## ⌨️ Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| `Ctrl+C` | Quit |
| `Ctrl+N` | New session |
| `Ctrl+L` | Clear chat |
| `Ctrl+R` | Session picker |
| `Ctrl+B` | Cycle mode: build/plan/chat |
| `Ctrl+S` | Settings dialog |
| `Ctrl+P` | Theme picker |
| `Ctrl+O` | Model picker |
| `Ctrl+Y` | Copy message to clipboard |
| `F1` | Help screen |
| `Escape` | Stop generation / abort |
| `PageUp/PageDown` | Scroll chat |
| `@` (in input) | File picker |
| `!command` (in input) | Run shell command |
| `↑/↓` (in input) | Recall input history (persistent across sessions) |

---

## 🤖 Models

### Free Models (No API key needed)

PyCode works out of the box with [OpenCode Zen](https://opencode.ai/zen) and **auto-detects all the free models** available on the endpoint (`Ctrl+O` to pick). The default is `mimo-v2.5-free`. Real context windows are pulled from the [models.dev](https://models.dev/) catalog.

| Model | Description |
|-------|-------------|
| 🧠 `mimo-v2.5-free` | Balanced performance (default) |
| ⚡ `deepseek-v4-flash-free` | Fast and efficient |
| 🔍 `ling-3.0-flash-free` | Fast language model |
| 💡 `nemotron-3-ultra-free` | Advanced capabilities |
| 🚀 `north-mini-code-free` | Optimized for code |
| 🌊 `laguna-s-2.1-free` | Lightweight and fast |
| 🌐 [Exa](https://exa.ai/) | Web search — also **free** |

### Bring Your Own API

PyCode works with any OpenAI-compatible API. Configure via `Ctrl+S` or edit `~/.config/pycode-tui/config.json`:

- **OpenAI** — set API URL to `https://api.openai.com/v1`
- **Anthropic** — via [LiteLLM](https://github.com/BerriAI/litellm) proxy
- **Ollama** — set API URL to `http://localhost:11434/v1`
- **OpenCode Zen** — default, free models included

---

## 📊 System Requirements

| Requirement | Details |
|-------------|---------|
| 🖥️ **OS** | Linux (x86_64) |
| 🧠 **RAM** | ~80 MB (process: ~2 MB CLI + ~78 MB core) |
| 📦 **Binary** | ~25 MB (x86_64) |
| 💽 **Disk** | ~40 MB (25 MB binary + ~15 MB config/cache) |
| ⚡ **CPU** | Any x86_64 processor (~1% idle, ~5% during inference) |
| 📜 **License** | Proprietary |

---

## ⚙️ Configuration

| Path | Description |
|------|-------------|
| `~/.config/pycode-tui/config.json` | API URL, API key, model, theme |
| `~/.config/pycode-tui/sessions/` | Session history (JSON) |
| `~/.config/pycode-tui/prompt-history.jsonl` | Input history (persistent across sessions) |
| `~/.cache/pycode-tui/models-dev.json` | Model catalog cache (7-day TTL) |

### Environment Variables

| Variable | Description |
|----------|-------------|
| `HTTPS_PROXY` / `https_proxy` | Proxy for HTTPS requests (LLM API only) |
| `HTTP_PROXY` / `http_proxy` | Proxy for HTTP requests (LLM API only) |
| `ALL_PROXY` / `all_proxy` | Fallback proxy for any scheme (LLM API only) |
| `NO_PROXY` / `no_proxy` | Hosts excluded from the proxy |
| `SSL_CERT_FILE` | Custom CA certificate bundle |
| `TEXTUAL_DRIVER` | Textual driver override |

---

## 📜 License

**PyCode is a closed-source, proprietary application.** It is distributed as a ready-to-run binary and is free to use, but the source code is not published and may not be redistributed or modified.

---

## 🙏 Credits

Inspired by [OpenCode](https://opencode.ai/) — an AI-powered coding assistant for the terminal.

---

## 📞 Contact

| Channel | Link |
|---------|------|
| 🌐 **Website** | [pycode.kozow.com](https://pycode.kozow.com/) |
| 📧 **Email** | [hellocodelinux@gmail.com](mailto:hellocodelinux@gmail.com) |
| 💬 **WhatsApp** | [@hellocodelinux](https://wa.me/5491112345678) |

---

<div align="center">

**Made with ❤️ for terminal lovers**

© 2026 PyCode

</div>
