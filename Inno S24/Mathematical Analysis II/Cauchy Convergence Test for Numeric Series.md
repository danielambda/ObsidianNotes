---
tags:
  - MathematicalAnalysis
  - Math
---
## Theorem
- The [[Numeric Series]] converges if
$$\forall\varepsilon\in\mathbb R,\varepsilon>0\;\exists N\in\mathbb N: \forall n, p\in\mathbb N, N<n<p$$

$$\left|\sum^p_{k=n}a_k\right|<\varepsilon$$
## Proof 
- From [[Cauchy Sequences Convergence test]] we get the inequality:
$$|S_p-S_n|<\varepsilon, N<n<p\implies\forall p\in\mathbb N, N>n>p:\left|\sum^p_{k=n}a_k\right|<\varepsilon. \blacksquare$$