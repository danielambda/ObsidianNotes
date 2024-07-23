---
tags:
  - Math
  - MathematicalAnalysis
---
## Theorem
$$\lim_{n\to\infty}\left|\frac{a_{n+1}}{a_n}\right|=q<1$$
implies [[Absolute Convergence of Numeric Series]] $a_n$ ($a$)
## Proof
$$\forall\varepsilon\in\mathbb R, \varepsilon>0\;\exists N\in\mathbb N\;\forall m\in\mathbb N,m>N\;\exists Q\in\mathbb R, q<Q<1:$$
$$|a_{m+k}|<|a_{m+k-1}|Q<...<|a_m|Q^k$$
$$\sum^\infty_{k=m}|a_m|Q^k=\frac{|a_m|}{1-Q}$$
$$\sum^\infty_{n=1}|a_n|<\sum^{N}_{n=1}|a_n|+\frac{|a_{N+1}|}{1-Q}\in\mathbb R\implies$$
$$\sum^\infty_{n=1}|a_n|\in\mathbb R. \blacksquare$$
## Example
$$S=\sum^\infty_{n=0}\frac{n^2}{3^n}$$
$$\lim_{n\to\infty}\frac{(n+1)^23^n}{3^{n+1}n^2}=\frac13\lim_{n\to\infty}\frac{(n+1)^2}{n^2}=\frac13\implies S\in\mathbb R$$