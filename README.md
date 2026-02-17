# Traveling-Salesman-Problem-TSP-Optimization-using-Genetic-Algorithms

A custom implementation of a Genetic Algorithm (GA) to solve the classic NP-hard Traveling Salesman Problem. This project focuses on optimizing the route for a 100-city dataset using evolutionary strategies, implemented entirely from scratch in Python.

## Algorithm Features

* **Custom Evolutionary Operators**: Hand-coded logic for population initialization, fitness evaluation, and selection.
* **Selection Strategy**: Tournament Selection (size k=5) to maintain healthy pressure and diversity.
* **Crossover Methods**: Implemented **Order-Based Crossover** to ensure valid permutations (no duplicate cities).
* **Mutation Strategies**: Includes multiple mutation types to avoid local optima:
  * Inversion Mutation
  * Scramble Mutation
  * Displacement Mutation
  * Insertion Mutation
* **Elitism**: Preservation of the top-performing individuals across generations to guarantee convergence.

##  Performance

The algorithm successfully reduced the route cost from an initial random state of **~43.20** to an optimized state of **~9.30**.

##  Built With

* **Python**: Core logic and algorithmic structure.
* **NumPy**: Efficient distance matrix calculations.
* **Matplotlib**: Route visualization and convergence plotting.
* **Pandas**: Dataset management.

## Visualization

The project includes a plotting utility to visualize the "Best Route Found," connecting 100 coordinates in a closed loop to minimize total Euclidean distance.
