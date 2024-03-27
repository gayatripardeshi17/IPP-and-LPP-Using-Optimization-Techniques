# IPP-and-LPP-Using-Optimization-Techniques
IPP using a software package in Python



This code uses the PuLP library to solve a linear programming problem.
The problem is to maximize the profit from producing five different products (X1, X2, X3, X4, X5) subject to several constraints.

The objective function is to maximize the total profit, which is calculated by multiplying the profit per unit of each product by the number of units produced.

The constraints are:

* The total production time for all products cannot exceed 300 hours.
* The total production time for products X1, X2, and X3 cannot exceed 160 hours.
* The total production time for products X1, X2, X4, and X5 cannot exceed 150 hours.
* The production of each product is limited by its maximum capacity.

The code solves the problem using the GLPK solver and prints the optimal values of the decision variables and the optimal value of the objective function.

2)
This code solves the same linear programming problem using the SciPy library.
The code uses the linprog function to solve the problem.

The linprog function takes the following arguments:

* c: The objective coefficients.
* A_ub: The inequality constraints matrix.
* b_ub: The inequality constraints vector.
* A_eq: The equality constraints matrix.
* b_eq: The equality constraints vector.
* bounds: The bounds for the variables.
* method: The solver to use.

The code solves the problem using the highs solver and prints the optimal values of the decision variables and the optimal value of the objective function.


3)
This code solves the same linear programming problem using the OR-Tools library.
The code uses the pywraplp library to create a solver and solve the problem.

The pywraplp library provides a Python interface to the OR-Tools optimization suite.
The code creates a solver using the SCIP solver and defines the variables, objective function, and constraints.
The code then solves the problem and prints the optimal values of the decision variables and the optimal value of the objective function.

# All three codes solve the same linear programming problem and produce the same optimal solution. 
# The choice of solver depends on the user's preferences and the specific requirements of the problem.
