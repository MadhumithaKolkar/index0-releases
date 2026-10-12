# INDEX 0

[![Website](https://img.shields.io/badge/website-index--0.in-1cd6ac)](https://www.index-0.in)
[![Latest release](https://img.shields.io/github/v/release/MadhumithaKolkar/index0-releases?label=latest%20release&color=1cd6ac)](https://github.com/MadhumithaKolkar/index0-releases/releases/latest)
[![Downloads](https://img.shields.io/endpoint?url=https%3A%2F%2Fwww.index-0.in%2Fapi%2Fdownloads-badge)](#downloads)
[![Platforms](https://img.shields.io/badge/platform-macOS%20|%20Windows%20|%20Linux-1cd6ac)](#download)
[![License](https://img.shields.io/badge/license-free%20to%20use%2C%20source%20closed-1cd6ac)](#license)

**A free, local-first learning platform for engineers, covering DSA, ML/AI, electronics, system design, and cybersecurity, with an integrated AI coach.**

INDEX 0 runs entirely on the user's own machine against a local Ollama + Gemma model. There is no cloud dependency, account, or subscription, and no data leaves the device. This repository hosts the built application for macOS, Windows, and Linux, and backs the in-app update checker.

**[Download at www.index-0.in →](https://www.index-0.in)**

---

## Overview

| Metric | Value |
|---|---|
| DSA problems | 475 |
| DSA languages | Python, C++, Java, Kotlin, JavaScript, C# |
| ML/AI lectures | 34 |
| Electronics lessons | 74 |
| System design lessons | 102 |
| Cybersecurity lessons | 68 |
| Learn to Code (Python) lessons | 51 |
| Mock interview modes | Guided, specialization- and level-based |
| Supported platforms | macOS (Apple Silicon, Intel), Windows, Linux (x86_64, ARM64) |
| Deployment | Fully local, no cloud dependency |
| License | Free to use, source closed |

## Modules

| Module | Description |
|---|---|
| **DSA Coach** | 475 problems, each progressing through six structured stages: problem framing, intuition, initial implementation, complexity analysis, optimization, and final review. Solutions are withheld until the final stage to reinforce independent problem-solving. Solutions can be written in Python, C++, Java, Kotlin, JavaScript, or C#. |
| **ML/AI Roadmap** | 34 structured lectures covering core machine learning and AI concepts. |
| **Electronics Roadmap** | 74 lessons spanning fundamentals (Ohm's law, digital logic) through PCB design and a capstone connected-hardware project. |
| **System Design Roadmap** | 102 lessons covering fundamentals through real-world case studies. |
| **Cybersecurity Roadmap** | 68 lessons spanning networking and security fundamentals through common attack vectors, defensive practices, incident response and forensics, and career paths. |
| **Learn to Code (Python)** | 51 lessons teaching programming fundamentals from scratch, from variables and control flow through functions, object-oriented programming, and capstone projects, with a judged in-browser code editor. |
| **Mock Interviews** | A guided solo interview mode with specialization and difficulty selection, structured feedback, and a report on specific areas to improve. |
| **Games** | Six supplementary games (Sequence Recall, Quick Math Sprint, Pattern Predictor, Lights Out, ML Hangman, Big-O Blitz) reinforcing core concepts. |

All roadmap-style courses (ML/AI, Electronics, Cybersecurity) are grouped under a single "Roadmaps" entry in the app's navigation.

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

macOS builds are signed and notarized by Apple as of v1.9.0 onward, so Gatekeeper opens them without a warning. Windows and Linux builds are not code-signed; as a solo-built, free project, this is an accepted tradeoff there. Windows will show a SmartScreen warning on first launch — the [download page](https://www.index-0.in#download) documents the one-time steps required to proceed.

Installed copies check for updates automatically on launch and periodically while running, and prompt in-app when a new version is available.

---

## Version history

### v1.9.2 — Math in course chats, formatted interview answers, and solved-problem resets

**Added**
- Formulas in Zero's course chats now render as proper math.
- Guardrails added to prevent Zero's course chats from subject deviation.
- Solved problems can be unchecked to reset them, and solved tiles are highlighted.

**Fixed**
- Interview ideal answers are now formatted properly.
- Zero keeps track of the problem when you switch models.
- Fixed a startup error that affected some installs.

### v1.9.1 — C# support, Vim mode, new AI/ML lessons, and grading fixes

**Added**
- C# added as a supported language for DSA problems.
- Vim mode for the code editor, toggle in the editor toolbar.
- 9 new AI/ML lessons: agent orchestration, classical ML, LSTMs, and more.
- Two new free-tier Gemini models added to the BYOK model picker.
- Coach and Ask Zero now clearly decline off-topic requests instead of attempting them.

**Fixed**
- Fixed some DSA test cases.
- Fixed Zero's incomplete responses.
- Fixed some UI issues and installation issues.

### v1.8.0 — Quiz mode, achievement sharing, and update fixes

**Added**
- Quiz mode: pre-authored multiple-choice and AI-graded free-response questions after each lesson.
- A Revisit button on each of Zero's Observations, jump straight back to that topic.
- Share your achievement badges as a downloadable poster for LinkedIn or Instagram.
- Zero's notes about you are now more holistic across topics.

**Fixed**
- Fixed the app sometimes not reopening automatically after an update on Windows.
- Fixed auto-update failing on some Windows installs.
- Fixed thin test coverage on the 53 new DSA problems from the last release.

### v1.7.0 — 53 new DSA problems, plus some polish from Zero

**Added**
- 53 new DSA problems added, spanning nearly every major pattern.
- Zero now helps you stay hydrated and sleep on time.

### v1.6.1 — Manual toolchain paths, layout fixes

**Added**
- Added manual path setup for Java, C++, and Kotlin, for when auto-detect can't find them.
- Added an optional way to support the project from inside the app.

**Fixed**
- Fixed nav bar badges and links wrapping onto two lines under tight width.
- Fixed Kotlin path setup failing to recognize a valid compiler.
- Fixed a saved custom language path not being recognized as installed.
- Fixed manual toolchain paths failing to validate on Windows.

### v1.6.0 — The Big O plotter, and bring your own local model

**Added**
- The Big O plotter: see why your solution has the complexity it does, with an animated growth curve.
- Added custom model endpoints, can be saved for later use.
- Custom Ollama endpoint for those running it elsewhere.
- Gemini joins Claude and OpenAI as a bring-your-own-model option.
- A settings gear instead of a plain letter for the profile link in the header.
- A cancel button for language installs in progress.

**Fixed**
- Fixed a custom model endpoint sometimes showing as working when it wasn't.
- Fixed no confirmation showing after switching to a custom model endpoint.
- Fixed two notification popups overlapping.
- Fixed a visual glitch on the roadmap page.
- Fixed the Ollama installer occasionally failing right after downloading on Windows.
- Fixed installing a language from your profile stopping if you left the page.
- Fixed your saved theme and font sometimes not showing correctly right when a page loads.
- Fixed an empty message sometimes appearing after sharing your code with Zero.

### v1.5.2 — See your code's output, cancel setup downloads

**Added**
- See your code's print/stdout output after running it, broken down per test case. Run with Ctrl/Cmd+'.
- Python is now optional in setup, just like Java, C++, and Kotlin.
- Every setup download (Ollama, Python, Java, C++, Kotlin, the model) can now be cancelled partway through.
- A "Next Question" button, next to the problem name, to jump straight to the next problem in the same pattern.

**Fixed**
- Fixed a wrong test case on Longest Palindromic Substring.
- Fixed code hanging forever on a timeout instead of stopping cleanly.
- Fixed a saved short display name getting overwritten by browser autofill.
- Fixed language install status on your profile not always updating after a successful install.

### v1.5.1 — See which lectures you've completed at a glance

**Added**
- Completed lectures now show an orange ring around their number in the section list, so it's easy to tell what you've already gone through.

### v1.5.0 — Light and grey themes, and smarter notes from Zero

**Added**
- Light and grey theme options, cycled from the header next to the update badge.
- Zero's notes about you now stay current, replaced when there's something new on the same topic instead of piling up.
- Zero's notes about you are more specific, naming the actual concept instead of a general observation.
- The profile page now shows your 4 most recent notes from Zero, with a "See more" option for the rest.

**Fixed**
- Fixed picking a local model from your profile sometimes still showing "No model set up" afterward, even though it was working.
- Fixed Python (and other tools) sometimes not being detected right after installing them on Windows.

### v1.4.2 — Mac updates no longer get stuck

**Added**
- A clear message with recovery steps if an update ever fails to install.

**Fixed**
- Fixed the Mac app's updater crashing partway through installing an update.

### v1.4.0 — JavaScript joins the DSA language lineup

**Added**
- JavaScript as a DSA language, no install needed - works in practice problems, mock interviews, and Ask Zero.

**Fixed**
- Fixed a crash on 13 problems where a solution returning nothing would error out instead of just failing the test.

### v1.3.0 — Bring your own AI, or skip it for now

**Added**
- The test-results panel in the DSA editor can now be resized, trading space with the code editor.
- Bring your own Claude or OpenAI API key instead of running a local model.
- A "Skip for now" option in setup, for reading lectures and practicing DSA problems without Zero.
- A "Get Ollama" button in your profile to add local Zero back later.
- Zero's replies now render bold text, lists, and code blocks properly, with a copy button on code.
- A text size control just for the lecture chat with Zero.
- A "move on without submitting code" option in the mock interview coding round.

**Fixed**
- Fixed Ollama installs and Gemma model downloads stopping if you left the profile page.
- Fixed a stuck Gemma download sometimes never finishing or responding to Cancel.
- Fixed "Get Ollama" re-downloading the whole app instead of just launching it when already installed.
- Fixed the DSA chat not scrolling to new messages from Zero.
- Fixed the interview coding round's Reset sometimes leaving the editor unresponsive.
- Fixed a never-installed default model incorrectly showing as "current".
- Fixed Ask Zero's code answers not matching the problem's real function signature.

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
