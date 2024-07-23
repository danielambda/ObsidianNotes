---
tags:
  - Math
  - MathematicalAnalysis
---
## Theorem
- If $R$ is the [[Theorem about the Radius of Convergence|Radius of Convergence]], then $$\frac 1 R=\rho=\lim_{n=0}\sqrt[n]{|a_n|}$$
## Proof 
- We consider only the case $0<\rho<+\infty$
$$\forall\varepsilon\in\mathbb R, \varepsilon > 0\;\exists N\in\mathbb N\;\forall n\in\mathbb N, n>N:|a_n||x|^n\leq(\rho+\varepsilon)^n|x|^n, \forall |x|<\frac{1}{\rho+\varepsilon}$$
- Hence $$\sum_{n=0}^\infty|a_n||x|^n\leq\sum_{n=0}^\infty q^n, q=(\rho+\varepsilon)|x|<1$$