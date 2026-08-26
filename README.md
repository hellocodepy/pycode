<div align="center">

# PyCode

### AI-powered coding assistant in your terminal

**Chat with AI, run tools, and write code — all without leaving your command line.**

[![Website](https://img.shields.io/badge/Website-pycode.kozow.com-6366f1)](https://pycode.kozow.com/)
[![WhatsApp](https://img.shields.io/badge/WhatsApp-@hellocodelinux-25D366)](https://wa.me/5491112345678)
[![Email](https://img.shields.io/badge/Email-hellocodelinux@gmail.com-EA4335)](mailto:hellocodelinux@gmail.com)

---

Lightweight • Beautiful • Powerful • Free

</div>

---

<div align="center">

## Tired of endless tabs, painful setups, and keys that never work?

### With PyCode, forget all of that.

> **Your AI assistant lives in your terminal. Write code, fix bugs, and search the web with a single command.**

**No keys. No crazy installs. No hassle. Just download and type.**

</div>

---

<div align="center">

## Grab it NOW

### Website: [pycode.kozow.com](https://pycode.kozow.com/)

### Binary available on the site — ready to use in seconds

</div>

---

## Why PyCode is DIFFERENT

### Smart core

| Feature | Description |
|---------|-------------|
| Build / Plan / Chat Modes | Full access, read-only, or web-only — switch with `Ctrl+B`. |
| Chat Sessions | Persistent conversations. Revisit, rename, or delete anytime. |
| Context Compaction | Auto-summarizes long conversations. You never lose what matters. |
| Theme Picker | Multiple built-in themes, switch live with `Ctrl+P` or `Ctrl+T`. |
| Model Picker | Fetch and switch models on the fly with `Ctrl+O`. |
| Custom Provider Support | Connect your own AI provider with `Ctrl+U` or `/provider`. Use local models, private proxies, or any compatible service. |
| Automatic Titles | Sessions get smart, AI-generated titles based on your first message. |
| Message Queue | Type while the AI is thinking — your messages are queued and sent in order. |
| Language Detection | Always responds in your language, automatically. |

### Tools that DO the work

| Tool | Description |
|------|-------------|
| bash | Execute shell commands |
| read | Read file contents |
| write | Write/create files |
| edit | Edit with exact string replacement |
| glob | Find files by glob pattern |
| grep | Search file contents with regex |
| apply_patch | Apply code patches |
| webfetch | Fetch and extract text from a URL |
| websearch | Search the web for current info |
| todowrite | Structured task list |
| question | Multiple-choice questions |
| memory | Retrieve context from past sessions |
| task | Spawn sub-agents for delegated work |
| set_title | Set a custom session title |
| codeview | Render code snippets with syntax highlighting |

### An experience that HOOKS you

| Feature | Description |
|---------|-------------|
| Beautiful TUI | Rich colors, responsive, and easy on the eyes. |
| Context Usage Bar | Real-time token usage in the status bar. |
| Reasoning Display | See the AI's "thinking" with elapsed time. |
| Diff Rendering | Colored diffs for `apply_patch` results. |
| Persistent History | Your prompts are saved and recalled with Up/Down arrows. |
| Help Screen | Keyboard shortcuts on 2 pages (`F1`). |
| Copy Messages | Copy responses via `/copy`. |
| Mouse Selection | Toggle with `Ctrl+S` or `/select`. |
| Error Dialogs | Friendly handling for rate limits, auth, server errors. |
| Session Memory | The `memory` tool retrieves snippets from past chats. |
| File References | Mention files with `@path` to reference them in your messages. |
| Shell Commands | Run shell commands directly with `!command`. |

### Agents ready for anything

| Agent | Type | Description |
|-------|------|-------------|
| `build` | Primary | Default agent — full tool access. |
| `plan` | Primary | Read-only — great for analysis and planning. |
| `explore` | Subagent | Fast codebase exploration. |
| `general` | Subagent | Research and multi-step execution. |

### ADVANCED mode

| Feature | Description |
|---------|-------------|
| Web Browser Mode | `pycode web` serves the TUI in your browser. |
| CLI Subcommands | `pycode`, `pycode web`, `pycode run TEXT`, `pycode help`. |
| Session Resume | `pycode -s SESSION_ID` picks up where you left off. |
| Auto Update Check | `pycode help` shows an update notice if a newer version exists. |
| Accurate context windows | Real per-model context limits, kept current automatically. |
| Proxy Support | Respects `HTTPS_PROXY` / `HTTP_PROXY` / `ALL_PROXY` and `NO_PROXY`. |
| Non-blocking Tools | All tools run in background threads. UI stays responsive. |
| Slash Commands | Type `/` for the filterable commands menu. |
| Automatic Retries | Silently retries on transient errors (up to 3 times). |

---

## FREE MODELS — NO KEY REQUIRED

**Works out of the box.** PyCode includes **6 free models**, automatically detected and switchable on the fly with `Ctrl+O`. The default model is `mimo-v2.5`.

| Model | Description |
|-------|-------------|
| deepseek-v4-flash | Fast and efficient |
| mimo-v2.5 | Balanced performance (default) |
| hy3 | Powerful and versatile |
| nemotron-3-ultra | Advanced capabilities |
| nemotron-3.5-lightning | Lightning-fast |
| laguna-s-2.1 | Lightweight and fast |

**Want your own models?** Add a custom AI provider (`Ctrl+U` or `/provider`) and use local models, private proxies, or any compatible service.

---

## Up and running in 5 SECONDS

### Install

```bash
# Linux x86_64
curl -L https://pycode.kozow.com/bin/lnx64/pycode -o pycode && chmod +x ./pycode

# Raspberry Pi (ARM64)
curl -L https://pycode.kozow.com/bin/pi64/pycode -o pycode && chmod +x ./pycode

# Windows (PowerShell)
curl -L https://pycode.kozow.com/bin/win64/pycode.exe -o pycode.exe
```

### Run

```bash
./pycode                  # Start the TUI
./pycode -s SESSION_ID    # Resume a previous session
./pycode web              # Serve in browser
./pycode web --port 8080  # Serve on custom port
./pycode web --public-url http://example.com:8080  # With public URL
./pycode help             # Show version and usage
./pycode run TEXT         # One-shot prompt
```

---

## Minimal requirements, MAXIMUM power

| Requirement | Details |
|-------------|---------|
| OS | Linux (x86_64), Windows (x64), Raspberry Pi / ARM64 Linux |
| RAM | ~80 MB (process: ~2 MB CLI + ~78 MB core) |
| Binary | ~17–20 MB (varies by platform) |
| Disk | ~40 MB (binary + ~15 MB config/cache) |
| CPU | Any x86_64, x64 or ARM64 processor (~1% idle, ~5% inference) |
| Terminal | Any terminal with Unicode or ASCII support (auto-detected) |
| License | Proprietary |

---

## Portable Mode — take it EVERYWHERE

Run PyCode from a USB drive or portable disk:

### Activation
Create an empty file named `portable.txt` next to the `pycode` binary:
```
/media/usb/pycode/
├── pycode              # binary
├── portable.txt        # marker file (activates portable mode)
├── pycodata/           # created automatically
    ├── config.json     # theme settings
    ├── sessions/       # all session files
    ├── prompt-history.jsonl  # input history
    └── models cache  # cached model catalog
```

### Priority
1. `PYCODE_DATA_DIR` env var (explicit override)
2. Portable mode (`portable.txt` marker)
3. Standard: `~/.config/pycode-tui/`

### Notes
- Prompts (`prompts/`) are bundled inside the binary (read-only)
- All your data travels in `pycodata/`
- No auto-detection of removable drives; requires the `portable.txt` marker

---

## Notable facts about PyCode

| Fact | Detail |
|------|--------|
| Current version | `1.6.4`. The app notifies you when a newer version is available. |
| Creator | Eduardo Castillo (`lu9dce@gmx.com`), a.k.a. **hElLocoDeLinux**. |
| Built-in provider | A free provider is included — no key or sign-up required. Switch anytime with `Ctrl+U` or `/provider`. |
| Available models | `deepseek-v4-flash`, `mimo-v2.5`, `hy3`, `nemotron-3-ultra`, `nemotron-3.5-lightning`, `laguna-s-2.1`. Default is `mimo-v2.5`. |
| Operation modes | `build` (full access), `plan` (read-only), `chat` (web only). Switch with `Ctrl+B` or `/mode`. |
| Agents | Two primary agents (`build`, `plan`) plus specialized sub-agents (`explore`, `general`) for delegated work. |
| Context handling | Automatic summarization when the conversation gets long, with smart overflow handling so you never lose context. |
| Context windows | Accurate per-model context windows, kept up to date automatically. |
| Reliability | Automatic retries with backoff on transient server errors. |
| Proxy support | Works behind corporate proxies (respects standard proxy settings). |
| Adaptive UI | Beautiful terminal interface that adapts its colors to your terminal's capabilities. |
| Web mode | Run the interface in your browser and access it from any device on the network. |
| Language | Always responds in the user's language. |
| Cross-platform | A single self-contained binary for Linux x86_64, Windows x64 and ARM64 (Raspberry Pi). |
| Privacy | Your sessions, history and settings are stored locally on your machine. |
| License | Proprietary / closed (free to use, source not published). |

### Keyboard shortcuts

| Shortcut | Action |
|----------|--------|
| `Ctrl+B` | Switch mode (build / plan / chat) |
| `Ctrl+P` / `Ctrl+T` | Select theme |
| `Ctrl+O` | Select model |
| `Ctrl+U` | Configure provider (URL + key) |
| `Ctrl+S` | Toggle mouse selection |
| `Ctrl+R` | Manage sessions |
| `Ctrl+N` | New session |
| `Ctrl+L` | Clear chat |
| `Ctrl+C` | Copy (overrides the default terminal binding) |
| `Ctrl+Q` | Quit |
| `Esc` | Stop / cancel |
| `F1` | Help screen (shortcuts + slash commands) |
| `PageUp` | Scroll up |
| `PageDown` | Scroll down |
| `↑` / `↓` | Navigate prompt history |

### Slash commands

`/mode` · `/model` · `/provider` · `/sessions` · `/new` · `/clear` · `/theme` · `/help` · `/copy` · `/select` · `/shell` · `/file` · `/exit`

---

## Alternatives

PyCode replaces: Claude Code · Aider · Gemini CLI · Codex CLI · Goose · Amazon Q Developer CLI

---

## License

**PyCode is a proprietary, closed-source application.** It is distributed as a ready-to-run binary, is free to use, but may not be redistributed or modified.

---

## Credits

Inspired by AI-powered coding assistants for the terminal.

---

## Contact

| Channel | Link |
|---------|------|
| Website | [pycode.kozow.com](https://pycode.kozow.com/) |
| Email | [hellocodelinux@gmail.com](mailto:hellocodelinux@gmail.com) |
| WhatsApp | [@hellocodelinux](https://wa.me/5491112345678) |

---

<div align="center">

**Made with love for terminal lovers**

© 2026 PyCode

</div>
