---
tags:
  - Math
  - MathematicalAnalysis
  - ComplexAnalysis
---
$$\frac12(a_n-ib_n)=\frac{1}{2\pi}\int_0^{2\pi}f(x)(\cos(nx)-i\sin(nx))dx=\frac{1}{2\pi}\int_0^{2\pi}f(x)e^{-inx}dx$$
$$\Large c_n=\frac{1}{2\pi}\int_{0}^{2\pi}f(x)e^{-inx}dx$$
---
if $\displaystyle \sum_{n=-\infty}^\infty|c_n|$ [[Absolute Convergence of Numeric Series|converges absolutely]] then $$\large f(x)=\sum_{n=-\infty}^\infty c_ne^{inx}$$