---
tags:
  - Math
  - MathematicalAnalysis
  - DifferentialEquations
---
## Applications
- Let's find the solution for the equation
$$\frac{du}{dx}=ku,\;u=\sum_{n=0}^\infty u_nx^n$$
$$\sum_{n=1}^\infty nu_nx^{n-1}=k\sum_{n=0}^\infty u_nx^n$$
$$nu_n=ku_{n-1},u_{n+1}=\frac{k}{n}u_n, u_0=const, u_n=\frac{k^n}{n!}u_0, n>0$$
$$u(x)=\sum_{n=0}^\infty\frac{k^n}{n!}x^nu_0=u_0\sum_{n=0}^\infty\frac{(kx)^n}{n!}=u_0e^{kx}$$