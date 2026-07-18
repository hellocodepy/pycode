# PyCode — Terminal AI Assistant

**PyCode** is a lightweight, open-source terminal assistant (TUI) for developers.
Chat with LLMs, run tools, and write code — all without leaving your command line.
It uses under **50 MB** of RAM and is built with Python and [Textual](https://textual.textualize.io/).

> Website: https://shure.kozow.com/
> Contact: lu9dce@gmx.com

---

## Features

- **Multi-Model (Free)** — Ships configured to use the free [OpenCode Zen](https://opencode.ai/zen) endpoint, which provides 5 free models out of the box. No paid API key required — just run it. You can still point it at OpenAI, Anthropic, Ollama, or any OpenAI-compatible API if you want.
- **Lightweight** — Consistently runs under 50 MB of RAM. No Electron, no bloated runtime — just Python and your terminal.
- **Built-in Tools** — File editor, code runner, web search, and more. PyCode can execute commands and modify files with your permission. Web search is powered by [Exa](https://exa.ai/) and works freely and at no cost.
- **Chat Sessions** — Persistent conversations with history. Revisit, rename, or delete sessions anytime.
- **Beautiful TUI** — Powered by Textual. Rich colors, themes, and a responsive terminal interface.
- **Open Source** — 100% free and open-source (MIT). Audit the code, contribute, and customize to your needs.

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

- **Python 3.10+** (for running from source)
- **Linux x86_64** (for the pre-compiled binary)
- **No API key needed** — PyCode ships pre-configured to use the free [OpenCode Zen](https://opencode.ai/zen) endpoint, which offers 5 free models out of the box:

  - `hy3-free`
  - `deepseek-v4-flash-free`
  - `mimo-v2.5-free`
  - `nemotron-3-ultra-free`
  - `north-mini-code-free`

  Web search via [Exa](https://exa.ai/) is also free. You only need your own API key if you want to use a different/paid provider.

---

## Installation

### Option 1 — Pre-compiled Binary (Linux x86_64)

No dependencies required. Download and run:

```bash
curl -L https://shure.kozow.com/download.php?type=bin -o pycode && chmod +x ./pycode
./pycode
```

### Option 2 — From Source

```bash
# Download source
curl -L https://shure.kozow.com/download.php?type=src -o pycode-source.zip
unzip pycode-source.zip
cd pycode-source

# Install dependencies
pip install -r requirements.txt

# Run
python main.py
```

Dependencies are kept minimal:

```
textual==8.2.8
httpx==0.28.1
```

---

## Building from Source

The binary is produced with [PyInstaller](https://pyinstaller.org/) using the
provided spec file:

```bash
pip install pyinstaller
pyinstaller src/pycode.spec
```

The resulting executable is written to `dist/pycode` (~15 MB).

---

## License

PyCode is released under the **MIT License**.

---

## Contact

- **Website:** https://shure.kozow.com/
- **Email:** lu9dce@gmx.com
- **Author:** Eduardo Castillo (lu9dce@gmx.com)

© 2026 PyCode — Open source (MIT). Built with ❤️ for terminal lovers.
