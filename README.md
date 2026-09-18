<p align="center">
  <a href="https://vibetyper.com"><img src="https://vibetyper.com/assets/images/common/logo.png" alt="Vibe Typer" width="96"></a>
</p>

<h1 align="center">Vibe Typer</h1>

<p align="center">
  AI voice typing for Linux, Windows, macOS and iPhone.<br>
  Hold a hotkey, talk, and clean text lands at your cursor in any app.
</p>

<p align="center">
  <a href="https://vibetyper.com">Website</a> ·
  <a href="https://vibetyper.com/downloads">Download</a> ·
  <a href="https://vibetyper.com/features">Features</a> ·
  <a href="https://vibetyper.com/pricing">Pricing</a> ·
  <a href="https://vibetyper.com/docs">Docs</a> ·
  <a href="https://discord.com/invite/s43JqaGxsZ">Discord</a> ·
  <a href="https://github.com/vibetyper/vibe-typer-official/issues">Issues</a>
</p>

<p align="center">
  <a href="https://vibetyper.com/downloads"><img alt="Linux, Windows, macOS and iOS" src="https://img.shields.io/badge/platforms-Linux%20%7C%20Windows%20%7C%20macOS%20%7C%20iOS-4c1?style=flat-square"></a>
  <a href="https://vibetyper.com/pricing"><img alt="Free plan" src="https://img.shields.io/badge/free%20plan-2%2C000%20words%20a%20month-blue?style=flat-square"></a>
  <a href="https://apps.apple.com/app/vibe-typer/id6787101284"><img alt="App Store" src="https://img.shields.io/badge/App%20Store-iPhone-black?style=flat-square&logo=apple"></a>
  <a href="https://discord.com/invite/s43JqaGxsZ"><img alt="Discord" src="https://img.shields.io/badge/Discord-join-5865F2?style=flat-square&logo=discord&logoColor=white"></a>
  <a href="https://x.com/vibetyper"><img alt="X" src="https://img.shields.io/badge/X-%40vibetyper-000?style=flat-square&logo=x"></a>
</p>

<p align="center">
  <img src="https://vibetyper.com/images/app/history-diff-light-1120.webp" alt="Vibe Typer history showing the Magic Formatter diff between what was said and what was typed" width="800">
</p>

## What it is

Vibe Typer is a system-wide AI dictation app, built in Australia. Press a hotkey in whatever app is in front, Slack, a terminal, VS Code, Gmail, Word, a browser form, say what you mean, and let go. Magic Formatter strips the ums, false starts and self-corrections on the way through, and the finished text is typed at your cursor. No window to copy out of, no plugin per app, nothing to learn beyond one hotkey.

It runs natively on Linux (Wayland and X11), Windows and macOS, and as a dictation keyboard on iPhone. One account covers all of them.

## Why people switch to it

- **It just works.** Install, set a hotkey, talk. No models to download, no dependencies, no per-app setup.
- **Fast on any machine.** Transcription runs on our servers, on large speech models and inference hardware built for speed, not on your CPU. Let go of the hotkey and the text lands before your hand is back on the keyboard, on a five-year-old laptop as much as on a workstation. The models that transcribe best are the ones consumer hardware runs slowest, which is why local tools make you choose between accuracy and waiting.
- **Text you can send without editing.** Magic Formatter cleans fillers, self-corrections, grammar and punctuation, and can fix mistranscriptions, then shows you a word-level diff of what it changed. Custom instructions and three tone settings make it write the way you do.
- **Configurable where it matters.** A dictionary with Smart, Whole word and Exact phrase matching that offers to learn from your corrections. Per-app paste rules. A second hotkey, mouse-button bindings, and hooks that run shell commands when recording starts and stops.
- **Linux is a first-class citizen.** One AppImage for Ubuntu, Fedora, Debian, Arch and Mint. Native text insertion on both Wayland and X11, no xdotool, no ydotool. Wispr Flow and Superwhisper do not ship a Linux build.
- **Nothing kept.** Audio is processed in memory on our servers and discarded. No recordings, no transcripts, no training on your voice. History stays on your device.

## Install

