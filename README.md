# Bubble Hit

**Pop, Splash, and Score!**  
A fast-paced reflex game where bubbles rise from the bottom, and you must click (or tap) them before they escape. Every pop adds +10 to your score, but let just one bubble reach the top — and it's game over!

<img width="1876" height="970" alt="image" src="https://github.com/user-attachments/assets/36cffb3b-546c-49b9-bfde-ec84760d21f9" />



---

## Features

-  **Rising bubbles** – Different sizes, colors, and speeds.
-  **Click or tap** – Play with mouse or touch (mobile friendly).
-  **Persistent High Score** – Your best score is saved in your browser.
-  **Explosive feedback** – Visual and text pop effects.
-  **Glossy bubble design** – With highlights and a playful underwater theme.
-  **Responsive layout** – Works on desktop, tablet, and mobile screens.
-  **Quick restart** – Instantly start a new game.

---

## How to Play

1. Click (or tap) on any bubble before it reaches the **top edge** of the screen.
2. Each popped bubble gives you **+10 points**.
3. If **any bubble touches the top**, the game ends.
4. Try to beat your own **high score**!

> **Tip:** Bubbles move at different speeds. Focus on the faster ones first!

---

## Game Logic

- Bubbles spawn continuously up to a **maximum of 45** on screen.
- Bubble radius: `24–48 px` • Speed: `0.65–1.65 px/frame`
- Score resets on game over, but the **highest score** remains until you beat it.
- Game over is triggered the moment a bubble’s top reaches `y ≤ 0`.

---

## Built With

- **HTML5 Canvas** – Smooth rendering and animations.
- **Vanilla JavaScript** – No external libraries or frameworks.
- **CSS3** – Gradient backgrounds, glassmorphism panels, and responsive design.

---

## Project Structure

```
bubble-hit-game/
├── index.html          # Complete game (HTML, CSS, JS)
└── README.md           # You are here
```

> The entire game is contained in a **single HTML file** – easy to deploy or modify.

---

## 🚀 How to Run Locally

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/bubble-hit.git
   cd bubble-hit
   ```

2. **Open the game**
   - Double-click `index.html` – it will open in your default browser.
   - Or use a local dev server (e.g., Live Server in VS Code).

3. **Start popping!** 🎈

---

## 📱 Mobile Play

The game works on touch devices:
- Tap directly on a bubble to pop it.
- Use the **NEW GAME** button to restart.
- All touch events are optimized with `preventDefault` to avoid zoom interference.

---

## 🧪 Customization Ideas

Want to tweak the game? Edit the constants at the top of the script section in `index.html`:

```javascript
const MAX_BUBBLES = 45;        // More bubbles = harder
const BASE_SPAWN_RATE = 32;    // Lower = faster spawn
const MIN_SPEED = 0.65;        // Increase for harder difficulty
const SCORE_PER_POP = 10;      // Points per pop
```

You can also:
- Change bubble colors in `COLOR_PALETTE`.
- Adjust canvas size (`width` / `height`).
- Modify the background gradient or light rays.

---

## 📄 License

MIT License – feel free to use, modify, and share.

---

## 🙌 Acknowledgments

- Inspired by classic “balloon pop” and arcade shooting games.
- Built with ☕ and lots of bubble physics.

