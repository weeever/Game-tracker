# Quest Log 🎮

> A beautiful, premium, and gamified game backlog tracker with automated overlay notifications, Discord Rich Presence, and level-up mechanics.

---

Quest Log is a desktop application designed for gamers who want to organize their backlog, track their playtime, and turn their gaming achievements into a role-playing experience. Earn XP, gain levels, and accumulate gold as you complete your games!

---

## Key Features

* **Gamified Progression:** Earn XP and Gold coins as you play and complete games. Watch your level grow from a novice adventurer to a legendary gamer.
* **Smart Discord Rich Presence:** Automatically displays what you are playing, showing game covers in full HD (1080p via IGDB/Steam) alongside a custom status and interactive link to your gaming profile.
* **In-Game Overlay:** A premium, neon-themed custom overlay celebrating level-ups, game completion achievements, and toasts with custom line-art vector icons.
* **Auto-Completion Detection:** Analyzes unlocked achievements in real-time. Once the campaign or epilogue is finished, Quest Log triggers a celebratory banner and prepares a rating card for you.
* **Auto-Updater & Setup Installer:** Built-in seamless updates directly linked to GitHub Releases. Single-click setups create start menu entries, desktop shortcuts, and support silent tray starts on system boot.

---

## Architecture & Tech Stack

Quest Log is built with a lightweight, secure desktop architecture:

* **Core Framework:** Electron (HTML5, Vanilla CSS3, Javascript)
* **API Integrations:** IGDB (Internet Game Database) proxy & Steam Web API
* **Local Emulators Support:** Automated achievement tracking for local emulators (Goldberg, RUNE, CODEX)
* **Audio Synthesis:** In-app synthesizer using the Web Audio API for custom 8-bit sound effects (Level Up & Achievement bells)
* **Installer Engine:** NSIS (Nullsoft Scriptable Install System) for Windows setups

---

## Installation

### For Players

1. Download the latest installer from the [Releases](https://github.com/weeever/Game-tracker/releases) tab.
2. Run the `Quest Log Setup.exe` file.
3. Once installation completes, launch the app from your Desktop or Start Menu.
4. Set up your profile and start adding games to your backlog!

*Note: You can configure the application to run silently on startup (minimized in your system tray).*

---

## Development Setup

### Prerequisites

* [Node.js](https://nodejs.org/) (v16+ recommended)
* npm (comes with Node.js)

### Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/weeever/Game-tracker.git
   cd Game-tracker
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Launch the app in development mode:
   ```bash
   npm start
   ```

4. Compile the Windows NSIS Setup installer:
   ```bash
   npm run build
   ```
