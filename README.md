# ◎ PONG//DUO — two-player Pong

![macOS](https://img.shields.io/badge/macOS-Übersicht-3ef0ff?style=flat-square&logo=apple&logoColor=white&labelColor=040914) ![Vibecoded](https://img.shields.io/badge/vibecoded-with%20Claude-ff5ad9?style=flat-square&labelColor=040914)

Classic Pong for two people on one keyboard. Same height as the other widgets, three of them wide (714 × 314). No backend: the game runs entirely in the widget.

| File | What |
|:--|:--|
| `pongduo.jsx` | The whole game. Copy it into Übersicht's widgets folder and it works. |

## Play

**Click the field** to focus it. Clicking elsewhere pauses the game.

| Key | Action |
|:--|:--|
| W · S | left paddle up · down |
| ↑ · ↓ | right paddle up · down |
| Space / Enter | start / rematch |
| P / Esc | pause · R restart |

The ball bounces off the top and bottom walls. Get it past the other paddle for a point; **first to 7 wins**. Every paddle hit makes the ball 6 % faster (capped at 900 px/s); it drops back to the serve speed after each point and is served towards whoever just lost the point. Where it hits the paddle sets the angle (edge = 55°, centre = flat).

**Scores** (match wins per side, last match, best rally, matches played): `~/Library/Application Support/STUDYTERM/pongduo-scores`

## 🚀 Install

1. Download this repo (green **Code** button → *Download ZIP*) and double-click **`install.command`**. The first time, macOS may block it: right-click → *Open*.
   It installs [Übersicht](https://tracesof.net/uebersicht/) if you don't have it and copies `pongduo.jsx` into its widgets folder.
2. Click the widget to use it. If clicks fall through to the desktop: Übersicht menu-bar icon → this widget → turn on interaction.

- **Needs:** macOS 13+ · a screen at least ~800 px wide · nothing else, the game is a single file
- **By hand:** Copy `pongduo.jsx` into Übersicht's widgets folder (menu-bar icon → *Open Widgets Folder*).
- **Remove:** delete `pongduo.jsx` from the widgets folder.

## 🎨 Look and position

Out of the box it sits along the bottom in the cyan terminal theme. Install [**WIDGET//CTL**](https://github.com/SlicingReaper/widgetctl) to drag it anywhere on the grid (it takes three columns) and pick from 16 colour schemes × 8 styles, and to get `⌃⌥⌘W`, which hides all widgets at once.

## 🧩 Part of a collection

This widget is one of twelve that share the same retro-terminal look, the same theming and the same show/hide hotkey. Each works on its own; together they make a desktop dashboard.

| | Widget | What |
|:-:|:--|:--|
| 💰 | [**WALLET//Ð**](https://github.com/SlicingReaper/points-wallet-widget) | Points wallet: earn for habits, spend on rewards, lock savings, keep a streak |
| 🔥 | [**75//HARD**](https://github.com/SlicingReaper/75-hard-widget) | 75 Hard challenge tracker: 7 daily tasks, day counter, auto-fail on a missed day |
| ⏱️ | [**STUDY//TERM**](https://github.com/SlicingReaper/study-timer-widget) | Study stopwatch that logs what you did, with a stats page and points |
| ✎ | [**NOTE//PAD**](https://github.com/SlicingReaper/notepad-widget) | Checklist notes with deadline countdowns, auto-expiry and a bin |
| “ | [**QUOTE//DAY**](https://github.com/SlicingReaper/quote-of-the-day-widget) | A new quote every midnight from a pool of 300, with likes and your own quotes |
| ▦ | [**TETRIS//GRID**](https://github.com/SlicingReaper/tetris-widget) | Tetris on the desktop: hold, ghost piece, levels, best score |
| ◉ | [**PONG//SOLO**](https://github.com/SlicingReaper/pong-widget) | Single-player Pong: keep the ball up, it speeds up every hit |
| ◎ | [**PONG//DUO**](https://github.com/SlicingReaper/pong-duo-widget) ← you are here | Two-player Pong, 3 widgets wide: W/S vs ↑/↓, first to 7 |
| ⊞ | [**2048//TILE**](https://github.com/SlicingReaper/2048-widget) | 2048 with undo, keyboard or drag, saved between sessions |
| ⌂ | [**OUTPOST//**](https://github.com/SlicingReaper/outpost-colony-widget) | Colony-trading game: claim land, outfit robots, trade against 3 AI rivals |
| ☠ | [**DOOM//TERM**](https://github.com/SlicingReaper/doom-widget) | DOOM shareware Episode 1 in a 2-column widget: WebAssembly engine, savegames kept |
| 🎛️ | [**WIDGET//CTL**](https://github.com/SlicingReaper/widgetctl) | Menu-bar app that arranges and themes all the widgets, plus a ⌃⌥⌘W show/hide hotkey |

**Install all of them at once:** [`vibecoded` → install-all.command](https://github.com/SlicingReaper/vibecoded) · 🤖 Vibecoded with [Claude](https://claude.ai): I designed, directed and tested it, the AI wrote most of the code.
