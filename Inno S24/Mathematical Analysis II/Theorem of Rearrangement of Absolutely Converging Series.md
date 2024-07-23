---
tags:
  - Math
  - MathematicalAnalysis
---
## Theorem
- Consider $\displaystyle S=\sum^{\infty}_{n=0} a_n$ is [[Absolute Convergence of Numeric Series|absolutely converging]]. Consider the [[Numeric Series]] with the same terms but permutated: $$\tilde S=\sum^\infty_{n=0} \tilde a_n$$
$$S=\tilde S$$
## Proof 
- Denote  $$\sigma = \sum^{\infty}_{n=0}|a_n|, \tilde\sigma = \sum^{\infty}_{n=0}|\tilde a_n|$$
- $\forall m\;\exists n\geq m,\set{\tilde a_k}_{k=0}^m\subset\set{a_k}_{k=0}^n$, then $\tilde\sigma_m\leq \sigma_n\implies \set{\tilde\sigma_m}^\infty_{m=0}$ is increasing bounded [[Sequence]], hence it has a [[Limit of a Sequence|limit]] $\tilde\sigma\leq\sigma$ 
- For the same reasons $\sigma\leq\tilde\sigma$
- Therefore $$\sigma=\tilde\sigma\implies\sum^{\infty}_{n=0}|a_n|=  \sum^{\infty}_{n=0}|\tilde a_n|$$
- Let's consider a [[Sequence]] of [[Partial Sum|partial]] [[Numeric Series]] $S_n$. Due to the absolute convergence we get: $$\forall\varepsilon\in\mathbb R, \varepsilon>0\;\exists N\in\mathbb N\;\forall n\in\mathbb N, n>N: |S_n-S_n+1|\leq \varepsilon$$
- Due to the [[Cauchy Convergence Test for Numeric Series]]: $$\exists S=\lim_{n\to\infty} S_n$$
- For the same reasons $\displaystyle \exists \tilde S=\lim_{n\to\infty}\tilde S_n$
$$\forall n\in\mathbb N\;\exists N\in\mathbb N: \set{\tilde a_k}_{k=0}^n\subset\set{a_n}_{m=0}^N$$
- Let's consider the difference, where $m\geq N$:
$$|S-\tilde S_n|=|S-\tilde S_n+S_m-S_m|\leq|S-S_m|+|S_m-\tilde S_n|\to 0, n\to\infty\implies$$
$$\implies \tilde S=S. \blacksquare$$