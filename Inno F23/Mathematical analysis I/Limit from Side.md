---
tags:
  - Math
  - MathematicalAnalysis
---
## Definitions
- A point $x\in\mathbb R$ is a **right**-side [[Limit of a Function|limit of a real function]] $f: D\to\mathbb R$ when $x$ tending from right to $d\in\mathbb R$
	$\displaystyle y= \lim_{x\to d+0}f(x)\iff$$$\iff\forall\varepsilon\in\mathbb R, \varepsilon>0\;\exists\delta\in\mathbb R, \delta>0\;\forall x\in D: d<x\leq d+\delta\implies |f(x)-y|\leq\varepsilon$$
	function $f$ with restricted domain $(D\cap]d,+\infty[)$ has $y$ as a limit, as $x\to d$

A point $x\in\mathbb R$ is a **left**-side [[Limit of a Function|limit of a real function]] $f: D\to\mathbb R$ when $x$ tending from right to $d\in\mathbb R$
	$\displaystyle y= \lim_{x\to d+0}f(x)\iff$$$\iff\forall\varepsilon\in\mathbb R,\varepsilon>0\;\exists\delta\in\mathbb R, \delta>0\;\forall x\in D: d-\delta\leq x<d\implies |f(x)-y|\leq\varepsilon$$
function $f$ with restricted domain $(D\cap]-\infty,d[)$ has $y$ as a limit, as $x\to d$
## Relations with usual Limit
1. if $\displaystyle\lim_{x\to d}f(x)$ does exists, then $\displaystyle\lim_{x\to d-0}f(x)$ and $\displaystyle\lim_{x\to d+0}f(x)$ also exist and $\displaystyle\lim_{x\to d-0}f(x)=\lim_{x\to d}f(x)=\lim_{x\to d+0}f(x)$
2. if $\displaystyle\lim_{x\to d-0}f(x)$ and $\displaystyle\lim_{x\to d+0}f(x)$ exist and are equal then $\displaystyle\lim_{x\to d}f(x)$ exists and $\displaystyle\lim_{x\to d-0}f(x)=\lim_{x\to d}f(x)=\lim_{x\to d+0}f(x)$