---
tags:
  - Math
  - MathematicalAnalysis
  - ComplexAnalysis
---
## Definition
- Using the [[Euler's Formula]] from [[Fourier Series]] one can write:
$$S(x)=\frac12a_0+\sum_{n=1}^\infty (a_n\cos(nx)+b_n\sin(nx))=$$
$$=\frac12a_0\sum_{n=1}^\infty\left(a_n\frac{e^{inx}+e^{-inx}}{2}+b_n\frac{e^{inx}-e^{-inx}}{2i}\right)=$$$$\frac12a_0+\sum_{n=1}^\infty\left(\frac{a_n-ib_n}{2}e^{inx}+\frac{a_n+ib_n}{2}e^{-inx}\right)=$$
$$=\frac12a_0+\sum_{n=1}^\infty\left(\frac{a_n-ib_n}{2}e^{inx}\right)+\sum_{n=1}^\infty\left(\frac{a_n+ib_n}{2}e^{-inx}\right)=$$

$$=\frac12a_0+\sum_{n=1}^\infty\left(\frac{a_n-ib_n}{2}e^{inx}\right)+\sum_{n=-\infty}^{-1}\left(\frac{a_{-n}+ib_{-n}}{2}e^{inx}\right)=$$
- Define $\displaystyle c_0=a_0, c_n=\frac{a_n-ib_n}{2}, c_{-n}=\frac{a_{-n}+ib_{-n}}{2},n\in\mathbb N$
$$\Large S(x)=\sum_{n=-\infty}^\infty c_ne^{inx}$$
