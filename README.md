## Welcome To My Sudoku Library
# Table Of Contents
1. Overview
2. Motivation
3. Key Features
4. Technical Focus & Learning
5. Project Structure
6. How the Solver Works
7. Future Enhancements
8. Why This Project Matters
# Overview
The Sudoku Algorithms Library is a standalone C# project implementing core Sudoku solving and generation algorithms. It serves as an algorithmic sandbox where I strengthened my foundations in recursion, backtracking, constraint satisfaction, and grid‑based data structures. This project reflects my early development as an engineer—building structured logic, learning to break problems into smaller components, and writing code I can explain, defend, and maintain.

The library is intentionally lightweight, modular, and testable, making it suitable for integration into larger applications or for educational use in understanding algorithmic reasoning.
# Motivation
My interest in this project comes from two places:

1. my background in **Combinatorics**, and
2. my long-standing hobby of solving Sudoku puzzles.

While most Sudoku solvers focus exclusively on the standard **9×9 grid**, I became curious about the mathematical structure of Sudoku in higher dimensions. This project was driven by a desire to explore Sudoku beyond the traditional format and investigate the combinatorial properties of generalized Sudoku boards.

Formally, I was interested in Sudoku grids of size:

$$n \in \\{x \in N \mid x \geq 4 \;\land\; \sqrt{x} \in N\\}$$

In other words, any $n \times n$ Sudoku grid where the sub-grid size $\sqrt{n}$ is also an integer (e.g., 4×4, 9×9, 16×16).

This curiosity led to two core questions:

1. **Enumeration Problem:**
   *Given a valid Sudoku dimension $n$, how many fully solved Sudoku grids exist?*
   (i.e., listing or generating all valid completed boards for a given $n$)

2. **Solving Problem:**
   *Given an nxn Sudoku puzzle, how can we solve it to completion using generalized constraint-satisfaction algorithms?*

The Sudoku Algorithms Library was built to explore these questions through structured C# implementations of:

- recursive backtracking
- constraint checking
- grid validation
- generalized $n \times n$ board generation

This project strengthened my foundations in algorithmic reasoning, recursion, and mathematical problem-solving while giving me a practical environment to apply concepts from combinatorics and discrete mathematics.
# Key Features
This library is designed to explore generalized Sudoku solving and enumeration for any valid grid size:  
$$n \in \\{x \in N \mid x \geq 4 \;\land\; \sqrt{x} \in N\\}$$
In other words, any $n \times n$ Sudoku grid where the sub-grid size $\sqrt{n}$ is also an integer (e.g., 4×4, 9×9, 16×16).  
The project supports two core capabilities:
1. **List All Solved $n \times n$ Sudoku Grids**
Generate or enumerate all fully solved Sudoku boards for a given valid dimension 𝑛. This feature explores the combinatorial structure of Sudoku and the mathematical question: "How many distinct completed Sudoku grids exist for a given n?
2. **Solving Any Valid $n \times n$ Sudoku Grid to Completion**
Solve generalized Sudoku puzzles using recursive backtracking and constraint‑satisfaction logic. The solver:
- Handles arbitrary valid grid sizes
- Applies row, column, and sub-grid constraints
- Uses depth-first search and backtracking
- Guarantees correctness for valid puzzles  
This feature addresses the mathematical question: "Given an $n \times n$ Sudoku puzzle, how can we solve it to completion using generalized algorithms?"