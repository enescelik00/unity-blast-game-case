# Unity Blast Puzzle Game

This project is a tile-based blast puzzle game developed with Unity.  
The core gameplay is inspired by classic collapse / blast mechanics where players remove groups of adjacent blocks with the same color to score points.

The project focuses on clean gameplay logic, grid-based systems, and performance-conscious implementation.

---

## Gameplay Overview

- The game board consists of a 2D grid filled with colored blocks.
- When the player clicks on a group of **2 or more adjacent blocks of the same color**, the group is destroyed.
- Blocks above the destroyed group **fall down due to gravity**.
- New blocks are spawned from the top to fill empty spaces.
- Each successful blast increases the player's score.

---

## Core Mechanics

### 🔹 Group Detection
- Adjacent blocks with the same color are detected as a group.
- Groups smaller than the minimum required size cannot be destroyed.
- The system dynamically recalculates groups after each move.

### 🔹 Gravity & Refill System
- After blocks are removed, remaining blocks fall vertically to fill empty cells.
- New blocks are spawned above the grid and dropped into place.
- The board always refills to a valid playable state.

### 🔹 Score System
- Each destroyed block contributes to the total score.
- Larger groups reward higher scores, encouraging strategic plays.

### 🔹 Visual State Changes
- Block visuals change based on the size of their connected group.
- As the number of adjacent blocks increases, different shapes/icons are displayed.
- This helps players identify larger groups more easily during gameplay.

---

## Technical Details

- **Engine:** Unity
- **Language:** C#
- **Architecture:** Grid-based game logic
- **Key Focus Areas:**
  - Efficient group detection
  - Clean separation of gameplay logic
  - Reusable and readable code structure
  - Runtime-safe gravity and refill logic

---

## Project Structure

- `Assets/` – Game scripts, sprites, and scenes  
- `Packages/` – Unity package dependencies  
- `ProjectSettings/` – Unity project configuration  

The project files are provided as a compressed archive for convenience.

---

## Notes

- All gameplay logic was implemented by me.
- Visual assets used in this project were provided as part of the original task and are used for demonstration purposes only.
- This project was developed as a small scoped gameplay prototype.

---

## Screenshots

<img width="320" height="573" alt="image" src="https://github.com/user-attachments/assets/21fdcbc6-b629-4d36-aff9-8a6dceca6f3e" />


*(You can add gameplay screenshots here to visually showcase the project.)*
