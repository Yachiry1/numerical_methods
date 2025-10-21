# numerical_methods
# Jacobi Method Solver

This project implements the **Jacobi iterative method** to solve systems of linear algebraic equations (SLAE) of the form:

\[
A \cdot x = b
\]

where `A` is a square coefficient matrix, `b` is the right-hand side vector, and `x` is the solution vector.

## Features

- Reads input from `input.txt` (matrix `A` and vector `b` in numeric table format).  
- Checks if `A` is diagonally dominant and rearranges rows if necessary to improve convergence.  
- Solves the system iteratively using the Jacobi method with a configurable tolerance and maximum iterations.  
- Stores the first 10 iterations for inspection.  
- Writes output to `output.txt`, including:
  - Solution vector `x`
  - Convergence flag
  - Number of iterations
  - Residual norm \(\|Ax-b\|_\infty\)
  - Condition number of the matrix
  - Values from the first 10 iterations

## Usage

1. Prepare `input.txt` with the system of equations.  
2. Run the program:

```bash
python main.py
