#  Rocket's Ship - Alien Invasion Game

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue.svg)](https://www.python.org/downloads/)
[![Pygame](https://img.shields.io/badge/Pygame-2.0%2B-green.svg)](https://www.pygame.org/)
[![License](https://img.shields.io/badge/License-MIT-brightgreen.svg)](#license)

**A classic 2D space shooter game built with Python and Pygame where you pilot a rocket ship through waves of alien invaders!** 

Defend Earth from extraterrestrial threats in this action-packed arcade-style game featuring dynamic difficulty scaling, persistent high scores, and smooth gameplay mechanics.

![Game Screenshot](https://github.com/Ashish1455/Space-Game/blob/main/game_overview.png?raw=true)

---

## 🎮 Game Features

### Core Gameplay
- **🚀 Rocket Ship Control**: Smooth 4-directional movement with responsive controls
- **💥 Bullet System**: Fire up to 5 bullets simultaneously with realistic physics
- **👽 Alien Fleet**: Face organized alien formations that move toward you
- **🎯 Collision Detection**: Precise hit detection for bullets, aliens, and ship
- **⚡ Dynamic Difficulty**: Game speed and alien points increase with each level

### Progression System
- **📊 Real-time Scoring**: Earn 50+ points per alien (increases with level)
- **🏆 High Score Tracking**: Persistent high score system across game sessions
- **🎚️ Level Progression**: Advancing levels with increasing challenge
- **❤️ Lives System**: Start with 3 ships, lose one when hit by aliens
- **🔄 Game Restart**: Click "Play" button to restart after game over

### Visual & Audio
- **📱 Clean UI**: Score, high score, level, and remaining ships display
- **🖱️ Mouse Support**: Click-to-play functionality with visual feedback
- **⌨️ Keyboard Controls**: Intuitive arrow key movement and spacebar shooting

---

## 🛠️ Installation & Setup

### Prerequisites
- **Python 3.10+** installed on your system
- **pip** package manager

### Quick Start Guide

1. **Clone the Repository**
   ```bash
   git clone https://github.com/Ashish1455/Space-Game.git
   cd Space-Game
   ```

2. **Install Dependencies**
   ```bash
   pip install pygame
   ```

3. **Launch the Game**
   ```bash
   python run_game.py
   ```
---

## 🎯 Game Controls

| Control | Action | Description |
|---------|--------|-------------|
| **⬆️ Up Arrow** | Move Up | Navigate ship upward |
| **⬇️ Down Arrow** | Move Down | Navigate ship downward |
| **⬅️ Left Arrow** | Move Left | Navigate ship left |
| **➡️ Right Arrow** | Move Right | Navigate ship right |
| **Spacebar** | Fire Bullet | Shoot at aliens (max 5 bullets) |
| **Q Key** | Quit Game | Exit the game immediately |
| **Mouse Click** | Start Game | Click "Play" button to begin |

---

## 📁 Project Structure

This game follows a modular architecture with clear separation of concerns:

| File | Purpose | Key Features |
|------|---------|--------------|
| **`run_game.py`** | 🎮 Main Game Loop | Entry point, initializes all components |
| **`settings.py`** | ⚙️ Configuration Manager | Screen size (1200x800), speeds, colors, limits |
| **`ship.py`** | 🚀 Player Ship Class | Movement, rendering, collision detection |
| **`alien.py`** | 👽 Enemy Alien Class | AI movement, edge detection, fleet behavior |
| **`bullet.py`** | 💥 Projectile System | Bullet physics, rendering, lifecycle |
| **`game_functions.py`** | 🧠 Core Game Logic | Event handling, collisions, fleet management |
| **`game_stats.py`** | 📊 Statistics Tracker | Score, lives, level, high score persistence |
| **`scoreboard.py`** | 🏆 UI Display System | Score rendering, level display, ship counter |
| **`button.py`** | 🔘 UI Button Component | Play button, click detection, visual feedback |
| **`Images/`** | 🎨 Game Assets | `ship.bmp`, `alien.bmp` sprite files |

### Architecture Overview
```
Space-Game/
├── run_game.py          # Main game loop and initialization
├── settings.py          # Global game configuration
├── ship.py              # Player ship mechanics
├── alien.py             # Enemy alien behavior
├── bullet.py            # Projectile system
├── game_functions.py    # Core game logic and utilities
├── game_stats.py        # Statistics and progression tracking
├── scoreboard.py        # UI and display management
├── button.py            # Interactive UI elements
├── Images/
│   ├── ship.bmp        # Player ship sprite
│   └── alien.bmp       # Alien enemy sprite
└── game_overview.png    # Game screenshot
```

---

## 🎲 How to Play

### Getting Started
1. **Launch the Game**: Run `python run_game.py`
2. **Start Playing**: Click the green "Play" button or press any key
3. **Control Your Ship**: Use arrow keys to move around the screen
4. **Attack Aliens**: Press spacebar to fire bullets at the alien fleet

### Gameplay Mechanics
- **Objective**: Destroy all aliens in each wave to advance to the next level
- **Lives**: You have 3 ships; lose one when aliens hit your ship or reach the bottom
- **Scoring**: Earn points for each alien destroyed (base: 50 points, increases per level)
- **Progression**: Each level increases game speed and alien point values
- **Game Over**: When all ships are lost, click "Play" to restart

---

## 🔧 Technical Specifications

### Game Settings
- **Screen Resolution**: 1200x800 pixels
- **Frame Rate**: Controlled by Pygame's display system
- **Ship Speed**: 1.5 pixels/frame (increases per level)
- **Bullet Speed**: 3.0 pixels/frame (increases per level)
- **Alien Speed**: 0.5 pixels/frame (increases per level)
- **Max Bullets**: 5 simultaneous bullets allowed

---
## 🗺️ Roadmap & Future Features

### Planned Enhancements
- 🎵 **Sound Effects**: Shooting, explosions, and background music
- 💾 **Save System**: Persistent game progress and statistics
- 🎮 **Multiple Ship Types**: Different ships with unique abilities

### Version History
- **v1.0** - Core gameplay implementation with all basic features

---

##  Acknowledgments

- **Pygame Community**: For the excellent game development framework
- **Python Software Foundation**: For the Python programming language
- **Classic Arcade Games**: Inspiration from Space Invaders and similar games
- **Open Source Community**: For continuous support and contributions
