## Particle Swarm Optimization (PSO) – Python Implementation

This project demonstrates the **Particle Swarm Optimization (PSO)** algorithm, a nature-inspired optimization technique based on the collective behaviour of birds and fish.

The implementation focuses on solving a mathematical minimization problem:

\[
f(x) = x^2
\]

Subject to:

\[
-10 \leq x \leq 10
\]

### Objective

The objective is to find the value of `x` that produces the minimum value of the objective function. The theoretical optimal solution is:

- **Optimal value of x:** 0
- **Minimum function value:** 0

### Algorithm Overview

The PSO algorithm works with a group of particles, where each particle represents a possible solution. Particles continuously update their positions and velocities using their individual best-known position (Pbest) and the best position found by the entire swarm (Gbest).

The implementation follows these steps:

1. Initialize a swarm of 30 particles with random positions and velocities.
2. Calculate the fitness value of each particle using the objective function.
3. Identify the Personal Best (Pbest) and Global Best (Gbest).
4. Update particle velocities using inertia, cognitive and social components.
5. Update particle positions within the defined search boundaries.
6. Repeat the process for 100 iterations.
7. Display the best solution and visualize the optimization process.

### Parameters Used

| Parameter | Value |
|---|---:|
| Swarm Size | 30 |
| Maximum Iterations | 100 |
| Inertia Weight (w) | 0.7 |
| Cognitive Coefficient (c1) | 1.5 |
| Social Coefficient (c2) | 1.5 |
| Search Range | [-10, 10] |

### Technologies Used

- **Python** – Programming language
- **NumPy** – Numerical computations
- **Matplotlib** – Graph visualization

### Visualizations

The implementation generates two graphs:

1. **PSO Convergence Graph:** Displays how the best fitness value changes over successive iterations.
2. **Objective Function Graph:** Displays the function \(f(x)=x^2\) and the best solution obtained by PSO.

### How to Run

Install the required libraries:

```bash
pip install numpy matplotlib
```

Run the Python file:

```bash
python pso_implementation.py
```

### Expected Outcome

The algorithm searches for the minimum of the objective function and should converge towards:

\[
x = 0,\quad f(x) = 0
\]

### Purpose of the Project

This implementation is part of a review study on **Evolutionary Computation and Swarm Optimization**. It provides a practical demonstration of how Particle Swarm Optimization can be applied to a mathematical optimization problem.
