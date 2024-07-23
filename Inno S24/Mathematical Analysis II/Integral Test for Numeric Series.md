---
tags:
  - Math
  - MathematicalAnalysis
---
## Theorem
- Let $f(x)$ be positive [[Continuity|continuous]] [[Monotonicity in CS|decreasing]] [[Function]]
	- Then
	$$\int^\infty_1f(x)dx\in\mathbb R\iff\sum_{n=1}^\infty f(n)\in\mathbb R$$
## Proof
$$f(n+1)\leq\int^{n+1}_nf(x)dx\leq f(n)$$
$$\sum^N_{n=1}\int_n^{n+1}f(x)dx=\int^{N+1}_1f(x)dx$$
$$\sum^N_{n=1}f(n+1)\leq\int^{N+1}_1f(x)dx\leq\sum^N_{n=1}f(n)$$
$$S_{N+2}-f(1)\leq\int_1^{N+1}f(x)dx\leq S_{N+1}$$
If the [[Definite Integral|integral]] diverges, then $\{S_{N+1}\}$ diverges. If the integral converges then $\{S_{N+2}\}$ converges and vice versa. $\blacksquare$