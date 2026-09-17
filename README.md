# INDEX 0

[![Website](https://img.shields.io/badge/website-index--0.in-1cd6ac)](https://www.index-0.in)
[![Latest release](https://img.shields.io/github/v/release/MadhumithaKolkar/index0-releases?label=latest&color=1cd6ac)](https://github.com/MadhumithaKolkar/index0-releases/releases/latest)
[![Downloads](https://img.shields.io/github/downloads/MadhumithaKolkar/index0-releases/total?label=downloads&color=1cd6ac)](https://github.com/MadhumithaKolkar/index0-releases/releases)
[![Platforms](https://img.shields.io/badge/platform-macOS%20|%20Windows%20|%20Linux-1cd6ac)](#download)
[![License](https://img.shields.io/badge/license-free%20to%20use%2C%20source%20closed-1cd6ac)](#license)

**A free, local-first learning platform for engineers - DSA, ML/AI, electronics, and system design, all coached by the same AI, entirely on your own machine.**

No cloud, no subscription, no account. INDEX 0 runs a local Ollama + Gemma model on your computer, so nothing you write is ever sent anywhere. This repo hosts the built app for macOS, Windows, and Linux, and powers the in-app "check for updates" feature.

**[Download it at www.index-0.in →](https://www.index-0.in)**

---

## What's actually in it

INDEX 0 isn't just a DSA tool - it's one coach across four subjects, so you build one way of thinking instead of stitching together a hundred scattered tutorials.

| Section | What it is |
|---|---|
| **DSA Coach** | 422 problems, each walked through with a strict 6-stage Socratic loop: understand → intuition → brute force → tradeoffs → optimize → final. Zero won't show you working code before the final stage - no matter how directly you ask. |
| **ML/AI Roadmap** | 34 structured lectures, not a scattered YouTube playlist. |
| **Electronics Roadmap** | 74 lessons, from Ohm's law through PCB design, logic gates, and a full connected capstone project. |
| **System Design Roadmap** | 102 lessons, from fundamentals through real-world case studies. |
| **Mock Interviews** | A guided solo interview with Zero - pick a specialization and level, get graded, get a report on exactly what to fix. |
| **Games** | Sequence Recall, Quick Math Sprint, Pattern Predictor, Lights Out, ML Hangman, and Big-O Blitz - for when you need an actual break, not more studying. |

### Meet Zero

Zero is the coach behind all of it, and it's built to be strict on purpose. Most tools optimize for the moment you get unstuck; Zero optimizes for the moment six months from now when you see a similar problem and actually recognize it. That means:

- No working code before the final stage - guiding questions instead of instructions, however directly you ask.
- Every judgment grounded in the specific problem's real constraints, not a model's fuzzy memory of "what LeetCode 42 is."
- Progressively stronger hints as you get stuck, never just handing you the pattern's name outright.

### Fully local, by design

The whole app runs against a local [Ollama](https://ollama.com) install and a [Gemma](https://ai.google.dev/gemma) model on your own machine. There's no server, no account, no telemetry pipeline. The one-time setup wizard walks you through installing anything you're missing (Ollama, Python, and whichever language toolchains you want for DSA).

---

## Download

Grab the latest build from the [Releases page](../../releases/latest), or use the platform-specific links on **[www.index-0.in](https://www.index-0.in)**, which always point at the current release automatically.

| Platform | File | Notes |
|---|---|---|
| macOS (Apple Silicon) | `INDEX0-arm64.dmg` | M1 and newer |
| macOS (Intel) | `INDEX0-x64.dmg` | 2019 and newer |
| Windows | `INDEX0-Setup.exe` | Windows 10 (64-bit) and newer |
| Linux (x86_64) | `INDEX0-x86_64.AppImage` | any modern 64-bit distro |
| Linux (ARM64) | `INDEX0-arm64.AppImage` | any modern ARM64 distro |

**These builds aren't code-signed** - a free, solo-built project, that's the honest tradeoff. Your OS will show a security warning on first launch (Gatekeeper on macOS, SmartScreen on Windows). The [download page](https://www.index-0.in#download) has the one-time steps to get past that safely.

Once installed, the app checks for updates automatically on launch and periodically while running, and prompts you in-app when a new version is ready - no need to come back here to redownload manually.

---

## Version history

### v1.2.0 - DSA screen fixes, from real user feedback

**Added**
- Failed test cases now show the input that produced the failure.
- Moved the editor zoom control next to the language picker, and added a Reset button to start a problem over with fresh starter code.

**Fixed**
- Python (and other tools) sometimes not being detected on Linux even when installed.
- Your language choice not sticking when solving DSA problems.
- In-progress code sometimes being lost when navigating back.
- Zero's replies occasionally getting cut off.
- Zero still saying "Captain" after you've set your own name.
- Setup downloads failing outright on a dropped connection instead of retrying.
- In-app updates not actually working on Linux.

### v1.1.0 - Linux support, an Intel Mac build, and a few fixes

**Added**
- Linux support (AppImage, x86_64 and ARM64).
- An Intel Mac build alongside the existing Apple Silicon one.
- A font-size control for the code editor, separate from the app-wide one.

**Fixed**
- "Zero's notes about you" sometimes cutting a note off mid-word.
- Softened the app's main text color so it's easier on the eyes.

### v1.0.0 - Initial public launch

First public release: macOS (Apple Silicon) and Windows builds, with Linux support and an Intel Mac build following shortly after in v1.1.0.

---

## License

INDEX 0 is **free to use, but not open source** - the source code and all content (curriculum, coaching prompts, branding) remain fully owned by the author. In short, you may download and use the app for free, for your own learning, but you may not:

- Sell, sublicense, or charge money for INDEX 0 or any derivative of it.
- Use it as part of a paid product or service.
- Redistribute the source code (it isn't published here - this repo only hosts built binaries).

The full license text is available in-app and on the [website](https://www.index-0.in).

---

## Feedback & support

Source code lives in a separate private repository. This repo exists solely to distribute builds and back the in-app "check for updates" feature - it isn't meant to receive issues or PRs.

- **Bugs, feedback, or feature requests:** [creator@index-0.in](mailto:creator@index-0.in), or the feedback form on [the website](https://www.index-0.in).
- **1:1 mentoring:** [book a session](https://topmate.io/madhumitha_kolkar/).

If INDEX 0 has been useful, the download page has a way to say thanks - entirely optional, the app itself will always be free.
