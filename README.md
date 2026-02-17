# 🎮 Water Sort Puzzle Game

<div align="center">

![Python](https://img.shields.io/badge/Python-3.12.7-blue?logo=python&logoColor=white)
![Pygame](https://img.shields.io/badge/Pygame-2.6.1-green?logo=python&logoColor=white)
![WebAssembly](https://img.shields.io/badge/WebAssembly-WASM-654FF0?logo=webassembly&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-yellow.svg)
![Platform](https://img.shields.io/badge/Platform-Web%20%7C%20Desktop%20%7C%20Mobile-orange)

**An interactive browser-based puzzle game built with Python and Pygame, compiled to WebAssembly**

[🎮 Play Live](https://parth-r-kunkunkar.itch.io/water-sort-puzzle-game) • [📝 Report Bug](https://github.com/yourusername/water-sort-puzzle/issues) • [✨ Request Feature](https://github.com/yourusername/water-sort-puzzle/issues)

![Game Screenshot](https://via.placeholder.com/800x400/2d3436/ffffff?text=Add+Your+Game+Screenshot+Here)

</div>

---

## 📖 Table of Contents

- [About](#about)
- [Features](#features)
- [Demo](#demo)
- [Tech Stack](#tech-stack)
- [Getting Started](#getting-started)
- [How to Play](#how-to-play)
- [Game Mechanics](#game-mechanics)
- [Project Structure](#project-structure)
- [Code Highlights](#code-highlights)
- [Deployment](#deployment)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)
- [Contact](#contact)

---

## 🧪 About

Water Sort Puzzle is an addictive browser-based puzzle game where players strategically sort colored liquids into test tubes. Built entirely in Python using the Pygame framework and compiled to WebAssembly with Pygbag, this project demonstrates modern web game development techniques while maintaining the simplicity and readability of Python code.

The game features progressive difficulty levels, intelligent hint systems, smooth particle-based animations, and full cross-platform support including desktop and mobile devices.

### 🎯 Project Goals

- Demonstrate Python game development with Pygame
- Showcase Python-to-WebAssembly compilation using Pygbag
- Implement engaging game mechanics with smooth animations
- Create a fully playable cross-platform web game
- Practice object-oriented programming and game design patterns

---

## ✨ Features

### Core Gameplay
- 🧪 **Liquid Sorting Mechanic** - Pour colored liquids between test tubes
- 🎯 **Progressive Difficulty** - 12+ levels with increasing complexity (3-10 colors)
- 🏆 **Victory System** - Celebrate completing levels with particle effects
- 🎨 **12 Vibrant Colors** - Rich color palette for visual appeal

### Player Controls
- 🔄 **UNDO System** - Reverse any move with complete history tracking
- 🔃 **RESET Option** - Restart current level at any time
- 💡 **Smart Hints** - Intelligent two-pass algorithm suggests best moves
- 🚫 **Stuck Detection** - Alerts when no valid moves are available

### Visual & UX
- ✨ **Particle Physics** - Gravity-based celebration effects
- 🌊 **Pour Animation** - Smooth arc trajectory with realistic liquid flow
- 🎭 **Tube Shake** - Visual feedback for invalid moves
- 💫 **Selection Highlight** - Golden outline for selected tubes
- 🖱️ **Hover Effects** - Interactive feedback for buttons and tubes

### Technical
- 📱 **Mobile Support** - Touch controls for phones and tablets
- 🖥️ **Desktop Support** - Mouse controls for computers
- 🌐 **Cross-Platform** - Runs in any modern web browser
- ⚡ **60 FPS Performance** - Smooth gameplay on all devices
- 🎮 **No Installation** - Play directly in browser

---

## 🎬 Demo

### 🎮 Play Online
**Live Game:** [https://parth-r-kunkunkar.itch.io/water-sort-puzzle-game](https://parth-r-kunkunkar.itch.io/water-sort-puzzle-game)

### 📸 Screenshots

<div align="center">

| Gameplay | Victory Screen | Hint System |
|----------|----------------|-------------|
| ![Gameplay](https://via.placeholder.com/250x200/636e72/ffffff?text=Gameplay) | ![Victory](https://via.placeholder.com/250x200/00b894/ffffff?text=Victory) | ![Hint](https://via.placeholder.com/250x200/fdcb6e/ffffff?text=Hints) |

| Mobile View | Particle Effects | No Moves Alert |
|-------------|------------------|----------------|
| ![Mobile](https://via.placeholder.com/250x200/0984e3/ffffff?text=Mobile) | ![Particles](https://via.placeholder.com/250x200/6c5ce7/ffffff?text=Particles) | ![Alert](https://via.placeholder.com/250x200/d63031/ffffff?text=Alert) |

</div>

### 🎥 Video Demo
> *[Add your YouTube or video link here]*

---

## 🛠️ Tech Stack

### Core Technologies
- **Python 3.12.7** - Primary programming language
- **Pygame 2.6.1** - Game development framework
- **Pygbag** - Python to WebAssembly compiler
- **WebAssembly (WASM)** - Browser execution format

### Libraries & Modules
```python
pygame      # Graphics, events, rendering
random      # Level generation, randomization
math        # Physics calculations, animations
asyncio     # Web browser compatibility
```

### Web Technologies
- **HTML5** - Game container and canvas
- **JavaScript** - Runtime loader and initialization
- **CSS** - Basic styling (generated by Pygbag)

### Development Tools
- **Visual Studio Code** - Code editor
- **Git** - Version control
- **GitHub** - Repository hosting
- **itch.io** - Game deployment platform

---

## 🚀 Getting Started

### Prerequisites

Ensure you have the following installed:
- **Python 3.12+** ([Download](https://www.python.org/downloads/))
- **pip** (comes with Python)
- **Git** ([Download](https://git-scm.com/downloads))

### Installation

#### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/water-sort-puzzle.git
cd water-sort-puzzle
```

#### 2. Install Dependencies
```bash
pip install -r requirements.txt
```

Or install manually:
```bash
pip install pygame==2.6.1
pip install pygbag
```

#### 3. Run Locally (Desktop)
```bash
python main.py
```

The game window will open and you can play using mouse controls.

#### 4. Build for Web
```bash
pygbag .
```

This will:
- Compile Python to WebAssembly
- Generate HTML/JS wrapper files
- Start a local web server
- Open your browser to `http://localhost:8000`

The compiled files will be in the `build/web/` directory.

---

## 🎮 How to Play

### Objective
Sort all colored liquids so that each test tube contains only one color.

### Controls

#### Desktop (Mouse)
- **Left Click** - Select a tube (first click) or pour to another tube (second click)
- **UNDO Button** - Reverse the last move
- **RESET Button** - Restart the current level
- **HINT Button** - Get a suggestion for the next move

#### Mobile (Touch)
- **Tap** - Select a tube (first tap) or pour to another tube (second tap)
- **Tap Buttons** - UNDO, RESET, or HINT

### Rules

1. ✅ **Valid Moves:**
   - Pour liquid from one tube to another
   - Can pour onto matching color
   - Can pour into empty tube
   - Multiple units of same color pour at once

2. ❌ **Invalid Moves:**
   - Cannot pour if destination is full
   - Cannot pour different colors onto each other
   - Cannot pour from empty tube

3. 🏆 **Winning:**
   - Each tube must contain 4 units of the same color
   - OR be completely empty
   - All tubes must be "complete"

### Tips
- 💡 Use empty tubes strategically as temporary storage
- 🎯 Try to complete one color at a time
- 🔄 Don't be afraid to use UNDO - it's there to help!
- 💭 Use HINT when stuck - it shows the best available move

---

## 🎲 Game Mechanics

### Progressive Difficulty System

The game automatically increases difficulty as you progress:

| Level Range | Colors | Empty Tubes | Total Tubes |
|-------------|--------|-------------|-------------|
| 1-3         | 3      | 2           | 5           |
| 4-7         | 4      | 1           | 5           |
| 8-11        | 5      | 1           | 6           |
| 12-15       | 6      | 1           | 7           |
| 16+         | 7-10   | 1           | 8-11        |

**Formula:**
```python
num_colors = 3 + ((level - 1) // 4)  # +1 color every 4 levels
num_empty_tubes = max(1, 2 - ((level - 1) // 2))  # Reduces to 1 after level 3
```

### Hint Algorithm

The intelligent hint system uses a **two-pass search strategy**:

**Pass 1: Strategic Moves** (Priority)
- Looks for moves that combine matching colors
- Prefers non-empty destination tubes
- Better long-term strategy

**Pass 2: Any Valid Move**
- Searches for moves to empty tubes
- Only if no strategic moves exist
- Ensures a move is always suggested if possible

**No Moves Detection**
- If both passes fail → Player is stuck
- Displays "NO PLAYABLE MOVES AVAILABLE"
- Suggests using UNDO or RESET

### Physics & Animations

#### Particle System
```python
# Each particle has:
- Position (x, y)
- Velocity (vx, vy)
- Gravity acceleration (0.3 pixels/frame²)
- Lifespan (60 frames = 1 second)
- Alpha fade-out effect
```

#### Pour Animation Arc
```python
# Creates realistic liquid trajectory:
t = animation_progress (0.0 to 1.0)
x = linear_interpolation(start_x, end_x, t)
y = linear_interpolation(start_y, end_y, t) + sin(t * π) * 30
# The sine wave creates the curved arc effect
```

---

## 📂 Project Structure
```
water-sort-puzzle/
│
├── main.py                 # Main game file (800+ lines)
│   ├── Game                # Core game logic and state management
│   ├── Tube                # Test tube class (pouring, validation)
│   ├── Particle            # Particle physics for effects
│   ├── PourAnimation       # Liquid pouring animation
│   └── Button              # UI button components
│
├── images.jpg              # Background image asset
│
├── README.md               # Project documentation (this file)
├── requirements.txt        # Python dependencies
├── .gitignore              # Git ignore rules
├── LICENSE                 # MIT License
│
└── build/                  # Generated by Pygbag (not committed)
    └── web/
        ├── index.html      # Web entry point
        ├── main.py         # Game code
        ├── images.jpg      # Assets
        └── *.wasm          # WebAssembly binaries
```

### Class Architecture
```
Game (Main Controller)
├── Manages game state and level progression
├── Handles user input (mouse/touch events)
├── Coordinates rendering and updates
└── Controls game loop (async for web)

Tube (Game Object)
├── Stores colored liquid units
├── Validates pour operations
├── Handles selection and hover states
└── Renders tube with liquids

Particle (Visual Effect)
├── Physics simulation (velocity, gravity)
├── Alpha transparency fade-out
└── Automatic lifecycle management

PourAnimation (Animation Controller)
├── Manages particle generation
├── Creates arc trajectory
└── Signals completion

Button (UI Component)
├── Click/touch detection
├── Hover state management
└── Text rendering
```

---

## 💻 Code Highlights

### 1. Intelligent Hint System
```python
def find_available_move(self):
    """Two-pass search for best available move"""
    
    # PASS 1: Strategic moves (combine matching colors)
    for from_tube in self.tubes:
        if not from_tube.is_empty():
            for to_tube in self.tubes:
                if (from_tube != to_tube and 
                    from_tube.can_pour_to(to_tube) and 
                    not to_tube.is_empty()):
                    return (from_tube, to_tube)
    
    # PASS 2: Any valid move (including empty tubes)
    for from_tube in self.tubes:
        if not from_tube.is_empty() and not from_tube.is_complete():
            for to_tube in self.tubes:
                if (from_tube != to_tube and 
                    from_tube.can_pour_to(to_tube) and 
                    to_tube.is_empty()):
                    return (from_tube, to_tube)
    
    return (None, None)  # No moves available - stuck!
```

### 2. Arc Trajectory Animation
```python
# Creates realistic liquid pouring arc
t = min(self.progress * 1.2, 1.0)  # Interpolation factor
x = start_x + (end_x - start_x) * t  # Linear X movement

# Y movement with sine wave arc
y = start_y + (end_y - start_y) * t + math.sin(t * math.pi) * 30

self.particles.append(Particle(x, y, self.color))
```

### 3. WebAssembly Compatibility
```python
# Async game loop for browser compatibility
async def run(self):
    running = True
    while running:
        self.clock.tick(60)  # 60 FPS
        
        # Handle events, update, render...
        
        await asyncio.sleep(0)  # Yield to browser
    
    pygame.quit()

# Entry point
if __name__ == "__main__":
    game = Game()
    asyncio.run(game.run())
```

### 4. Mobile Touch Support
```python
for event in pygame.event.get():
    # Desktop: Mouse events
    if event.type == pygame.MOUSEBUTTONDOWN:
        self.handle_click(mouse_pos)
    
    # Mobile: Touch events
    if event.type == pygame.FINGERDOWN:
        touch_x = int(event.x * WIDTH)
        touch_y = int(event.y * HEIGHT)
        self.handle_click((touch_x, touch_y))
```

### 5. Particle Physics
```python
class Particle:
    def update(self):
        self.vy += 0.3  # Gravity acceleration
        self.x += self.vx  # Horizontal movement
        self.y += self.vy  # Vertical movement (affected by gravity)
        self.life -= 1     # Countdown to fade-out
    
    def draw(self, screen):
        alpha = int(255 * (self.life / 60))  # Fade effect
        # Draw semi-transparent particle...
```

---

## 🌐 Deployment

### Deploy to itch.io (Recommended)

1. **Build the game:**
```bash
pygbag .
```

2. **Prepare upload:**
```bash
cd build/web
# Select ALL files inside this folder
# Create a ZIP file
```

3. **Upload to itch.io:**
   - Go to [itch.io](https://itch.io) and create account
   - Click "Upload New Project"
   - Fill in game details:
     - **Title:** Water Sort Puzzle Game
     - **Project URL:** your-game-name
     - **Classification:** Games
     - **Kind of project:** HTML
     - **Viewport:** 800 × 600 px
   - Upload your ZIP file
   - Check ☑️ "This file will be played in the browser"
   - Click "Save & View Page"

4. **Configure settings:**
   - ☑️ Mobile friendly
   - ☑️ Automatically start on page load
   - ☑️ Fullscreen button
   - Set pricing to FREE

### Deploy to GitHub Pages
```bash
# Create gh-pages branch
git checkout -b gh-pages

# Copy build files
cp -r build/web/* .

# Commit and push
git add .
git commit -m "Deploy to GitHub Pages"
git push origin gh-pages
```

Enable GitHub Pages in repository settings → Pages → Source: gh-pages branch

### Other Hosting Options
- **Netlify** - Drag and drop `build/web/` folder
- **Vercel** - Connect GitHub repository
- **Firebase Hosting** - `firebase deploy`

---

## 🤝 Contributing

Contributions make the open-source community amazing! Any contributions you make are **greatly appreciated**.

### How to Contribute

1. **Fork the Project**
2. **Create your Feature Branch**
```bash
   git checkout -b feature/AmazingFeature
```
3. **Commit your Changes**
```bash
   git commit -m 'Add some AmazingFeature'
```
4. **Push to the Branch**
```bash
   git push origin feature/AmazingFeature
```
5. **Open a Pull Request**

### Contribution Ideas
- 🎵 Add sound effects and background music
- 🎨 Create new visual themes (dark mode, neon, etc.)
- 🏆 Implement achievement system
- 📊 Add leaderboard functionality
- 🎮 Create level editor
- 🌍 Add internationalization (i18n)
- ♿ Improve accessibility features
- 📱 Optimize mobile performance

### Bug Reports

Found a bug? Please open an issue with:
- Clear description of the problem
- Steps to reproduce
- Expected vs actual behavior
- Screenshots (if applicable)
- Browser/device information

---

## 📊 Project Statistics

- **Lines of Code:** 800+
- **Classes:** 5
- **Methods/Functions:** 30+
- **Color Variations:** 12
- **Supported Platforms:** 6+ (Windows, Mac, Linux, Android, iOS, Web)
- **Supported Browsers:** 5+ (Chrome, Firefox, Edge, Safari, Opera)
- **Frame Rate:** 60 FPS
- **Resolution:** 800×600 pixels
- **Average Load Time:** 3-5 seconds

---

## 📜 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.
```
MIT License - Copyright (c) 2026 Parth R. Kunkunkar
```

**TL;DR:** You can use, modify, and distribute this project freely, even commercially, as long as you include the original license.

---

## 🙏 Acknowledgments

### Technologies
- [Pygame](https://www.pygame.org/) - Python game development framework
- [Pygbag](https://github.com/pygame-web/pygbag) - Python to WebAssembly compiler
- [itch.io](https://itch.io/) - Free game hosting platform

### Inspiration
- Classic water sort puzzle games
- Mobile puzzle game mechanics
- Web-based game development tutorials

### Resources
- [Pygame Documentation](https://www.pygame.org/docs/)
- [WebAssembly Docs](https://webassembly.org/)
- [Python Documentation](https://docs.python.org/3/)

---

## 📞 Contact

**Parth R. Kunkunkar**

- GitHub: [@yourusername](https://github.com/yourusername)
- itch.io: [Play the Game](https://parth-r-kunkunkar.itch.io/water-sort-puzzle-game)
- Project Link: [https://github.com/yourusername/water-sort-puzzle](https://github.com/yourusername/water-sort-puzzle)

---

## 🔮 Future Roadmap

- [ ] **Sound & Music**
  - Pour sound effects
  - Victory fanfare
  - Background music
  - Mute toggle

- [ ] **Advanced Features**
  - Daily challenges
  - Timed mode
  - Move counter
  - Star rating system (3 stars based on moves)

- [ ] **Social Features**
  - Global leaderboard
  - Share scores
  - Challenge friends

- [ ] **Customization**
  - Multiple themes (dark, neon, minimal)
  - Custom color palettes
  - Different tube shapes
  - Background selection

- [ ] **Gameplay Enhancements**
  - Level editor
  - Custom levels
  - Puzzle solver mode
  - Replay system

- [ ] **Technical Improvements**
  - Local storage for progress
  - PWA (Progressive Web App)
  - Offline play
  - Performance optimizations

---

<div align="center">

## ⭐ Star This Repository!

If you found this project helpful or interesting, please consider giving it a star! ⭐

**[🎮 Play the Live Game](https://parth-r-kunkunkar.itch.io/water-sort-puzzle-game)**

---

Made with ❤️ and Python | © 2026 Parth R. Kunkunkar

</div>
