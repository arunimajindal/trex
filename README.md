# 🦕 T-Rex Runner

A browser-based clone of the iconic Chrome dinosaur game, built with [p5.js](https://p5js.org/) and [p5.play](https://molleindustria.github.io/p5.play/).

## 🎮 Demo

Open `index.html` in any modern browser to play instantly — no server or build step required.

## 🕹️ How to Play

- Press **Space** to jump over incoming obstacles
- Avoid cacti and other obstacles to keep running
- Your **score** increases the longer you survive
- The game speeds up progressively as your score climbs
- Hit restart to try again after a collision

## 🚀 Getting Started

```bash
git clone https://github.com/arunimajindal/trex.git
cd trex
# Open index.html in your browser
open index.html   # macOS
start index.html  # Windows
```

No npm, no build tools — just open and play.

## 🛠️ Built With

| Library | Purpose |
|---|---|
| [p5.js](https://p5js.org/) | Canvas rendering & game loop |
| [p5.play](https://molleindustria.github.io/p5.play/) | Sprite management & collision detection |
| [p5.sound](https://p5js.org/reference/#/libraries/p5.sound) | Audio support |
| Vanilla HTML/CSS | Page structure & styling |

## 📁 Project Structure

```
trex/
├── index.html          # Entry point
├── sketch.js           # Main game logic
├── style.css           # Page styles
├── p5.js               # p5.js library
├── p5.play.js          # p5.play sprite library
├── p5.dom.min.js       # p5 DOM utilities
├── p5.sound.min.js     # p5 sound utilities
├── trex1.png           # Dino running frame 1
├── trex3.png           # Dino running frame 2
├── trex4.png           # Dino running frame 3
├── trex_collided.png   # Dino collision frame
├── ground2.png         # Scrolling ground
├── cloud.png           # Background cloud
├── obstacle1–6.png     # Random obstacle sprites
├── gameOver.png        # Game over screen
└── restart.png         # Restart button
```

## ⚙️ Game Mechanics

- **Gravity** is simulated with a constant downward velocity on the dino sprite
- **Ground speed** increases with score: `velocity = -(6 + 3 * score / 100)`
- **Obstacles** are chosen randomly from 6 variants and spawned every 60 frames
- **Clouds** scroll at a fixed slower speed for a parallax effect
- **High score** is persisted in `localStorage` across sessions

## 🤝 Contributing

Pull requests are welcome! Feel free to open an issue for bug reports or feature suggestions.

## 📄 License

This project is open source. See the repository for details.
