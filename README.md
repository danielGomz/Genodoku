# 🧬 Genodoku — Genetic Algorithm Sudoku Solver

**Genodoku** is an experimental Sudoku solver powered by a genetic algorithm. Instead of backtracking or brute force, it evolves populations of candidate solutions until it finds a valid one — all while showing its progress in real time.

> 🧩 Think of it as Darwin playing Sudoku.

---

## 🚀 Features

- Load Sudoku puzzles from `.csv` files
- Real-time graphical interface:
  - Displays the evolving Sudoku board
  - Tracks generation count and fitness
- Custom genetic algorithm:
  - Handles fixed cells correctly
  - Selection, crossover, and mutation
  - Tunable parameters
- Written entirely in Haskell 💚

---

## 🧠 How it Works

1. **Input**: Load a puzzle from a CSV file.
2. **Initialization**: Generate a random population of complete boards, respecting the fixed cells.
3. **Evolution**: Over generations:
   - Select the fittest candidates
   - Combine them with crossover
   - Mutate them slightly
   - Keep the elites
4. **Goal**: Reach a Sudoku grid with **no conflicts** in rows, columns, or 3×3 boxes.

---

## 📂 Project Structure

