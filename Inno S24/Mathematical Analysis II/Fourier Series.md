---
tags:
  - Math
  - MathematicalAnalysis
---
## Definition
- The series $$S(x)=\frac12a_0+\sum_{n=1}^\infty a_n\cos(nx)+b_n\sin(nx)$$
- There are specific points for $x$:
	- $\displaystyle x=2\pi k,k\in\mathbb Z: S(x)=\frac12a_0+\sum_{n=1}^\infty a_n$
	- $\displaystyle x=\frac\pi2+2\pi k,k\in\mathbb Z: S(x)=\frac12a_0+\sum_{n=1}^\infty b_n$ 
- In these cases the series are [[Absolute Convergence of Numeric Series|absolutely convergent]] uniformly of the interval $x\in[0,2\pi[$ if both series containing $a_n,b_n$ are [[Absolute Convergence of Numeric Series|absolutely convergent]] 
## Formulas for Coefficients
$$a_0=\frac1{\pi}\int_0^{2\pi}f(x)dx$$
$$a_n=\frac1\pi\int_0^{2\pi}f(x)\cos(nx)dx, n\in\mathbb N$$
$$b_n=\frac1\pi\int_0^{2\pi}f(x)\sin(nx)dx,n\in\mathbb N$$
## [[Complex Fourier Series]] 
