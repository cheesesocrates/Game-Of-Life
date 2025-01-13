# Game-Of-Life
The .txt version of Conway's Game of Life

This repository contains an implementation of Conway's **Game of Life**, a fascinating simulation that demonstrates how simple rules can result in complex and lifelike behaviors. The program operates on a 30x30 grid of cells, where each cell can either be alive or dead. Over multiple generations, the grid evolves based on a set of rules, revealing interesting patterns and behaviors.

---

## Features
- **Grid Initialization**:
  - A 30x30 grid is used as the simulation environment.
  - Input data for the grid is loaded from a text file containing a matrix of `1`s and `0`s:
    - `1` represents a live cell.
    - `0` represents a dead cell.
  - The user is prompted to provide the file name for the initial grid setup.

- **Simulation Rules**:
  - A live cell with fewer than two neighbors dies (underpopulation).
  - A live cell with two or three neighbors survives.
  - A live cell with more than three neighbors dies (overpopulation).
  - A dead cell with exactly three neighbors becomes alive (restoration).

- **Simulation Execution**:
  - The user specifies the number of generations to simulate.
  - For each generation:
    - The current grid is displayed along with the generation number and the population count.
    - The next generation is calculated based on the Game of Life rules.
    - The console is cleared between generations to simulate animation.

- **File Output**:
  - After each generation, the updated grid is saved back to the same file from which it was initially loaded.

---

## How to Use
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/conways-game-of-life.git
   cd conways-game-of-life
