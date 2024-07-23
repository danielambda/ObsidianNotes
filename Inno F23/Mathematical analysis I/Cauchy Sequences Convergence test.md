---
tags:
  - Math
  - MathematicalAnalysis
---
## Definition
- A real sequence $(x_n)_{n\in\mathbb N}$ meets Cauchy sequence convergence test if: $$\forall\varepsilon\in\mathbb R, \varepsilon>0\;\exists m\in\mathbb N\;\forall n_1, n_2\geq m: |x_{n_1}-x_{n_2}| \leq \varepsilon$$
- Meeting Cauchy sequences convergence test $\iff$ converging $\iff$ having a *real* [[Limit of a Sequence|limit]]
## Proof for if-derection
- Let $(x_n)_{n\in\mathbb N}$ converge $\iff$ $\exists x: x = \displaystyle\lim_{n\to\infty} x_n$
- Let $\varepsilon > 0$ be any positive real
	- $x = \displaystyle\lim_{n\to\infty} \implies \exists m\in\mathbb N: \forall n\in\mathbb N: |x_n - x| \leq \frac{\varepsilon}{2}$
	- hence, $\forall n_1, n_2 > m: |x_{n_1} - x_{n_2}| = |(x_{n_1} - x) + (x - x_{n_2})| \leq$
								$\leq |x_{n_1} - x| + |x_{n_2} - x| \leq \varepsilon$
	- $\implies$ sequence meets the test definition