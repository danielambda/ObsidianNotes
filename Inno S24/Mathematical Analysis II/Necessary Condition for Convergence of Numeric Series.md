---
tags:
  - Math
  - MathematicalAnalysis
---
## Theorem
$$\displaystyle S=\sum^{\infty}_{n=0}a_n\in\mathbb R\implies \displaystyle \lim_{n\to\infty} a_n=0$$
## Proof
- Assume $\exists\displaystyle \lim_{n\to\infty}S_n, S_{n+1}=S_n+a_n$
	- Due to the uniqueness of the [[Limit of a Sequence|limit]]: 
	$$\forall\varepsilon\in\mathbb R, \varepsilon >0\;\exists N\in\mathbb N\;\forall n\in\mathbb N, n>N: |S_n-S_{n-1}|<\varepsilon \implies|a_n|<\varepsilon. \blacksquare$$