---
tags:
  - Math
  - MathematicalAnalysis
slide: "3.52"
---
## Statement
Each [[Continuity of a Set of Points|continuous]] on a closed finite interval function that
- equals to 0 at both ends of the interval
- and is [[Differentiability on a Set of Points|differentiable]] in each internal point of the interval
Has [[Derivative]] equals 0 at some point of the interval
## Proof
- Let $f\in C[a,b]\;\&\;f\in C^1]a,b[\;\&\;f(a)=f(b)=0$
- By the [[Extreme Value Theorem]] $f$ attains its both extreme values $mx=\max f([a,b]), mn=\min f([a,b])$ at some points $p, q$
- $mx=mn=0\implies f(x) = 0\implies f'(x)=0, \square$
Cases $mx\not =0$ and $mn\not=0$ are similar, so we can consider only the case
- $mx\not=0:$
- $p\in]a,b[\;\&\;\forall\Delta\in U(p),\Delta>0: f(p)\geq f(p-\Delta)\;\&\;f(p)\geq f(p+\Delta)$
- $\displaystyle\forall\Delta\in U(p),\Delta>0:f(p)\geq f(p-\Delta)\implies\frac{f(p-\Delta)-f(p)}{-\Delta}\geq0$
- $\displaystyle\forall\Delta\in U(p),\Delta>0:f(p)\geq f(p+\Delta)\implies\frac{f(p+\Delta)-f(p)}{\Delta}\leq0$
- Since $f$ is [[Derivative|differentiable]] at point $p$ 
	$\begin{cases}f'(p)=\displaystyle\lim_{\Delta\to0-}\frac{f(p-\Delta)-f(p)}{-\Delta}\geq0 \\ f'(p)=\displaystyle\lim_{\Delta\to0+}\frac{f(p+\Delta)-f(p)}{\Delta}\leq0\end{cases}\implies f'(p)=0, Q.E.D. \blacksquare$
	