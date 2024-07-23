---
tags:
  - Math
  - MathematicalAnalysis
---
## Definition
- Let assume $f(x)$ be a represented as a [[Fourier Series]]: 
$$f(x)=\frac12a_0+\sum_{n=1}^\infty a_n\cos(nx)+b_n\sin(nx)$$
- Then the coefficients of the [[Fourier Series]] are:
	- $\displaystyle a_0=\frac1\pi\int_0^{2\pi}f(x)dx$
	- $\displaystyle a_n=\frac1\pi\int_0^{2\pi}f(x)\cos(nx)dx,n\in\mathbb N$
	- $\displaystyle b_n=\frac1\pi\int_0^{2\pi}f(x)\sin(nx)dx,n\in\mathbb N$
## Reasoning
$$\int_0^{2\pi}\cos(ms)\cos(nx)dx=\int_{0}^{2\pi}\left(\frac12\cos\left(\frac{x(m-n)}{2}\right)+\frac12\cos\left(\frac{x(m+n)}{2}\right)\right)dx=$$$$=\frac12\left(\int_0^{2\pi}\cos\frac{x(m-n)}2dx+\int_0^{2\pi}\cos\frac{x(m+n)}2dx\right)=\begin{cases}\pi,n=m\\ 0,n\not=m\end{cases}$$

---
$$\int_0^{2\pi}\sin(ms)\sin(nx)dx=\int_{0}^{2\pi}\left(\frac12\cos\left(\frac{x(m-n)}{2}\right)-\frac12\cos\left(\frac{x(m+n)}{2}\right)\right)dx=$$$$=\frac12\left(\int_0^{2\pi}\cos\frac{x(m-n)}2dx-\int_0^{2\pi}\cos\frac{x(m+n)}2dx\right)=\begin{cases}\pi,n=m\\ 0,n\not=m\end{cases}$$

---
$$\int_0^{2\pi}\cos(ms)\sin(nx)dx=\int_{0}^{2\pi}\left(\frac12\sin\left(\frac{x(m-n)}{2}\right)-\frac12\sin\left(\frac{x(m+n)}{2}\right)\right)dx=0$$