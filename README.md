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

## ✨ Features

### 🧠 Core

| Feature | Description |
|---------|-------------|
| 🔀 **Build / Plan Modes** | Full access or read-only — switch with `Ctrl+B`. Plan mode injects system reminders so the LLM only plans. |
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
| 🩹 `apply_patch` | Apply unified diff-style patches |
| 🌐 `webfetch` | Fetch and extract text from a URL |
| 🔍 `websearch` | Search the web for current information |
| ✅ `todowrite` | Create and manage a structured task list |
| ❓ `question` | Ask the user a multiple-choice question |

### 🎯 UI & Experience

| Feature | Description |
|---------|-------------|
| 🎨 **Beautiful TUI** | Powered by [Textual](https://textual.textualize.io/). Rich colors, themes, responsive. |
| 📊 **Context Usage Bar** | Real-time token usage and percentage in the status bar. |
| 🧠 **Reasoning Display** | Shows model "thinking" process with elapsed time. |
| 📊 **Diff Rendering** | Colored diffs for `apply_patch` results. |
| ⚙️ **Settings Modal** | Configure API endpoint, key, and model (`Ctrl+S`). |
| ❓ **Help Screen** | Keyboard shortcuts reference (`F1`). |
| 📋 **Copy Messages** | Copy assistant responses to clipboard (`Ctrl+Y`). |
| 🛡️ **Error Dialogs** | Friendly handling for rate limits, auth failures, server errors. |

### 🔧 Advanced

| Feature | Description |
|---------|-------------|
| 🌐 **Web Browser Mode** | Run `pycode web` to serve the TUI in your browser via [textual-serve](https://github.com/Textualize/textual-serve). |
| 💻 **CLI Subcommands** | `pycode` (TUI), `pycode web` (browser), `pycode run TEXT` (one-shot), `pycode help` (version + usage). |
| 🔍 **Auto Update Check** | `pycode help` checks for newer versions and shows an update notice. |
| 🔄 **Models.dev Integration** | Auto-fetches real context windows from models.dev catalog. |
| 🌐 **Proxy Support** | Respects `HTTPS_PROXY` / `HTTP_PROXY` environment variables. |
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
./pycode           # 🖥️  Start the TUI
./pycode web       # 🌐  Serve in browser
./pycode help      # ℹ️  Show version and usage
./pycode run TEXT  # 🚀  One-shot prompt
```

---

## 🤖 Free Models Included

No API key needed! PyCode ships pre-configured with **5 free models** from [OpenCode Zen](https://opencode.ai/zen):

| Model | Description |
|-------|-------------|
| 🧠 `hy3-free` | High-quality reasoning |
| ⚡ `deepseek-v4-flash-free` | Fast and efficient |
| 🔍 `mimo-v2.5-free` | Balanced performance |
| 💡 `nemotron-3-ultra-free` | Advanced capabilities |
| 🚀 `north-mini-code-free` | Optimized for code |

🌐 Web search via [Exa](https://exa.ai/) is also **free**.

---

## 📊 System Requirements

| Requirement | Details |
|-------------|---------|
| 🖥️ **OS** | Linux x86_64 |
| 💾 **RAM** | < 50 MB |
| 📦 **Binary** | ~15 MB |
| 🐍 **Language** | Python |
| 📜 **License** | Free (binary only) |

---

## 📜 License

**PyCode is free to use but NOT open source.** No source code is available. The binary is distributed freely for personal and commercial use.

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

© 2026 PyCode — Free to use (binary only)

</div>
