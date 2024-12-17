# Numerical-Methods-and-Linear-Systems-Analysis
This repository contains MATLAB scripts demonstrating various numerical methods for solving linear systems, least squares problems, and numerical approximations. Key topics include iterative solvers, direct matrix decomposition methods, cubic spline interpolation, Gaussian quadrature, and Poisson equation solutions.

# Description 
This repository contains MATLAB scripts implementing numerical methods and matrix operations:
- Iterative Solvers: Conjugate Gradient (CG.m)​, Gauss-Seidel (GS.m)​ and Jacobi Method (Jacobi.m)​
- Direct Solvers: Gaussian Elimination with Partial Pivoting (GEpivot.m)​ and Tridiagonal Matrix Solver (tridiag.m)​
- Applications: Cubic spline interpolation (cubspline.m)​, Gaussian quadrature weights calculation (gaussweights.m)​, Least squares approximation (lsq.m)​ and Solving the Poisson equation (poisson.m)​.

# Usage 
Each script is self-contained. To use a specific solver or application, execute the corresponding script in MATLAB. For example:
Conjugate Gradient Method: 
```matlab
A = [4, 1; 1, 3];
b = [1; 2];
x0 = zeros(size(b));
delta = 1e-6;
max_it = 1000;
[x, iflag, itnum] = CG(A, b, x0, delta, max_it);
```
Cubic Spline Interpolation: 
```matlab
n = 10; % Number of data points
[res, time, itnum] = cubspline(n);
```
## License
This project is licensed under the MIT License - see the LICENSE file for details.
```
Feel free to adjust any part of this README to better fit your specific needs or preferences.