| Platform | Requirements | Download |
|---|---|---|
| Linux | Modern 64-bit distribution, X11 or Wayland | [VibeTyper.AppImage](https://cdn.vibetyper.com/releases/linux/VibeTyper.AppImage) |
| Windows | Windows 10 or later, 64-bit | [vibe-typer-Setup.exe](https://cdn.vibetyper.com/releases/windows/vibe-typer-Setup.exe) |
| macOS | macOS 12 Monterey or later, Apple Silicon | [VibeTyper-arm64.dmg](https://cdn.vibetyper.com/releases/mac/VibeTyper-arm64.dmg) |
| iPhone | iOS 17 or later | [App Store](https://apps.apple.com/app/vibe-typer/id6787101284) |

Android is in development.

### Linux

```bash
curl -LO https://cdn.vibetyper.com/releases/linux/VibeTyper.AppImage
chmod +x VibeTyper.AppImage
./VibeTyper.AppImage
```

Sign in with the one-time code sent to your email (no passwords), grant microphone access, keep the default hotkey (Ctrl + Space) or set your own, and dictate. The same AppImage runs on GNOME, KDE, COSMIC, Hyprland and Sway. On Wayland, run the in-app Wayland setup once so hotkeys and text insertion work. Sign-in needs a Secret Service keyring; see [keyring troubleshooting](https://vibetyper.com/docs/linux-keyring-troubleshooting) if your desktop does not ship one. Full notes: [voice typing on Linux](https://vibetyper.com/voice-typing-linux).

### Windows and macOS

Run the installer or open the disk image, sign in, grant the permissions it asks for, and press Ctrl + Space.

### iPhone

Install from the App Store, enable the "Vibe Typer Dictation" keyboard in iOS Settings, and switch to it in any app. Magic Formatter, custom instructions, tone and your dictionary carry over from desktop.

## Features

Every feature is available on the free plan. Pro removes the monthly caps.

**Dictation**

- Hold to talk or press to toggle, up to 5 minutes a take. Esc cancels, F8 re-pastes the last take.
- Works in any app, including full-screen apps, terminals and code editors. Automatic mode picks the right paste method per app (Ctrl + Shift + V in Linux terminals, for example) and you can override it per app.
- 99 languages. Tell it up to five you speak and it detects between them, or have it follow your keyboard layout.
- Pause sensitivity so it waits while you think, mutes other apps while you record, and a microphone switcher in the tray.

**Magic Formatter**

- On by default. Cleans fillers, self-corrections, grammar and punctuation, and can fix mistranscriptions. Never translates, never summarises, never changes numbers, names, prices or technical terms.
- Custom instructions: style preferences applied to every dictation, such as "always use Australian spelling".
- Tone: Normal, Casual, Very Casual.
- A word-level diff of every change, so you can see what it did and tune it.

**AI commands** (desktop)

- Rewrite: select any text, press the hotkey, say how you want it changed.
- Reply: draft a response to what is on screen.

**Dictionary and learning**

- Smart, Whole word or Exact phrase matching, no entry cap, synced to every device including the iPhone keyboard.
- Learn from my corrections: when you fix a word it got wrong, it offers to add the fix. Runs locally, and nothing is added until you accept it.

**Control and automation**

- A second hotkey and mouse-button bindings (Mouse3, Mouse4, Mouse5).
- [Hooks](https://vibetyper.com/docs/hooks): run a shell command before recording starts and after it stops. Pause your music with playerctl, flip a light, set a status.
- Preferences sync, launch at startup, automatic updates, opt-in beta releases.

**History and activity**

- Local history with the diff, search and re-insert. Saving audio is off by default and device-local.
- Activity: time saved measured against your own typing speed, words, dictations, words per minute, streak.

## Privacy

- Transcription runs in the cloud. Audio is held in memory only while it is transcribed, then dropped. No recordings are stored.
- Transcripts, prompts and AI outputs are returned to your device and are not stored on our servers.
- Nothing trains on your audio or text. Our providers are bound to no-retention and no-training terms.
- History, saved audio and correction-learning observations stay on your device.
- Stored server-side: account details, usage counts, synced settings and your dictionary. Delete them any time under Settings > Account.

Full policy: [vibetyper.com/privacy](https://vibetyper.com/privacy). Detail: [local history and privacy](https://vibetyper.com/docs/local-history-and-privacy).

## Pricing

| | Free | Pro |
|---|---|---|
| Transcribed words | 2,000 a month | Unlimited |
| AI operations (Rewrite and Reply) | 20 a month | Unlimited |
| Magic Formatter, custom instructions, dictionary, every platform | Included | Included |
| Price | $0, no card | $8 a month billed annually, or $10 month to month |

Business seats with central billing are available for teams. Details at [vibetyper.com/pricing](https://vibetyper.com/pricing).

## Compared with Wispr Flow and Superwhisper

Checked 18 September 2026 against each vendor's site.

| | Vibe Typer | Wispr Flow | Superwhisper |
|---|---|---|---|
| Linux | Yes, Wayland and X11 | No | No |
| Windows | Yes | Yes | Yes |
| macOS | Yes | Yes | Yes |
| iPhone | Yes | Yes | Yes |
| Android | In development | Yes | Yes |
| Free plan | 2,000 words a month | 2,000 words a week on desktop | 3,000 words of Pro features to trial |
| Pro | $8 a month annual, $10 monthly | $12 a month annual, $15 monthly | From $8.49 a month |

Guides: [Wispr Flow on Linux](https://vibetyper.com/blog/wisprflow-alternative-linux-guide) · [Superwhisper on Linux](https://vibetyper.com/blog/superwhisper-alternative-linux-guide) · [Wispr Flow vs Vibe Typer](https://vibetyper.com/blog/wispr-flow-vs-vibe-typer) · [Every dictation tool that runs on Linux](https://vibetyper.com/blog/best-ai-voice-typing-apps-linux)

## About this repository

Vibe Typer's application source is closed. This repository is the official public home of the project and exists to:

- **Track issues.** Bug reports and feature requests go in [Issues](https://github.com/vibetyper/vibe-typer-official/issues). Include your OS and version, your desktop environment and whether you are on X11 or Wayland if on Linux, the app version, and the [diagnostics bundle](https://vibetyper.com/docs/support-diagnostics) if you can.
- **Verify authenticity.** This is the only official GitHub repository for Vibe Typer. Repositories using the name Vibe Typer or variations of it are not affiliated with us. Download only from [vibetyper.com](https://vibetyper.com/downloads), cdn.vibetyper.com or the App Store.
- **Take security reports privately.** Email [support@vibetyper.com](mailto:support@vibetyper.com) rather than opening a public issue.

## Support and community

- Docs: [vibetyper.com/docs](https://vibetyper.com/docs)
- Help: [vibetyper.com/support](https://vibetyper.com/support) or [support@vibetyper.com](mailto:support@vibetyper.com)
- Discord: [discord.com/invite/s43JqaGxsZ](https://discord.com/invite/s43JqaGxsZ), where feature requests and Linux distro quirks get worked out
- Updates: [@vibetyper on X](https://x.com/vibetyper)

## Releases

The desktop apps update themselves, and you can opt into beta releases under Settings. Release notes are shown in the app after each update.

---

<p align="center">Made in Australia · © Vibe Typer · All rights reserved</p>
