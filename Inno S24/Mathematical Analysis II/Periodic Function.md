---
tags:
  - Math
  - MathematicalAnalysis
---
## Definition
- A [[Piecewise Continuous Function]] $f(x)$ such that:
	- $\forall x\in\mathbb R: f(x+T)=f(x)$ for certain constant $T>0$ is called *periodic function*
- The value $T$ is called *period*
--- 
- Let $T$ be a period of $f(x)$ then quantities $\tilde T=nT, n\in\mathbb Z$ are periods of $f(x)$
---
- The reciprocal quantity is called *frequency*: $\displaystyle\omega=\frac1T$
## Theorem
- Let $T$ be the smallest of the periods of a [[Piecewise Continuous Function]] $f(x)$
- Then all periods of the [[Function]] are $nT, n\in\mathbb Z$ or the function is constant
## Proof
- Suppose the [[Function]] $f$ has two different periods. Define the smallest one as $T_1$ and another one as $T_2\not=nT_1, n\in\mathbb Z$
- $f(t-T_1)=f(t), f(t-T_1+T+2)=f(t+(T_2-T_1))=f(t)\implies$
	- $\implies T_2-T_1$ is a period $\implies$
		- $\implies \exists N\in\mathbb N^+:T_1>T_2-NT_1>0\;\&\;T=T_2-NT_1\;\&\; f(t+T)=f(t)$
			- contradiction
## Properties
- Let 2 [[Function]]s $f(x)$ and $h(x)$ be periodic. Their periods are $T_f, T_h$. The sum of the functions: $g(x)=f(x)+h(x)$ is a periodic function of period $T$ if $\exists n,m\in\mathbb N: T_1n=T_2m$ and in such a case $T=T_1n=T_2m$
### Examples
- $g(x)=\sin(3x)+\cos(5t),\;T_{\sin}=\frac{2\pi}{3},T_{\cos}=\frac{2\pi}{5}$
	- $3T_{\sin}=5T_{\cos}=2\pi\implies T=2\pi$
---
- $g(x)=\sin(3x)+\cos(\sqrt2x),\;T_{\sin}=\frac{2\pi}{3},T_{\cos}=\frac{2\pi}{\sqrt2}$
	- $\displaystyle\frac{T_{\sin}}{T_{\cos}}\not\in\mathbb Q\implies g(x)$ is not periodic