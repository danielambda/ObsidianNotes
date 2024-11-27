---
tags:
  - Math
  - MathematicalAnalysis
aliases: [Continuous, continuous]
---
## Definition
- A function $f: D\to\mathbb R$ is said to be continuous at a real point $d$, if $f$ has a a definite value at this point and $\displaystyle \lim_{x\to d}f(x)=f(d)$
## Equivalents
1. The left $\displaystyle\lim_{x\to d-0}f(x)$ and the right $\displaystyle\lim_{x\to d+0}f(x)$ limits exist and are equal to $f(d)$
2. $\forall (d_n)_{n\in\mathbb N}$ that $d=\displaystyle\lim_{n\to\infty}d_n: f(d) = \lim_{n\to\infty}f(d_n)$
3. $\forall\varepsilon\in\mathbb R, \varepsilon>0\;\exists\delta\in\mathbb R, \delta>0\;\forall x\in D: |x-d|\leq\delta\implies|f(x)-f(d)|\leq\varepsilon$
4. $\forall$ neighborhood 𝑉 of $f(d)\;\exists$  a neighborhood $U$ of $d: f(U)\subseteq V$
## Proofs for Equivalents
0. Let us assume that a function $f: D\to\mathbb R$ has a definite value $f(d), d\in\mathbb R$. Continuity of $f$ at point $d\in\mathbb R$ means $\displaystyle\lim_{x\to d}f(x)=f(d)$
1. [[Limit from Side]]
2. [[Limits of a Sequence in a Function]]
3. [[Limit of a Function]]
## Properties
### 1. Statement
- Let $f,g: D\to\mathbb R$ be continuous at some point $d\in D$
	1. Functions
		1. $\lambda x\in D. (f(x)+g(x))$
		2. $\lambda x\in D.(f(x)-g(x))$
		3. $\lambda x\in D.(f(x)\times g(x))$
		are continuous at point d.
	2. If $g(d)\not=0\implies\lambda x\in D.\displaystyle\frac{f(x)}{g(x)}$ is continuous at point $d$
### 1. Proof
- Equivalent form 2 + [[Arithmetic operations with Limits]]
### [[Continuity of Composition]]
