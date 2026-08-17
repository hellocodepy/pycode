<div align="center">

# PyCode

### AI-powered coding assistant in your terminal

**Chat with LLMs, run tools, and write code — all without leaving your command line.**

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
| Context Compaction | Auto-summarizes when full. You never lose what matters. |
| Theme Picker | Multiple built-in themes, switch live with `Ctrl+P`. |
| Model Picker | Fetch and switch models on the fly with `Ctrl+O`. |
| Custom Provider Support | Connect your own OpenAI-compatible endpoint + access key with `Ctrl+U` or `/provider`. Use local models, private proxies, or any compatible service. |

### Tools that DO the work

| Tool | Description |
|------|-------------|
| bash | Execute shell commands |
| read | Read file contents |
| write | Write/create files |
| edit | Edit with exact string replacement |
| glob | Find files by glob pattern |
| grep | Search file contents with regex |
| apply_patch | Apply aider-style patches |
| webfetch | Fetch and extract text from a URL |
| websearch | Search the web for current info |
| todowrite | Structured task list |
| question | Multiple-choice question to the user |
| memory | Retrieve context from past sessions |
| task | Spawn sub-agents for delegated work |
| set_title | Auto-generated session title |
| codeview | Render code snippets with syntax highlighting |

### An experience that HOOKS you

