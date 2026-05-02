# 🎮 2048 — Python Tkinter

![Python](https://img.shields.io/badge/Python-3.7%2B-blue?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-green?style=flat-square)
![Platform](https://img.shields.io/badge/platform-Windows%20%7C%20macOS%20%7C%20Linux-lightgrey?style=flat-square)
![GUI](https://img.shields.io/badge/GUI-Tkinter-orange?style=flat-square)

A polished implementation of the classic **2048 puzzle game** built entirely with Python and Tkinter — no external dependencies required. Slide the tiles, merge the numbers, and reach the legendary **2048** tile!
---

## ✨ Features

- 🎮 **Classic 2048 mechanics** — faithful to the original game
- 🖥️ **Tkinter GUI** — clean, responsive graphical interface
- 📊 **Real-time score tracking** — score updates live as you play
- 🏆 **Persistent high score** — best score saved across sessions
- 🔄 **New game button** — restart anytime without closing the app
- 🎨 **Color-coded tiles** — distinct colors for every tile value
- ⌨️ **Keyboard controls** — arrow keys and WASD supported
- 📱 **Responsive design** — window adapts to different screen sizes
- 🚨 **Win / Game Over detection** — clear overlay messages with replay option
- ↩️ **Undo** — step back one move when you make a mistake

---

## 📸 Screenshot

```
┌──────────────────────────┐
│  2048        Score: 4096 │
│              Best:  8192 │
├──────┬──────┬──────┬─────┤
│      │   2  │  16  │  4  │
├──────┼──────┼──────┼─────┤
│   8  │  32  │      │  2  │
├──────┼──────┼──────┼─────┤
│      │  128 │  64  │  8  │
├──────┼──────┼──────┼─────┤
│   4  │   2  │  16  │ 512 │
└──────┴──────┴──────┴─────┘
```

---

## 🚀 Getting Started

### Prerequisites

- Python **3.6** or higher
- Tkinter (bundled with most Python installations)

> **Verify Tkinter is available:**
> ```bash
> python -m tkinter
> ```
> A small test window should appear. If not, see [Installing Tkinter](#installing-tkinter).

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/2048-python.git
   cd 2048-python
   ```

2. **Run the game**
   ```bash
   python main.py
   ```

That's it — no pip installs, no virtual environments needed.

---

## 🎯 How to Play

| Action | Keys |
|---|---|
| Move tiles | `↑` `↓` `←` `→` or `W` `A` `S` `D` |
| Undo last move | `U` or click **Undo** |
| New game | Click **New Game** |

**Rules:**
1. Tiles slide in the chosen direction until they hit a wall or another tile.
2. Two tiles with the **same number** merge into one with their **combined value**.
3. A new tile (**2** or **4**) spawns in a random empty cell after every move.
4. Reach the **2048** tile to win — but keep going for a higher score!
5. The game ends when **no moves remain**.

---

## 🗂️ Project Structure

```
2048-python/
├── main.py          # Entry point — launches the game window
├── game.py          # Core game logic (board, moves, merging)
├── gui.py           # Tkinter UI (tiles, colors, score display)
├── constants.py     # Tile colors, fonts, board size config
├── highscore.py     # Persistent high score (JSON/file storage)
└── README.md
```

---

## ⚙️ Configuration

Open `constants.py` to tweak the game:

```python
GRID_SIZE   = 4          # Board dimensions (4×4 default)
TILE_SIZE   = 100        # Pixel size of each tile
FONT_FAMILY = "Helvetica"
FONT_BOLD   = ("Helvetica", 36, "bold")

# Tile background colors
TILE_COLORS = {
    2:    "#eee4da",
    4:    "#ede0c8",
    8:    "#f2b179",
    16:   "#f59563",
    32:   "#f67c5f",
    64:   "#f65e3b",
    128:  "#edcf72",
    256:  "#edcc61",
    512:  "#edc850",
    1024: "#edc53f",
    2048: "#edc22e",
}
```

---

## 🛠️ Installing Tkinter

<details>
<summary><b>Ubuntu / Debian</b></summary>

```bash
sudo apt-get install python3-tk
```
</details>

<details>
<summary><b>Fedora / RHEL</b></summary>

```bash
sudo dnf install python3-tkinter
```
</details>

<details>
<summary><b>macOS (Homebrew)</b></summary>

```bash
brew install python-tk
```
</details>

<details>
<summary><b>Windows</b></summary>

Tkinter is included in the official Python installer from [python.org](https://www.python.org/downloads/). Make sure **tcl/tk and IDLE** is checked during installation.
</details>

---

## 🤝 Contributing

Contributions are welcome!

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/my-feature`
3. Commit your changes: `git commit -m "Add my feature"`
4. Push to the branch: `git push origin feature/my-feature`
5. Open a Pull Request

Please make sure your code follows PEP 8 and includes a brief description of your changes.

---

## 📋 Roadmap

- [ ] Animations for tile movement and merging
- [ ] 5×5 and 6×6 board size options
- [ ] Dark mode theme
- [ ] Sound effects
- [ ] Leaderboard with player names
- [ ] Mobile-friendly version (Kivy port)

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgements

- Original 2048 game by [Gabriele Cirulli](https://github.com/gabrielecirulli/2048)
- Inspired by the classic sliding puzzle concept

---

<p align="center">Made with ❤️ and Python</p>
