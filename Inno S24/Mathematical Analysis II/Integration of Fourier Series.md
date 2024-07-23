---
tags:
  - Math
  - MathematicalAnalysis
---
## Integration
$$\int_{x_0}^x S(t)dt=\int_{x_0}^x\left(\frac12a_0+\sum_{n=1}^\infty a_n\cos(nt)+b_n\sin(nt)\right)dt=$$$$=\int_{x_0}^x\left(\frac12a_0+\sum_{n=1}^N a_n\cos(nt)+b_n\sin(nt)\right)dt+\int_{x_0}^x\left(\sum_{n=N+1}^\infty a_n\cos(nt)+b_n\sin(nt)\right)dt$$$$\forall\varepsilon\in\mathbb R,\varepsilon>0\;\exists N\in\mathbb N:\left|\sum_{n=N}^\infty a_n\cos(nx)+b_n\sin(nx)\right|<\varepsilon\implies$$
$$\int_{x_0}^x S(t)dt=\frac12(x-x_0)a_0+\sum_{n=1}^N\int_{x_0}^x(a_n\cos(nt)+b_n\sin(nt))dt+O(\varepsilon)$$
$$\int_{x_0}^x S(t)dt=\frac12(x-x_0)a_0+\sum_{n=1}^\infty\left(\frac{a_n}{n}(\sin(nx)-\sin(nx_0))-\frac{b_n}{n}(\cos(nx)-\cos(nx_0))\right)=$$$$=\frac12a_n(x-x_0)+\sum_{n=1}^\infty\left(\frac{a_n}{n}\sin(nx)-\frac{b_n}{n}\cos(nx)\right)-\sum_{n=1}^\infty\left(\frac{a_n}n\sin(nx_0)+\frac{b_n}{n}\cos(nx_0)\right)$$
- If [[Fourier Series]] is absolutely convergent uniformly over the period, then the [[Indefinite Integral|integral]] of the series is equal to the [[Fourier Series]] integrated term by term. 