| Feature | Description |
|---------|-------------|
| Beautiful TUI | Powered by [Textual](https://textual.textualize.io/). Rich colors, responsive. |
| Context Usage Bar | Real-time token usage in the status bar. |
| Reasoning Display | See the model's "thinking" with elapsed time. |
| Diff Rendering | Colored diffs for `apply_patch` results. |
| Persistent History | Your prompts are saved and recalled with Up/Down arrows. |
| Help Screen | Keyboard shortcuts on 2 pages (`F1`). |
| Copy Messages | Copy responses via `/copy` (OSC 52, works in web). |
| Mouse Selection | Toggle with `Ctrl+S` or `/select`. |
| Error Dialogs | Friendly handling for rate limits, auth, server errors. |
| Session Memory | The `memory` tool retrieves snippets from past chats. |

### Agents ready for anything

| Agent | Type | Description |
|-------|------|-------------|
| `build` | Primary | Default agent — full tool access. |
| `plan` | Primary | Read-only — great for analysis. |
| `explore` | Subagent | Fast codebase exploration. |
| `general` | Subagent | Research and multi-step execution. |

### ADVANCED mode

| Feature | Description |
|---------|-------------|
| Web Browser Mode | `pycode web` serves the TUI in your browser via [textual-serve](https://github.com/Textualize/textual-serve). |
| CLI Subcommands | `pycode`, `pycode web`, `pycode run TEXT`, `pycode help`. |
| Session Resume | `pycode -s SESSION_ID` picks up where you left off. |
| Auto Update Check | `pycode help` shows an update notice if a newer version exists. |
| models.dev Integration | Real context windows from the catalog. |
| Proxy Support | Respects `HTTPS_PROXY` / `HTTP_PROXY` / `ALL_PROXY` and `NO_PROXY`. |
| Message Queue | Type while it processes — queued automatically. |
| Non-blocking Tools | All tools run in background threads. UI stays responsive. |
| File References | Reference files with `@path` or `/file`. |
| Shell Integration | Run inline with `!command` or `/shell command`. |
| Slash Commands | Type `/` for the filterable commands menu. |

---

## FREE MODELS — NO KEY REQUIRED

**Works out of the box.** PyCode ships with a built-in free provider offering **6 free models**, automatically detected and switchable on the fly with `Ctrl+O`. The default model is `mimo-v2.5`.

| Model | Description |
|-------|-------------|
| deepseek-v4-flash | Fast and efficient |
| mimo-v2.5 | Balanced performance (default) |
| hy3 | Powerful and versatile |
| nemotron-3-ultra | Advanced capabilities |
| nemotron-3.5-lightning | Lightning-fast |
| laguna-s-2.1 | Lightweight and fast |

**Want your own models?** Add a custom OpenAI-compatible provider (`Ctrl+U` or `/provider`) and use local LLMs (Ollama, LM Studio), private proxies, or any compatible service.

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
    └── models-dev.json  # model catalog cache
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

Technical and design details verified in the project source code:

| Fact | Detail |
|------|--------|
| Current version | `1.6.0` (defined in `__version__.py`; `pycode help` warns if a newer version exists at `pycode.kozow.com/version.txt`). |
| Creator / author | Eduardo Castillo (`lu9dce@gmx.com`), a.k.a. **hElLocoDeLinux**. |
| Default provider | Free public endpoint with `public` key — **no key or sign-up required**. Can be changed at runtime (`Ctrl+U` or `/provider`). |
| Available models | PyCode automatically detects the **6 free models** offered by the built-in provider (no key): `deepseek-v4-flash`, `mimo-v2.5`, `hy3`, `nemotron-3-ultra`, `nemotron-3.5-lightning`, `laguna-s-2.1`. Default model is `mimo-v2.5`. |
| Operation modes | `build` (full access), `plan` (read-only), `chat` (web only: `webfetch` + `websearch`). Switch with `Ctrl+B` or `/mode`. |
| Agents | Primary: `build`, `plan`. Sub-agents: `explore`, `general` (spawned via the `task` tool). Hidden/automatic: `title`, `compaction`. |
| Tools | 15 in total: `bash`, `read`, `write`, `edit`, `glob`, `grep`, `apply_patch`, `webfetch`, `websearch`, `todowrite`, `question`, `memory`, `task`, `set_title`, `codeview`. |
| Context compaction | Automatic summary when the context window fills up. Overflow detection with ~30 error patterns and retry with reduced context. |
| models.dev catalog | Real per-model context windows, with a 7-day local cache (`models-dev.json`). Fallback: 1,000,000 tokens. |
| Retries | **Fixed** backoff of 2 s (max 30 s), up to 3 attempts, for 5xx, 429, 408/409/425 and transport errors. |
| Proxy support | Respects `HTTP_PROXY` / `HTTPS_PROXY` / `ALL_PROXY` and `NO_PROXY`. The proxy is NOT applied to local/private hosts nor to the catalog query. |
| TUI | Built with [Textual](https://textual.textualize.io/) + [Rich](https://rich.readthedocs.io/). Color depth auto-detected (truecolor/256/16). |
| Web mode | `pycode web` serves the TUI in the browser via [textual-serve](https://github.com/Textualize/textual-serve) (default port `10365`). |
| Language | PyCode **always responds in the user's language** (fixed instruction in the system prompt). |
| Build | Packaged as a single binary with [PyInstaller](https://pyinstaller.org/) (see `pycode.spec`). Cross-platform: Linux x86_64, Windows x64 and ARM64 (Raspberry Pi). |
| Secure config | `config.json` is written with `0600` permissions (read/write for the user only). |
| License | Proprietary / closed (the binary is free but the source code is not published). |

### Keyboard shortcuts

| Shortcut | Action |
|----------|--------|
| `Ctrl+B` | Switch mode (build / plan / chat) |
| `Ctrl+P` / `Ctrl+T` | Select theme |
| `Ctrl+O` | Select model |
| `Ctrl+U` | Configure provider (endpoint + key) |
| `Ctrl+S` | Toggle mouse selection |
| `Ctrl+R` | Manage sessions |
| `Ctrl+N` | New session |
| `Ctrl+L` | Clear chat |
| `Ctrl+C` | Copy (overrides Textual's default binding) |
| `Esc` | Stop / cancel |
| `F1` | Help screen (shortcuts + slash commands) |

### Slash commands

`/mode` · `/model` · `/provider` · `/sessions` · `/new` · `/clear` · `/theme` · `/help` · `/copy` · `/select` · `/shell` · `/file` · `/exit`

---

## License

**PyCode is a closed-source, proprietary application.** It is distributed as a ready-to-run binary and is free to use, but the source code is not published and may not be redistributed or modified.

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