---
tags:
  - Math
  - MathematicalAnalysis
---
## Theorem
$$\lim_{n\to\infty}\sqrt[n]{|a_n|}=q<1\implies s=\sum^\infty_{n=0}|a_n|\in\mathbb R$$
## Proof
$$\lim_{n\to\infty}\sqrt[n]{|a_n|}=q>1$$
$$\forall\varepsilon\in\mathbb R, \varepsilon>0\;\exists N\in\mathbb N\;\forall m\in\mathbb N, m>N\;\exists Q\in\mathbb R, q<Q<1:$$
$$\sqrt[m]{|a_m|}<Q, |a_m|<Q^m$$
$$s=\sum^\infty_{n=0}|a_n|\leq\sum^N_{n=0}+\sum^\infty_{n=N+1}Q^n\in\mathbb R\implies s\in\mathbb R.\blacksquare$$
## Example
$$S=\sum^\infty_{n=0}\frac {n}{3^n}$$
$$\lim_{n\to\infty}\sqrt[n]{\frac{n}{3^n}}=\frac13\lim_{n\to\infty}\sqrt[n]{n}$$
$$\lim_{n\to\infty}\log(\sqrt[n]{n})=\lim_{n\to\infty}\frac{\log (n)}{n}=0\implies\lim_{n\to\infty}\sqrt[n]{n}=1$$
$$\frac13\lim_{n\to\infty}\sqrt[n]{n}=\frac13<1\implies S\in\mathbb R$$