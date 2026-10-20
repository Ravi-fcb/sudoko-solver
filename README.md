# Sudoku Solver using C++

A **Sudoku Solver implemented in C++** using Object-Oriented Programming (OOP), recursion, backtracking, and the **Minimum Remaining Values (MRV)** heuristic to solve a standard 9×9 Sudoku puzzle efficiently.

## 📌 Project Overview

This project automatically solves a Sudoku puzzle by filling empty cells while satisfying all Sudoku rules. It uses a backtracking algorithm combined with the MRV heuristic to select the next cell with the fewest valid candidate numbers.

The program displays the original Sudoku puzzle alongside the solved board in the console.

## ✨ Features

- Solves standard 9×9 Sudoku puzzles.
- Uses **Backtracking** to explore possible solutions.
- Implements the **Minimum Remaining Values (MRV)** heuristic to select the next empty cell.
- Validates numbers against row, column, and 3×3 subgrid constraints.
- Displays the original and solved Sudoku boards side by side.
- Reports when no solution is found.
- Demonstrates Object-Oriented Programming concepts in C++.

## 🛠️ Technologies Used

- **Language:** C++
- **Concepts:** Object-Oriented Programming, Recursion, Backtracking, Constraint Checking, MRV Heuristic
- **Compiler:** GCC / G++ or any compatible C++ compiler

## 📂 Project Structure

```text
sudoko-solver/
├── source_code.cpp
├── OOPS PRESENTATION.pptx
├── OOPSSS.pdf
└── README.md
```

## ⚙️ How It Works

1. **Initialize the board:** The program stores the Sudoku puzzle in a 9×9 integer array. Empty cells are represented by `0`.
2. **Validate candidates:** It checks whether a number can be placed in a cell without violating Sudoku rules.
3. **Select an empty cell:** The MRV heuristic chooses an empty cell with the fewest valid candidate numbers.
4. **Apply backtracking:** The solver tries valid numbers recursively. If a choice leads to a dead end, it resets the cell and tries another number.
5. **Display the result:** Once the puzzle is solved, the program prints the original and completed boards side by side.

## 🚀 Getting Started

### Prerequisites

Install a C++ compiler such as GCC or G++.

Verify the installation:

```bash
g++ --version
```

### Compilation

Clone the repository:

```bash
git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
```

Navigate to the project directory:

```bash
cd YOUR-REPOSITORY
```

Compile the source code:

```bash
g++ source_code.cpp -o sudoku_solver
```

### Run the Program

On Linux or macOS:

```bash
./sudoku_solver
```

On Windows:

```bash
sudoku_solver.exe
```

## 🧩 Algorithm Used

### Backtracking

Backtracking is a recursive problem-solving technique that tries a candidate solution and reverses the choice if it cannot lead to a valid result.

### Minimum Remaining Values (MRV)

The MRV heuristic selects the empty cell with the smallest number of valid candidate values. This helps reduce unnecessary searches and can improve solving efficiency.

### Sudoku Rules

- Each row must contain the numbers 1–9 without repetition.
- Each column must contain the numbers 1–9 without repetition.
- Each 3×3 subgrid must contain the numbers 1–9 without repetition.

## 💻 Sample Output

The program displays the unsolved and solved boards side by side.

```text
Unsolved Board           ||       Solved Board
---------------------    ||   ---------------------
5 3 0 | 0 7 0 | 0 0 0    ||   5 3 4 | 6 7 8 | 9 1 2
6 0 0 | 1 9 5 | 0 0 0    ||   6 7 2 | 1 9 5 | 3 4 8
0 9 8 | 0 0 0 | 0 6 0    ||   1 9 8 | 3 4 2 | 5 6 7
...
```

*Note: The ellipsis represents the remaining rows of the board.*

## 🎯 Learning Outcomes

- Understanding OOP concepts through a practical C++ project.
- Implementing recursion and backtracking.
- Applying constraint checking to solve combinatorial problems.
- Learning how heuristics such as MRV improve search strategies.
- Developing problem-solving and algorithm-design skills.

## 🔮 Future Improvements

- Accept custom Sudoku puzzles from user input.
- Detect invalid or contradictory initial puzzles.
- Support puzzles with multiple solutions.
- Build a graphical user interface (GUI).
- Allow users to solve puzzles of different sizes.

