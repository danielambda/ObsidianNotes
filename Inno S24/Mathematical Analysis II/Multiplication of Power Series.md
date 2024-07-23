---
tags:
  - Math
  - MathematicalAnalysis
---
- Let $R$ be the [[Theorem about the Radius of Convergence|Radius of Convergence]] for both [[Power Series]]:
$$A(x)=\sum_{n=0}^\infty a_nx^n,\;B(x)=\sum_{n=0}^\infty b_nx^n$$
- Then $$A(x)\cdot B(x)=\sum_{n=0}^\infty a_nx^n\cdot\sum_{n=0}^\infty b_nx^n=\lim_{N\to\infty}\left[\lim_{M\to\infty}\left[\sum_{n=0}^N\left(\sum_{m=0}^M a_nx^nb_mx^m\right)\right]\right]=$$
$$=\lim_{N\to\infty}\left[\lim_{M\to\infty}\left[\sum_{n=0}^N\left(\sum_{m=0}^M a_nb_mx^{n+m}\right)\right]\right]=\lim_{N\to\infty}\left[\sum_{n=0}^N\left(\left(\sum_{k=0}^n a_kb_{n-k}\right)x^n\right)\right]=$$
$$\large=\sum_{n=0}^\infty\left(\sum_{k=0}^n\left(a_kb_{n-k}\right)x^n\right)$$