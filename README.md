# Kisses and Cuddles 🎮
*A high-performance, interactive Tic-Tac-Toe game featuring smooth graphics and matrix-based logic.*

🚀 **[View Source Code](https://github.com/RhysJPaterson/kisses-and-cuddles)** 🧑‍💻 **Developed by:** Rhys John Paterson

---

## 📌 Overview
**Kisses and Cuddles** is a modern implementation of the classic Tic-Tac-Toe game. Built using **Python** and **Pygame**, it serves as a showcase of 2D game development fundamentals, focusing on coordinate mapping, event-driven programming, and efficient state management.

The game provides a vibrant, responsive interface for two players to compete locally, featuring real-time win detection and automated game-state resets.

---

## 🎯 Purpose
The goal of this project was to:
- Implement a 2D grid system using **NumPy** for optimized game state tracking.
- Create a polished UI using Pygame's drawing primitives.
- Bridge different Python libraries (Pygame for gameplay and Tkinter for system-level notifications).

---

## 🚦 Core Features
- **Dynamic Grid Interaction**: Pixel-perfect collision detection that maps mouse clicks directly to a 3x3 logic matrix.
- **Visual Win Indicators**: Automated drawing of winning lines (horizontal, vertical, or diagonal) upon victory.
- **Smart Game Loop**: Efficiently handles inputs, rendering, and logic updates at a stable framerate.
- **Native Notifications**: Integration with Tkinter to provide clear "Game Over" and "Draw" pop-up alerts.
- **Quick Reset**: Instant board clearing and variable reset via the **'R'** key for seamless replayability.

---

## 🧠 Technical Challenges
### Why NumPy for a 3x3 Grid?
While a standard Python list could store a 3x3 grid, I chose **NumPy** to practice scalable data structures.
* **The Challenge**: Standard nested lists in Python can become cumbersome when checking for multi-directional win conditions.
* **The Solution**: Using a NumPy array allowed for cleaner matrix manipulation and potentially easier expansion into larger grid sizes (like 4x4 or 5x5) where mathematical array operations are much faster than nested loops.

### Cross-Library Integration
Integrating **Tkinter** for pop-up messages inside a **Pygame** loop can often cause window "freezing" or threading issues. I resolved this by ensuring the Tkinter root window is explicitly withdrawn (`root.withdraw()`) so that only the dialogue box appears, maintaining a clean user experience.

---

## 🛠 Tech Stack
- **Python**: Core programming language.
- **Pygame**: 2D graphics rendering and event handling.
- **NumPy**: Matrix management and mathematical operations.
- **Tkinter**: Native OS-level message boxes for user feedback.

---

## 📂 Installation & Setup
To run the game locally, follow these steps:

1.  **Clone the repository**:
    ```bash
    git clone [https://github.com/RhysJPaterson/kisses-and-cuddles.git](https://github.com/RhysJPaterson/kisses-and-cuddles.git)
    ```
2.  **Install requirements**:
    ```bash
    pip install pygame numpy
    ```
3.  **Launch the game**:
    ```bash
    python main.py
    ```

---

## ⚖️ License
This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

---

## 📣 Contact
**Rhys John Paterson**
* **Portfolio**: [rhysjpaterson.com](https://rhysjpaterson.com/)  
* **GitHub**: [@RhysJPaterson](https://github.com/RhysJPaterson)
