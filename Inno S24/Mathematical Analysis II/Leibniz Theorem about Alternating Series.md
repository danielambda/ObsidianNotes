---
tags:
  - Math
  - MathematicalAnalysis
---
## Theorem
- Let $u_n>u_{n+1}$, if $\displaystyle \lim_{n\to\infty} u_n=0$ then $$S=\sum^\infty_{n=0}(-1)^n u_n\in\mathbb R$$
## Proof
$$S=(u_0-u_1)+(u_2-u_3)+...$$
- Define $\sigma_n=u_{2n}-u_{2n+1}>0$, then the partial sum $\displaystyle S_n=\sum_{n=0}^N\sigma^n$ increases
$$S=u_0-(u_1-u_2)-(u_3-u_4)-(u_5-u_6)-u_7+...$$
- Define $\tau_n=u_{2n-1}-u_{2n}>0$. The partial sums $$S_n=u_0-\tau_1-\tau_2-...$$
- Then $S_n$ is bounded. Therefore, the [[Sequence]] $S_n$ has a [[Limit of a Sequence|limit]]. The alternating [[Numeric Series]] converges
