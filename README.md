# PyCode — Terminal AI Assistant

**PyCode** is a lightweight, free terminal assistant (TUI) for developers.
Chat with LLMs, run tools, and write code — all without leaving your command line.
It uses under **50 MB** of RAM and is built with Python and [Textual](https://textual.textualize.io/).

> Website: [https://pycode.kozow.com/](https://pycode.kozow.com/)
> Contact: lu9dce@gmx.com
> WhatsApp: @hellocodelinux

---

## Features

- **Multi-Model (Free)** — Ships configured to use the free [OpenCode Zen](https://opencode.ai/zen) endpoint, which provides 5 free models out of the box. No paid API key required — just run it. You can still point it at OpenAI, Anthropic, Ollama, or any OpenAI-compatible API if you want.
- **Lightweight** — Consistently runs under 50 MB of RAM. No Electron, no bloated runtime — just Python and your terminal.
- **Built-in Tools** — File editor, code runner, web search, and more. PyCode can execute commands and modify files with your permission. Web search is powered by [Exa](https://exa.ai/) and works freely and at no cost.
- **Chat Sessions** — Persistent conversations with history. Revisit, rename, or delete sessions anytime.
- **Beautiful TUI** — Powered by Textual. Rich colors, themes, and a responsive terminal interface.
- **Free to Use** — 100% free to use. No source code available (binary only). Suggestions and feedback welcome via email (lu9dce@gmx.com) or WhatsApp (@hellocodelinux).
- **Build / Plan Modes** — Two modes: **Build** (full tool access) and **Plan** (read-only). Switch instantly with `Ctrl+B`.
- **Context Compaction** — Automatic conversation summarization when context fills up. Preserves key decisions, file changes, and open tasks while truncating old tool output.
- **Session Management** — Full session persistence: save, load, switch, rename, delete. Sessions survive restarts.
- **Theme Picker** — Multiple built-in themes, switchable at runtime (`Ctrl+P`).
- **Model Picker** — Fetch and switch models on the fly (`Ctrl+O`). Auto-detects free models from OpenCode Zen.
- **File Picker** — Interactive file browser with fuzzy filtering. Trigger with `@` in the input.
- **Shell Integration** — Run shell commands inline with `!command` or `/shell command`.
- **File References** — Reference files with `@path` — PyCode reads them on demand via the Read tool.
- **Reasoning Display** — Shows model "thinking" process with elapsed time (for models that support it).
- **Diff Rendering** — Colored diffs for `apply_patch` results (added/removed lines highlighted).
- **Context Usage Bar** — Real-time token usage and percentage in the status bar.
- **Settings Modal** — Configure API endpoint, key, and model without editing files (`Ctrl+S`).
- **Help Screen** — Keyboard shortcuts reference (`F1`).
- **Copy Messages** — Copy assistant responses to clipboard (`Ctrl+Y`).
- **Error Dialogs** — Friendly error handling for rate limits, auth failures, server errors.
- **Proxy Support** — Respects `HTTPS_PROXY` / `HTTP_PROXY` environment variables.
- **Models.dev Integration** — Auto-fetches real context windows from the models.dev catalog (same as opencode).

### Available Tools

PyCode ships with a set of built-in tools the LLM can call:

| Tool | Description |
|------|-------------|
| `bash` | Execute shell commands |
| `read` | Read file contents |
| `write` | Write/create files |
| `edit` | Edit files with exact string replacement |
| `glob` | Find files by glob pattern |
| `grep` | Search file contents with regular expressions |
| `apply_patch` | Apply unified diff-style patches |
| `webfetch` | Fetch and extract text from a URL |
| `websearch` | Search the web for current information |
| `todowrite` | Create and manage a structured task list |
| `question` | Ask the user a multiple-choice question |

---

## Requirements

- **Linux x86_64** (pre-compiled binary)
- **No API key needed** — PyCode ships pre-configured to use the free [OpenCode Zen](https://opencode.ai/zen) endpoint, which offers 5 free models out of the box:

  - `hy3-free`
  - `deepseek-v4-flash-free`
  - `mimo-v2.5-free`
  - `nemotron-3-ultra-free`
  - `north-mini-code-free`

  Web search via [Exa](https://exa.ai/) is also free. You only need your own API key if you want to use a different/paid provider.

---

## Installation

### Pre-compiled Binary (Linux x86_64)

No dependencies required. Download and run:

```bash
curl -L https://shure.kozow.com/bin/pycode -o pycode && chmod +x ./pycode
./pycode
```

**Source code is not publicly available.** PyCode is distributed as a free binary only. If you have feedback, suggestions, or bug reports, please contact

---

## License

**PyCode is free to use but NOT open source.** No source code is available. The binary is distributed freely for personal and commercial use.

Feedback, suggestions, and bug reports are welcome

---

## Contact

- **Website:** https://pycode.kozow.com/
- **Email:** lu9dce@gmx.com
- **WhatsApp:** @hellocodelinux
- **Author:** Eduardo Castillo
  
© 2026 PyCode — Free to use (binary only). Built with ❤️ for terminal lovers.
