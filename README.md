# 🎮 Enemy Chase Game – A* Pathfinding Visualizer

An interactive grid-based chase game and algorithm visualizer powered by the **A* Search Algorithm**. Built using vanilla HTML5 Canvas, JavaScript, and Tailwind CSS, this project provides a real-time hands-on simulation of AI pathfinding dynamics.

---

## ✨ Features

- **Real-Time A* Pathfinding:** The AI enemy recalculates the shortest path to the player in real time using Manhattan distance as its heuristic function.
- **Interactive Level Editor:** Click or drag across the grid to dynamically place or clear wall obstacles during gameplay.
- **Path Overlay Visualizer:** Toggle visual path cues to see the calculated shortest route nodes targeted by the AI enemy.
- **Responsive & Mobile-Friendly:** Designed using Tailwind CSS with an integrated touch D-Pad for mobile devices.
- **Adjustable Difficulty:** Modify the enemy's speed dynamically using an intuitive slider mechanism.
- **Zero External Dependencies:** Built with pure HTML5 Canvas and vanilla JavaScript.

---

## 🕹️ How to Play

1. **Objective:** Outrun and evade the red AI enemy block for as long as possible while accumulating points.
2. **Player Controls:**
   - **Keyboard:** `Arrow Keys` or `W`, `A`, `S`, `D` to navigate.
   - **Mobile / Mouse:** Use the on-screen D-Pad.
3. **Level Editing:**
   - **Click/Drag** on open grid spaces to place wall obstacles (`#`).
   - **Click/Drag** on existing walls to remove them.
   - Use the **Clear All Walls** button to reset the map layout.

---

## 🚀 Quick Start

No installation or build step is required!

1. Clone or download this repository:
   ```bash
   git clone https://github.com/purvat2008/mini-project
   ```
2. Open `chase game.html` directly in any web browser.

---

## 🛠️ Built With

* **HTML5 Canvas** - Grid rendering and real-time graphics handling.
* **JavaScript (ES6+)** - Game loop logic and A* algorithm implementation.
* **Tailwind CSS** - UI design and layout structure.

---

## 🧠 Algorithmic Details

The enemy AI tracks the player using the **A* Search Algorithm**:
- **Evaluation Function:** $f(n) = g(n) + h(n)$
  - $g(n)$: The cost of the path from the starting node to node $n$.
  - $h(n)$: The estimated cost from node $n$ to the goal using **Manhattan Distance**:
    $$h(n) = |x_1 - x_2| + |y_1 - y_2|$$
- **Priority Queue:** Orders frontier nodes by $f(n)$ score to expand optimal nodes first.

---

## 📄 License

This project is licensed under the MIT License - feel free to modify and share!
