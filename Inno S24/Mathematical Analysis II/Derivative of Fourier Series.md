---
tags:
  - Math
  - MathematicalAnalysis
---
## Differentiating
- If the coefficients of the [[Fourier Series]] $a_n,b_n$ are such that both series $$\sum_{n=1}^\infty n|a_n|,\sum_{n=1}^\infty n|b_n|$$
are convergent, then the [[Derivative]] of the [[Fourier Series]] is equal to differentiated term by term series
## Proof
$$S(x)=\int_{x_0}^x\sum_{n=1}^\infty (-na_n\sin(nt)+nb_n\cos(nt))dt=\sum_{n=1}^\infty (a_n\cos(nx)+b_n\sin(nx))\implies$$
$$\frac{d}{dx}S(x)=\sum_{n=1}^\infty (-na_n\sin(nx)+nb_n\cos(nx))$$