---
tags:
  - Math
  - MathematicalAnalysis
slide: "3.69"
---
## Definition
- Let $n\in\mathbb N; a,b\in\mathbb R; f\in C^n]a,b[$
- Taylor Polynomial (of the degree $n$) for this function $f$ at point $d\in]a,b[$ is the following polynomial $$T_{n,f,d}(x)=\sum_{k=0}^n\frac{f^{(k)}(d)}{k!}(x-d)k=$$
$$=f(d)+f'(d)(x-d)+\frac{f''(d)}{2!}(x-d)^2+\frac{f'''(d)}{3!}(x-d)^3+...+\frac{f^{(n)}(d)}{n!}(x-d)^n$$
## Statement about Taylor Formula
- Let $n\in\mathbb N; a,b\in\mathbb R;f\in C^n]a,b[;d\in]a,b[;T_{n,f,d}(x)$
- Then function $(f-T_{n,f,d})$ is an infinitesimal of order $n$ at point $d$ (or of order $(x-d)^n)$ in the following sense:
$$\lim_{x\to d}\frac{f(x)-T_{n,f,d}(x)}{(x-d)^n}=0$$
## Proof about Taylor Formula
$\displaystyle\lim_{x\to d}\frac{f(x)-T_{n,f,d}(x)}{(x-d)^n}=$
$=\displaystyle\lim_{x\to d}\frac{f(x)-\left(f(d)+f'(d)(x-d)+\frac{f''(d)}{2!}(x-d)^2+...+\frac{f^{(n)}(d)}{n!}(x-d)^n\right)}{(x-d)^n}=$

[[L'Hopital's Rule]] used
$=\displaystyle\lim_{x\to d}\frac{f'(x)-\left(0+f'(d)+2\frac{f''(d)}{2!}(x-d)+3\frac{f'''(d)}{3!}(x-d)^2+...+n\frac{f^{(n)}(d)}{n!}(x-d)^{n-1}\right)}{n(x-d)^{n-1}}$
[[L'Hopital's Rule]] used
$=\displaystyle\lim_{x\to d}\frac{f''(x)-\left(0+0+2\frac{f''(d)}{2!}+2*3\frac{f'''(d)}{3!}(x-d)+...+(n-1)n\frac{f^{(n)}(d)}{n!}(x-d)^{n-2}\right)}{(n-1)n(x-d)^{n-2}}$
[[L'Hopital's Rule]] used $n-2$ more times
$\displaystyle\lim_{x\to d}\frac{f^{(n)}(x)-\left(n(n-1)(n-2)\times...\times2\times1\times\frac{f^{(n)}(d)}{n!}\right)}{n(n-1)(n-2)\times...\times2\times1\times(x-d)^0}=$
$=\displaystyle\lim_{x\to d}\frac{f^{(n)}(x)-f^{(n)}(x)}{n!}=$
$\displaystyle\lim_{x\to d}\frac{0}{n!}=0.\;Q.E.D. \blacksquare$
