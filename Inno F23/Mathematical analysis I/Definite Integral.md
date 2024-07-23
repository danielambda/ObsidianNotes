---
tags:
  - Math
  - MathematicalAnalysis
a.k.a.: Riemann Integral
slide: "3.38"
---
## Definition
- Let $P$ be a set of [[Tagged Partition of a Closed Interval|all tagged partitions of a closed real interval]] $[a,b]$, $f:[a,b]\to\mathbb R$ be a total real [[Function]]; The [[Function]] is integrable if the exists a real number $S\in\mathbb R$ such that:
$$\forall\varepsilon\in\mathbb R,\varepsilon>0\;\exists\delta\in\mathbb R,\delta>0\;\forall\{(x_k)_{k\in[0..n]},(t_k)_{k\in[0..n[}\}\in P,mesh<\delta:$$$$|S(f,(x_k)_{k\in[0..n]},(t_k)_{k\in[0..n[})-S|\leq\varepsilon$$ [[Riemann Sum]]
## Notation
If such $S\in\mathbb R$ exists, then it is denoted by 
$$\int^b_af(x)dx$$
and is called the definite integral of the [[Function]] $f$ on the interval $[a,b]$
- if $b<a$ then let $\displaystyle\int^b_af(x)dx =-\int^a_bf(x)dx$
## Properties
- #### Additivity
	- For any real interval $[a,b]$ and any $c\in[a,b]$, any total real [[Function]] $f:[a,b]\to\mathbb R$:$$\int^b_af(x)dx=\int^c_af(x)dx+\int^b_cf(x)dx$$
	- in strong sense (i.e. both sides of the equality do exists simultaneously)
- #### Linearity
	- For any real interval $[a,b]$, any total real [[Function|Functions]] $f,g:[a,b]\to\mathbb R$, for ant real numbers $\alpha, \beta\in\mathbb R:$ $$\int^b_a(\alpha f(x)+\beta g(x))dx=\alpha\int^b_af(x)dx+\beta\int^b_ag(x)dx$$
	- in a weak sense (i.e. the left-side exists if both right-side integrals exist)