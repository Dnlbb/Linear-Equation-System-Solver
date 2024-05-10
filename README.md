# Linear Equation System Solver

### This Go program is designed to solve systems of linear equations using the Gaussian elimination method. It takes the dimension of the system N and the coefficients of the equations as input, and then outputs the solution of the system in the form of individual rational numbers.

## Functionality
* Input of the Equation System: The SLAY function takes the dimension of the system N and reads the coefficients of the equations from standard input. The coefficients are represented as rational numbers.

* Triangularization: The Triangular function transforms the system of equations into triangular form using the Gaussian elimination method. It performs the forward phase of the Gaussian elimination, finding the maximum element in each column and performing row swaps and row subtractions.

* Normalization of Equations: The Redukt function normalizes the diagonal elements in the triangular matrix by dividing each row by the corresponding diagonal element.

* Finding the Solution: The Otv_vect function finds the solution of the system of equations by performing the backward phase of the Gaussian elimination. If the system has no solution, the function returns a false flag.

* Output of the Result: In the main function, the helper functions are called, and the result is output to the standard output. If the system has no solution, the phrase "No solution" is printed. Otherwise, the values of the variables are printed as rational numbers.

## Input Format
The program takes the following input:

1. The dimension of the system N (an integer).
2. N lines, each containing N+1 rational numbers separated by spaces. The first N numbers in each line represent the coefficients of the equation, and the last number is the constant term.
## Output Format
* If the system has no solution, the program prints the phrase "No solution".
* If a solution exists, the program prints N lines, each containing a rational number in the form n/d, where n is the numerator, and d is the denominator.

## Usage Examples
Input:
```bash
3
-4 -1 8 2
7 -7 7 3
5 -1 -4 7
```
Output:
```bash
377/21
214/7
274/21
```
This example demonstrates a system of three equations with three variables, and the program outputs the values of these variables as rational numbers.



