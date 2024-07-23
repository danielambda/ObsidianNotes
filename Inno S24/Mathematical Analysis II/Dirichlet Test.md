---
tags:
  - Math
  - MathematicalAnalysis
---
## Test
- Let $\set{a_n}^\infty_{n=0}$ be a positive decreasing [[Sequence]] and $\displaystyle\lim_{n\to\infty} a_n=0$ and let $\displaystyle B_n=\sum_{k=0}^n b_k$ be bounded [[Sequence]]. Then the [[Numeric Series]] $$S=\sum_{n=0}^{\infty}a_nb_n\in\mathbb R$$
## Proof 
- Let's define $\displaystyle B_n=\sum^N_{k=0} b_k$ and let $B$ be the supremum of $B_N$ and $b_n=B_n-B{n-1}$: $$S_N=a_0B_0+a_1(B_1-B_0)+a_2(B_2-B_1)+...+a_N(B_N-B_{N-1})=$$ $$=B_0(a_0-a_1)+B_1(a_1-a_2)+...B_{N-1}(a_{N-1}-a_N)+a_NB_N=$$ $$=a_NB_N+\sum_{n=0}^{N-1}B_n(a_n-a_{n+1})=a_NB_N-\sum_{n=0}^{N-1}B_n(a_{n-1}-a_{n})$$
- Therefore, Adel's summation formula: $$\sum_{n=1}^Na_n(B_n-B_{n-1})=a_NB_N-a_0b_0-\sum_{n=0}^{N-1}B_n(a_{n+1}-a_n)$$
$$\left|\sum_{n=k+1}^{k+m}a_nb_n\right|\leq\left|a_{k+m}\tilde B_k^{k+m}-a_k\tilde B_k^k-\sum_{n=k}^{k+m-1}\tilde B_k^n(a_{n+1}-a_n)\right|$$
where $\displaystyle \tilde B_k^l=\sum^l_{n=k} b_n$
я устал писать дальше и уже не понимаю... Btw, lecture 2 slide 14