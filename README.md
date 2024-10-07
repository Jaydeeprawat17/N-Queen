# N Queen Problem - Backtracking Approach

This repository contains a solution to the **N Queen Problem** using the **Backtracking** approach in C++. The N Queen problem is a classic problem in which the task is to place `N` queens on an `N x N` chessboard such that no two queens can attack each other.

## Overview

The **N Queen Problem** is a fundamental example of a constraint satisfaction problem, where we need to find ways to place `N` queens on a chessboard such that:
1. No two queens are in the same row.
2. No two queens are in the same column.
3. No two queens are on the same diagonal.

This solution uses the **Backtracking** approach to try placing queens one by one, and if placing a queen leads to a conflict (violation of the conditions), it backtracks and tries a new position.

## Algorithm

The **Backtracking** approach tries to place a queen in each column one by one. It checks if placing a queen in the current position is safe:
- If the position is safe, it moves forward to place the next queen.
- If placing the queen causes a conflict, it backtracks and tries a different column in the previous row.

### Key Functions:
- `solve()`: This is a recursive function that tries to place queens on the board.
- `safe()`: This function checks whether placing a queen at a given position is safe.
- `validPlace()`: This function checks whether two queens are placed on the same diagonal or column.

## Prerequisites

- Turbo C++ or any C++ compiler.
- Basic understanding of C++ and recursion.
- Knowledge of the N Queen Problem.


## How to Run

### Step 1: Clone the repository

### Step 2: Compile the code using Turbo C++ or any C++ compiler

If you're using Turbo C++, follow these steps:
1. Open Turbo C++.
2. Copy the code from `n_queen.cpp` and paste it in a new file.
3. Save the file.
4. Compile the program by pressing `Alt + F9`.
5. Run the program by pressing `Ctrl + F9`.

For other C++ compilers (e.g., g++):
```bash
g++ n_queen.cpp -o n_queen
./n_queen

