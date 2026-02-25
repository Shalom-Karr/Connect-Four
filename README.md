# 🔴 Connect Four

A sleek, modern, and responsive browser-based implementation of the classic strategy game. This version features a sophisticated AI opponent powered by the Minimax algorithm with Alpha-Beta pruning.

![Connect Four Preview](https://img.shields.io/badge/Game-Connect%20Four-red)
![AI Difficulty](https://img.shields.io/badge/AI-Minimax%20w/%20Alpha--Beta-yellow)
![Tech](https://img.shields.io/badge/Tech-HTML5%20%2F%20CSS3%20%2F%20JS-blue)

## 🚀 Features

-   **Advanced AI:** Play against a computer that thinks ahead. The AI evaluates thousands of potential future board states to find the optimal move.
-   **Difficulty Levels:**
    -   **Easy:** AI makes frequent mistakes and lacks foresight.
    -   **Medium:** A balanced challenge for casual players.
    -   **Hard:** Uses deep recursive look-ahead to block your moves and setup complex traps.
-   **Smooth Animations:** Gravity-based piece dropping using CSS transitions and timing functions.
-   **Responsive Design:** Fully playable on desktops, tablets, and smartphones.
-   **Win Highlighting:** Visual animation for the winning four-in-a-row combination.

## 🎮 How to Play

1.  **Objective:** Be the first to get four of your colored discs in a row (horizontally, vertically, or diagonally).
2.  **Your Turn:** Click on any column in the board. Your red disc will drop into the lowest available slot.
3.  **AI Turn:** The AI will automatically calculate its response based on the selected difficulty.
4.  **Winning:** The game detects a win immediately and highlights the winning connection.
5.  **Reset:** Use the "Reset" button to clear the board and start over.

## 🛠️ Technical Breakdown

### The AI Logic (Minimax + Alpha-Beta Pruning)
The core of the "Hard" mode is the **Minimax Algorithm**. 
-   **Minimax:** The AI simulates every possible move, then every possible response from the player, and so on, up to 7 moves deep. It assigns scores to board states (e.g., center control is rewarded; having 3-in-a-row with an open end is highly rewarded).
-   **Alpha-Beta Pruning:** This optimization technique allows the AI to "ignore" branches of the move tree that are guaranteed to be worse than previously explored options. This significantly speeds up computation, allowing the AI to look deeper into the future without lagging the browser.

### Styling & UI
-   **CSS Grid:** The board is built using a CSS Grid layout for perfect alignment.
-   **Modern Aesthetics:** Uses a "Dark Mode" palette (`#1a1a2e`) with vibrant accent colors for a premium feel.
-   **Interactive Layer:** A transparent "hitbox" layer sits above the board to handle user clicks without interfering with the piece-dropping animations.

## 📦 Installation

No installation is required. This is a portable, single-file application.

1.  Copy the code into a file named `index.html`.
2.  Open `index.html` in any modern web browser (Chrome, Firefox, Safari, Edge).
