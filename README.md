# Traveling Salesman Problem Optimization with Genetic Algorithms

A custom Python implementation of a Genetic Algorithm for solving the Traveling Salesman Problem (TSP), an NP-hard route optimization problem. The project optimizes a 100-city route using evolutionary search techniques implemented from scratch.

## Project Overview

The Traveling Salesman Problem asks for the shortest possible route that visits each city exactly once and returns to the starting point. Because the search space grows extremely quickly, this project uses a Genetic Algorithm to find a strong approximate solution efficiently.

## Results

The algorithm reduced route cost from an initial random state of approximately `43.20` to an optimized route cost of approximately `9.30`, showing a major improvement through selection, crossover, mutation, and elitism.

## Tech Stack

- Python
- NumPy
- Pandas
- Matplotlib

## Algorithm Components

- Population initialization for candidate routes
- Fitness evaluation based on route distance
- Tournament selection with `k = 5`
- Order-Based Crossover to preserve valid city permutations
- Multiple mutation strategies:
  - Inversion mutation
  - Scramble mutation
  - Displacement mutation
  - Insertion mutation
- Elitism to preserve the strongest routes between generations

## Visualization

The project includes route and convergence plots to show:

- Best route found across 100 coordinates
- Route improvement over generations
- Convergence behavior of the genetic search process

## How to Run

```bash
git clone https://github.com/marcelngoyi90/Traveling-Salesman-Problem-TSP-Optimization-using-Genetic-Algorithms.git
cd Traveling-Salesman-Problem-TSP-Optimization-using-Genetic-Algorithms
pip install numpy pandas matplotlib jupyter
jupyter notebook
```

## Future Improvements

- Add benchmark comparisons against nearest-neighbor and 2-opt heuristics.
- Add configurable population size, mutation rate, and generation count.
- Save final route visualizations as images for the README.
- Package the algorithm into reusable Python modules.
