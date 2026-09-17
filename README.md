# INDEX 0

[![Website](https://img.shields.io/badge/website-index--0.in-1cd6ac)](https://www.index-0.in)
[![Latest release](https://img.shields.io/github/v/release/MadhumithaKolkar/index0-releases?label=latest%20release&color=1cd6ac)](https://github.com/MadhumithaKolkar/index0-releases/releases/latest)
[![Downloads](https://img.shields.io/github/downloads/MadhumithaKolkar/index0-releases/total?label=downloads&color=1cd6ac)](https://github.com/MadhumithaKolkar/index0-releases/releases)
[![Platforms](https://img.shields.io/badge/platform-macOS%20|%20Windows%20|%20Linux-1cd6ac)](#download)
[![License](https://img.shields.io/badge/license-free%20to%20use%2C%20source%20closed-1cd6ac)](#license)

**A free, local-first learning platform for engineers, covering DSA, ML/AI, electronics, and system design, with an integrated AI coach.**

INDEX 0 runs entirely on the user's own machine against a local Ollama + Gemma model. There is no cloud dependency, account, or subscription, and no data leaves the device. This repository hosts the built application for macOS, Windows, and Linux, and backs the in-app update checker.

**[Download at www.index-0.in →](https://www.index-0.in)**

---

## Overview

| Metric | Value |
|---|---|
| DSA problems | 422 |
| ML/AI lectures | 34 |
| Electronics lessons | 74 |
| System design lessons | 102 |
| Mock interview modes | Guided, specialization- and level-based |
| Supported platforms | macOS (Apple Silicon, Intel), Windows, Linux (x86_64, ARM64) |
| Deployment | Fully local, no cloud dependency |
| License | Free to use, source closed |

## Modules

| Module | Description |
|---|---|
| **DSA Coach** | 422 problems, each progressing through six structured stages: problem framing, intuition, initial implementation, complexity analysis, optimization, and final review. Solutions are withheld until the final stage to reinforce independent problem-solving. |
| **ML/AI Roadmap** | 34 structured lectures covering core machine learning and AI concepts. |
| **Electronics Roadmap** | 74 lessons spanning fundamentals (Ohm's law, digital logic) through PCB design and a capstone connected-hardware project. |
| **System Design Roadmap** | 102 lessons covering fundamentals through real-world case studies. |
| **Mock Interviews** | A guided solo interview mode with specialization and difficulty selection, structured feedback, and a report on specific areas to improve. |
| **Games** | Six supplementary games (Sequence Recall, Quick Math Sprint, Pattern Predictor, Lights Out, ML Hangman, Big-O Blitz) reinforcing core concepts. |

### AI coach

The in-app coach ("Zero") is designed to reinforce understanding rather than provide direct answers:

- No working solution code is shown before the final review stage, regardless of how directly it is requested.
- Feedback is grounded in the specific problem's stated constraints rather than the model's general training data.
- Hints escalate progressively as the user gets stuck, rather than revealing the underlying pattern outright.

### Local execution

The application runs against a local [Ollama](https://ollama.com) installation and a [Gemma](https://ai.google.dev/gemma) model on the user's own machine. There is no backend server, account system, or telemetry collection. A one-time setup wizard installs any missing dependencies (Ollama, Python, and the language toolchains required for DSA problem execution).

---

## Download

The latest build is available from the [Releases page](../../releases/latest), or via the platform-specific links on **[www.index-0.in](https://www.index-0.in)**, which resolve to the current release automatically.

| Platform | File | Requirements |
|---|---|---|
| macOS (Apple Silicon) | `INDEX0-arm64.dmg` | M1 or newer |
| macOS (Intel) | `INDEX0-x64.dmg` | 2019 or newer |
| Windows | `INDEX0-Setup.exe` | Windows 10 (64-bit) or newer |
| Linux (x86_64) | `INDEX0-x86_64.AppImage` | Any modern 64-bit distribution |
| Linux (ARM64) | `INDEX0-arm64.AppImage` | Any modern ARM64 distribution |

These builds are not code-signed. As a solo-built, free project, this is an accepted tradeoff. The OS will show a security warning on first launch (Gatekeeper on macOS, SmartScreen on Windows); the [download page](https://www.index-0.in#download) documents the one-time steps required to proceed.

Installed copies check for updates automatically on launch and periodically while running, and prompt in-app when a new version is available.

---

## Version history

### v1.2.0 — DSA screen fixes, from user feedback

**Added**
- Failed test cases now display the input that produced the failure.
- Editor zoom control relocated next to the language picker; added a Reset button to restore a problem's starter code.

**Fixed**
- Python (and other tools) sometimes not being detected on Linux even when installed.
- Language selection not persisting while solving DSA problems.
- In-progress code occasionally lost when navigating back.
- Coach replies occasionally truncated.
- Coach using a default name after the user had set a custom display name.
- Setup downloads failing outright on a dropped connection instead of retrying.
- In-app updates not functioning on Linux.

### v1.1.0 — Linux support, Intel Mac build

**Added**
- Linux support (AppImage, x86_64 and ARM64).
- Intel Mac build alongside the existing Apple Silicon build.
- Independent font-size control for the code editor.

**Fixed**
- Memory notes occasionally truncated mid-word.
- Reduced primary text contrast for improved readability.

### v1.0.0 — Initial public release

First public release: macOS (Apple Silicon) and Windows builds. Linux support and an Intel Mac build followed in v1.1.0.

---

## License

INDEX 0 is **free to use but not open source**. The source code and all content (curriculum, coaching prompts, branding) remain the property of the author.

**Permitted:**
- Downloading and using the application for personal learning, at no cost.

**Not permitted:**
- Selling, sublicensing, or charging for INDEX 0 or any derivative of it.
- Incorporating it into a paid product or service.
- Redistributing the source code (not published in this repository, which hosts built binaries only).

Full license text is available in-app and on the [website](https://www.index-0.in).

---

## Feedback & support

Source code is maintained in a separate private repository. This repository exists solely to distribute builds and back the in-app update checker; it does not accept issues or pull requests.

| Channel | Purpose |
|---|---|
| [creator@index-0.in](mailto:creator@index-0.in) | Bug reports, feedback, feature requests |
| [Website feedback form](https://www.index-0.in) | Bug reports, feedback, feature requests |
| [Topmate](https://topmate.io/madhumitha_kolkar/) | 1:1 mentoring sessions |
