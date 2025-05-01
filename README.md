# N-Queens Solver Using Genetic Algorithm

This Python project solves the classic **N-Queens problem** using a **Genetic Algorithm (GA)** approach. The program evolves solutions where N queens are placed on an N×N chessboard such that no two queens threaten each other.

## Features

- Uses a genetic algorithm with population initialization, selection, crossover, and mutation operators.
- Supports any board size `N` specified by the user.
- Displays the best solution found after the algorithm finishes or a valid solution once discovered.
- Prints the solution board with `Q` representing queens and `.` representing empty spaces.

## How It Works

1. **Representation**: Each individual (candidate solution) is represented as a permutation list where the index corresponds to the row and the value to the column position of a queen.
2. **Fitness Function**: Evaluates the number of pairs of queens attacking each other (lower is better).
3. **Selection**: Selects the top half of the population with the lowest fitness scores.
4. **Crossover**: Uses an ordered crossover method to produce valid offspring from two parent solutions.
5. **Mutation**: Swaps two random positions in an individual with a small mutation rate to maintain diversity.
6. **Iteration**: Repeats selection, crossover, and mutation for a fixed number of generations or until a perfect solution is found.

## Requirements

- Python 3.x
- `numpy` package

Install numpy if you don’t have it already:

```bash
pip install numpy
