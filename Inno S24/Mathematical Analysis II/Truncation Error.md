---
tags:
  - Math
  - MathematicalAnalysis
---
## Definition
- Consider a convergent [[Numeric Series]] $$S=\sum_{n=0}^\infty a_n$$
- Define the reminder of [[Partial Sum]] $S_N$:$$R_N=S-S_N$$
- The *truncation error* is the sum of the reminder terms
## Theorem about truncation error of an alternating series
- An absolute value of the reminder of a [[Partial Sum]] of an alternating [[Numeric Series]] $$S=\sum_{n=0}^\infty(-1)^n u_n, 0<u_{n+1}<u_n, \lim_{n\to\infty} u_n=0$$
can be estimated as an absolute value of first discarded term: $$|R_N|<|u_{n+1}|$$
## Proof
$$R_N=\sum_{n=N+1}^{\infty}(-1)^n u_n=(-1)^{N+1}(u_{N+1}-(u_{N+2}-u_{N+3})-(u_{N+4}-u_{N+5})-...)$$
- Consider $$(-1)^{N+1}\sum_{N+1}^\infty(-1)^nu_n=(u_{N+1}-u_{N+2})+(u_{N+3}-u_{N+4})+...$$
is the sum of positive terms, hence, the partial sums increase
- Let's rewrite the series in a following form: $$(-1)^{N+1}\sum_{N+1}^\infty(-1)^n u_n=u_{N+1}-(u_{N+2}-u_{N+3})-(u_{N+4}-u_{N+5})-...$$
- Due to the decreasing property of the [[Sequence]] $\set{u_n}$ and the [[Partial Sum]]s do not exceed $u_{N+1}$. Hence, one can see the increasing bounded sequence of the partial sums then: $$|R_N|<|u_{N+1}|$$
