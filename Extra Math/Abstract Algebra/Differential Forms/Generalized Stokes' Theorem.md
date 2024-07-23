---
tags:
  - Math
  - MathematicalAnalysis
  - DifferetialForms
---
## Special Case
- Suppose $\omega=f\,dx_2\wedge...\wedge dx_n$ is an [[Differential m-Form|differential (n-1)-form]] on $\mathbb R^n$ and $R=[0,1]^n$. 
- Then $$\LARGE\int_{\partial R}\omega=\int_R d\omega$$
## Proof of the Special Case
- Fix $N\in\mathbb N$, for $I=(i_1,...,i_n)$
- Assume $e_i$ is the orthonormal [[Basis]] of $\mathbb R^n$
$$x_I=\left(\frac{i_1}{N},...,\frac{i_n}{N}\right)$$
$$d\omega=\frac{\partial f}{\partial x_1}dx_1\wedge...\wedge dx_n$$
$$\Large\int_R d\omega=\lim_{N\to\infty}\left(\sum_{j=1}^n\sum_{i_j=0}^N d\omega_{x_I^*}\left(\frac{e_1}{N},...,\frac{e_N}{N}\right)\right)$$
where $\displaystyle x_I^*\in\left[\frac{i_{1}}{N},\frac{i_{1+1}}{N}\right]\times\left[\frac{i_{2}}{N},\frac{i_{2+1}}{N}\right]\times...$
$$\Large \lim_{N\to\infty}\left[\sum_{j=1}^n\sum_{i_j=0}^N \frac{\partial f}{\partial x_1}(x_I^*)dx_1\wedge...\wedge dx_n\left(\frac{e_1}{N},...,\frac{e_N}{N}\right)\right]$$
Using [[Mean Value Theorem]]
$$\large\lim_{N\to\infty}\left[\sum_{j=1}^n\sum_{i_j=0}^N \frac{f\left(\frac{i_1+1}{N},\frac{i_2}N,...,\frac{i_n}N\right)-f(x_I)}{1/N}\frac{dx_{\color{red}2}\wedge...\wedge dx_n}{N}\left(\frac{e_{\color{red}2}}{N},...,\frac{e_N}{N}\right)\right]$$
$$\large\lim_{N\to\infty}\left[\sum_{j=1}^n\sum_{i_j=0}^N \left(f\left(\frac{i_1+1}{N},\frac{i_2}N,...,\frac{i_n}N\right)-f(x_I)\right)dx_{\color{red}2}\wedge...\wedge dx_n\left(\frac{e_{\color{red}2}}{N},...,\frac{e_N}{N}\right)\right]$$
Somehow $f(x_I)$ telescopes and results in this:
$$\large\lim_{N\to\infty}\left[\sum_{j=2}^n\sum_{i_j=0}^N \left(f\left(1,\frac{i_2}{N},...,\frac{i_n}{N}\right)-f\left(0,\frac{i_2}{N},...,\frac{i_n}{N}\right)\right)dx_{\color{red}2}\wedge...\wedge dx_n\left(\frac{e_{\color{red}2}}{N},...,\frac{e_N}{N}\right)\right]$$
$$\Large\int_{\set{1}\times[0,1]^{n-1}}\omega-\int_{\set0\times[0,1]^{n-1}}\omega=\int_{\set{0^-,1^+}\times[0,1]^{n-1}}\omega=\int_{\partial R}\omega\;\blacksquare$$
