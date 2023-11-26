# Linear-programming-problem-solving-with-the-Gurobi-library
A Python script for solving linear programming models using the Gurobi library, enabling users to define variables, objectives, constraints, and perform sensitivity analysis. Note that this script focuses on solving linear optimization problems and does not include functionality for solving integer programming problems.


## Key Features

- **Variable Definition:** The script enables the definition of variables with non-negativity constraints and free variables.
- **Objective Function and Constraints:** Allows users to specify the objective function and constraints of the linear programming problem.
- **Sensitivity Analysis:** Provides sensitivity analysis for reduced costs and dual value ranges.

### Note on Constraints

- The library supports constraints in the form of `>=`, `<=`, or `=`.
- For strict inequalities (`>` or `<`), adjust the value slightly below or above the desired constraint value. Choose a small ε value that is significantly smaller than the problem's range to ensure it doesn't impact the solution.
- Example:
To represent a strict inequality like `X < 12`, use `X <= 12 - ε`. For instance, set epsilon to a value like `0.0001`, ensuring it's sufficiently small to avoid affecting the problem's solution.

## Usage

1. Run the `Linear programming problem solver.ipynb` script.
2. Follow the instructions to input the number of variables, objective function, and constraints.
3. The script will display the optimal solution of the problem and sensitivity analysis.


## Contribution

Contributions are welcome. If you have suggestions for improvement, please create an issue or submit a pull request.
