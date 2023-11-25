
# Fletcher-Reeves Conjugate Gradient Implementation
This repository presents a pure Python implementation of the Fletcher-Reeves Conjugate Gradient method. This optimization algorithm is particularly effective for large-scale problems and is implemented here from the ground up. It includes a numerical approach to gradient calculation and a backtracking line search for optimal step size determination.

## Features
Numerical Gradient Calculation: Computes gradients numerically for any given function.
Backtracking Line Search: Employs a simple yet effective line search algorithm to find the optimal step size.
Fletcher-Reeves Update: Utilizes the Fletcher-Reeves formula for updating conjugate directions.

## Example Usage
The fletcher_reeves_step_by_step function is versatile and can be applied to a variety of objective functions, including but not limited to:

Quadratic Function: f(x) = x[0]^2 + x[1]^2
Rosenbrock Function: f(x) = (1 - x[0])^2 + 100 * (x[1] - x[0]^2)^2
Sphere Function: f(x) = sum(x^2)
Rastrigin Function: f(x) = 10 * len(x) + sum(x^2 - 10 * cos(2 * pi * x))
Challenging Objective Functions
To test the robustness of the algorithm, the following challenging functions are also included:

Saddle Point Function: f(x) = x[0]^2 - x[1]^2
Himmelblau's Function: f(x) = (x[0]^2 + x[1] - 11)^2 + (x[0] + x[1]^2 - 7)^2
Eggholder Function: f(x) = -(x[1] + 47) * sin(sqrt(abs(x[0]/2 + (x[1] + 47)))) - x[0] * sin(sqrt(abs(x[0] - (x[1] + 47))))
Getting Started
To use this implementation:

Clone this repository.
Import the fletcher_reeves_step_by_step function into your Python script.
Define or select an objective function.
Execute the function with an initial guess, for example: fletcher_reeves_step_by_step(rosenbrock, x0=[0, 0]).
Dependencies
NumPy
