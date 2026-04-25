# Native Audio Editor

<h3 align="center">A fast, privacy-first audio editor and converter directly in your browser – zero uploads required.</h3>
<p align="center">No installs. No accounts. No uploads.</p>

<p align="center">
  <img src="https://img.shields.io/badge/version-1.0.0-blue.svg" alt="Version">
  <img src="https://img.shields.io/badge/dependencies-none-brightgreen" alt="Dependencies">
  <a href="#license">
    <img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License">
  </a>
</p>

---

## Table of Contents
- [Positioning](#positioning)
- [Why This Exists](#why-this-exists)
- [Comparison](#comparison)
- [Features](#features)
- [Screenshots](#screenshots)
- [Keyboard Shortcuts](#keyboard-shortcuts)
- [Quick Start](#quick-start)
- [Tech Stack](#tech-stack)
- [Customize / Extend It Yourself](#customize--extend-it-yourself)
- [Contributing](#contributing)

---

## Positioning

Native Audio Editor is built for:
- **Lightweight audio editing** without installing heavy software
- **Privacy-first local processing** where files never leave your device
- **Portable single-file deployment** with full user control
- A **zero-bloat alternative** for simple audio trimming and conversion tasks

---

## Why This Exists

Traditional desktop audio workspaces (DAWs) like Audacity or Logic are incredibly powerful, but they often come with steep learning curves, large installation sizes, and complex plugin ecosystems. On the other hand, many online audio editors force you to upload your sensitive files to remote servers, compromising privacy and introducing upload/download delays.

Native Audio Editor bridges this gap. It provides an accessible, fast-loading utility for everyday audio tasks—like trimming a podcast clip or converting a WAV to MP3—while ensuring 100% privacy and fast local performance. 

---

## Comparison

| Feature | Native Audio Editor | Traditional Desktop DAWs |
| :--- | :--- | :--- |
| **Installation Friction** | None (Single HTML file) | High (Downloads, installers, plugins) |
| **Privacy** | 100% Local (No uploads) | 100% Local |
| **Portability** | High (Runs in any browser) | Low (Tied to OS/Machine) |
| **Simple Edit Speed** | Instant | Moderate (App boot times, project setups) |
| **Offline Usage** | Yes | Yes |
| **Complexity Level** | Very Low | High |

---

## Features

- **Privacy-First Local Processing:** 100% client-side execution using the [Web Audio API](https://developer.mozilla.org/en-US/docs/Web/API/Web_Audio_API). Your files never leave your machine.
- **Waveform Audio Editing:** Visualize tracks with a custom-built, performant HTML5 [`<canvas>`](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API) engine.
- **Trim / Cut:** Precise, non-destructive editing workflows.
- **Undo / Redo:** Full history stack to easily reverse or re-apply your edits.
- **Format Converter:** Convert directly in the browser to WAV, MP3, OGG, and WebM with built-in adjustable bitrates.
- **Time Jump:** Hit `J` to instantly jump to specific timestamps.
- **Keyboard Shortcuts Help System:** Press `?` to view a comprehensive built-in shortcuts guide.
- **Single-File App:** Everything (HTML, CSS, JS) is cleanly packaged into one self-contained file.
- **Offline Capable:** Run it totally offline. No internet connection is ever needed after downloading the file.

---

## Screenshots

### Landing Page
![First Page](./First%20Page.png)
*The clean, intuitive dropzone interface for loading your audio.*

### Audio Editor
![Audio Editor](./Audio%20Editor.png)
*The main editing interface featuring the custom waveform, playback controls, and duration info.*

### Format Converter
![Format Converter](./Format%20Convertor.png)
*Convert your audio files directly in the browser to multiple formats with customizable bitrates.*

### Keyboard Shortcuts
![Help Page](./Help%20Page.png)
*Built-in interactive help modal detailing all professional keyboard shortcuts.*

---

## Keyboard Shortcuts

Speed up your workflow using built-in keyboard shortcuts:

| Key / Shortcut | Action |
| :--- | :--- |
| <kbd>Space</kbd> | Play / Pause |
| <kbd>S</kbd> | Stop audio |
| <kbd>Escape</kbd> | Stop audio and clear selection |
| <kbd>←</kbd> / <kbd>→</kbd> | Skip backward / forward by 5 seconds |
| <kbd>Ctrl</kbd> + <kbd>Z</kbd> | Undo last action |
| <kbd>Ctrl</kbd> + <kbd>Y</kbd> / <kbd>Shift</kbd> + <kbd>Z</kbd> | Redo last action |
| <kbd>Delete</kbd> / <kbd>Backspace</kbd> | Cut (delete selected region) |
| <kbd>T</kbd> | Trim (keep selected region) |
| <kbd>+</kbd> / <kbd>=</kbd> | Zoom In |
| <kbd>-</kbd> | Zoom Out |
| <kbd>0</kbd> | Reset Zoom (Zoom to Fit) |
| <kbd>J</kbd> | Open Time Jump prompt |
| <kbd>?</kbd> | Show Help & Shortcuts Modal |

---

## Quick Start

Since it is entirely a single-file application, there is no build process required to get started.

### Option 1: Run Locally
1. Download or clone this repository:
   ```bash
   git clone https://github.com/yourusername/native-audio-editor.git
   ```
2. Navigate into the folder:
   ```bash
   cd native-audio-editor
   ```
3. Just double-click on `audio-editor.html` to open it in any modern browser!

### Option 2: Host on GitHub Pages
Because the application is completely static, you can host it permanently for free on [GitHub Pages](https://pages.github.com/).
1. Fork this repository.
2. Go to **Settings** > **Pages**.
3. Select your main branch and save.
4. Your audio editor is live!

---

## Tech Stack

Built with native web standards:
- **HTML5** (Semantics & Structure)
- **CSS3 / Vanilla CSS** (Responsive UI, Animations, & Variables)
- **Vanilla JavaScript (ES6+)** (Zero frameworks, Zero build dependencies)
- **[Web Audio API](https://developer.mozilla.org/en-US/docs/Web/API/Web_Audio_API)** (Audio decoding, playback, and offline rendering)
- **[Canvas API](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API)** (Performant waveform visualization)

---

## Customize / Extend It Yourself

Because this is a simple, framework-free single-file app, it is highly extensible. You can easily copy the code into tools like GitHub Copilot or other AI coding assistants to add your own features.

Here are a few easy extensions you might consider building:
- **Fades:** Add simple fade in/out tools for the start or end of tracks.
- **Labels / Markers:** Add the ability to drop named markers on the timeline.
- **Batch Processing:** Allow dropping multiple files to convert them all at once.
- **Multitrack:** Expand the `<canvas>` to render and mix multiple audio files.
- **Transcription:** Hook up a local transcription model to generate subtitles.

---

## Contributing

We welcome contributions. If you have a feature idea, find a bug, or want to share your personal customizations, feel free to fork the project and open a Pull Request. Since it's a single file, it's incredibly easy to jump in and start tinkering.

---

## License

This project is licensed under the [MIT License](LICENSE).
