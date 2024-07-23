---
tags:
  - Math
  - MathematicalAnalysis
  - ComplexAnalysis
---
- If $f(x)=f(x+T)$ and $T$ is the smallest [[Periodic Function|period]] of the [[Function]] $f(x)$, then the [[Fourier Series]] for this [[Function]] can be constructed by the following formula:
## Real
$$a_n=\frac2T\int_0^Tf(x)\cos\left(\frac{2\pi}Txn\right)dx,\;\;b_n=\frac2T\int_0^Tf(x)\sin\left(\frac{2\pi}Txn\right)dx$$
$$S(x)=\frac12a_0+\sum_{n=1}^\infty\left(a_n\cos\left(\frac{2\pi}Txn\right)+b_n\sin\left(\frac{2\pi}Txn\right)\right)$$
## Complex
$$c_n=\frac1T\int_0^T f(x)e^{-i\frac{2\pi}Tnx}dx$$
$$S(x)=\sum_{n=-\infty}^\infty c_n e^{i\frac{2\pi}Tnx}$$