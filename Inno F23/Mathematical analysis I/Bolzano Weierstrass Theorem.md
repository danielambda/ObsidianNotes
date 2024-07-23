---
tags:
  - Math
  - MathematicalAnalysis
slide: "2.12"
---
## Statement
Each bounded [[Sequence]] has a [[Limit of a Sequence|converging]] [[Subsequence]], but not vise-versa.
## Proof
1. Let $[a_0, b_0]:=$ an interval containing all terms of $(x_n)_{n\in\mathbb N}, m:=0\;\&\;y_m:=$ the first term from $(x_n)_{n\in\mathbb N}\in[a_0,b_0];$
2. Loop
	Let $[a_{m+1},b_{m+1}]:=$ a half of the interval $[a_m,b_m]$ that $(x_n)_{n\in\mathbb N}$ hits infinitely often,
	$y_{m+1}:=$ the first after $y_m$ term from $(x_n)_{n\in\mathbb N}\in[a_{m+1},b_{m+1}];$ 
	$m:=m+1$
3. Loop invariant
	$(x_n)_{n\in\mathbb N}$ hits $[a_m,b_m]$ infinitely often
	$y_0...y_m$ is a [[Subsequence]] of a prefix of $(x_n)_{n\in\mathbb N}$
	$|a_m,b_m|=\frac{|a_0,b_0|}{2^m}$
4. Let ${y}:=\cap_{m\in\mathbb N}[a_m,b_m]$
5. Let $\varepsilon>0$ be any positive real and $m\in\mathbb N$ be the first natural number such that $|a_m,b_m|\leq\varepsilon$
6. By construction, $\forall n\in\mathbb N, n\geq m: y_n\in[a_m,b_m]\implies |y_n-y|\leq\varepsilon$
7. Therefore, $\displaystyle y=\lim_{n\to\infty}y_n, Q.E.D.\square$ 