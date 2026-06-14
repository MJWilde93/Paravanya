# 🏔️ Paravanya — Mountain of Shadows

A Castlevania-inspired side-scrolling action platformer built with Python and Pygame. Fight skeleton enemies across a parallax mountain landscape, level up through waves, and survive as long as you can.

![Python](https://img.shields.io/badge/Python-3.9+-3a7bd5?style=flat-square&logo=python&logoColor=white)
![Pygame](https://img.shields.io/badge/Pygame-2.5+-7ee8c2?style=flat-square)
![License](https://img.shields.io/badge/License-MIT-f4a261?style=flat-square)

---

## 🎮 Gameplay

- Side-scrolling parallax world with 5 background layers
- Animated thief player character with walk, jump, idle, and 9-frame combo attack
- Skeleton enemies with patrol AI, aggro states, and scaling difficulty
- Double jump, attack combos, and particle hit effects
- Health drop system — skeletons have a 35% chance to drop a heart on death
- Level progression — kill quota per level, escalating enemy size and spawn rate
- Score system based on enemy size and current level

---

## 🕹️ Controls

| Key | Action |
|-----|--------|
| `A` / `←` | Move left |
| `D` / `→` | Move right |
| `Space` / `↑` / `W` | Jump (double jump supported) |
| `Z` | Attack (press again during combo window for follow-up) |
| `R` | Restart (Game Over screen) |
| `ESC` / `Q` | Quit |

---

## 🚀 Installation & Running

**Requirements:** Python 3.9+ and Pygame 2.5+

```bash
# Clone the repo
git clone https://github.com/yourusername/paravanya.git
cd paravanya

# Install dependencies
pip install -r requirements.txt

# Run the game
python castlevania_mountain.py
```

---

## 📁 Project Structure

```
paravanya/
├── castlevania_mountain.py   # Main game — all logic in one file
├── requirements.txt
├── README.md
└── assets/
    ├── parallax-mountain-bg.png
    ├── parallax-mountain-montain-far.png
    ├── parallax-mountain-mountains.png
    ├── parallax-mountain-trees.png
    ├── parallax-mountain-foreground-trees.png
    ├── parallax-mountain-music.flac
    ├── wall128x128.png
    ├── thief_idle.png
    ├── walk1.png – walk6.png
    ├── jump1.png – jump2.png
    ├── attack1.png – attack9.png
    ├── skel_idle.png
    ├── skel_walk1.png – skel_walk5.png
    ├── skel_attack1.png – skel_attack5.png
    └── skel_damage1.png – skel_damage2.png
```

---

## 🛠️ Technical Highlights

- **Parallax scrolling** — 5 independent background layers with configurable scroll speeds
- **Sprite animation system** — frame-based animation with configurable tick rates per state
- **Enemy AI state machine** — idle → patrol → aggro → chase → attack → stagger
- **Combo system** — two-hit attack chain with a time-limited follow-up window
- **Particle system** — physics-based particles with gravity, alpha fade, and size decay
- **Level manager** — kill-based progression with dynamic difficulty scaling for enemy size, spawn rate, and max count
- **Health drop system** — bobbing animated hearts with a pickup radius and fade-out on expiry

---

## 🎨 Credits

Parallax mountain background and music assets from [free game art resources](https://opengameart.org).

---

*Built by Madison · Phoenix, AZ · [Portfolio](https://yourusername.github.io)*
