---
tags:
  - Math
  - MathematicalAnalysis
russian: Лемма о двух милиционерах
slide: "2.21"
---
## Statement
For any real [[Sequence|sequences]] $(x_n)_{n\in\mathbb N},(y_n)_{n\in\mathbb N},(z_n)_{n\in\mathbb N}$
- If $(x_n)_{n\in\mathbb N}, (z_n)_{n\in\mathbb N}$ have joint [[Limit of a Sequence|limit]]
- and $\exists m\in\mathbb N\;\forall n\in\mathbb N,n\geq m: x_n\leq y_n\leq z_n$
Then $(y_n)_{n\in\mathbb N}$ converges to the same limit as both $(x_n)_{n\in\mathbb N}$ and $(z_n)_{n\in\mathbb N}$
---
$\forall (x_n)_{n\in\mathbb N}, (y_n)_{n\in\mathbb N}, (z_n)_{n\in\mathbb N}\in\mathbb R:$$(\displaystyle\lim_{n\to\infty}x_n=\lim_{n\to\infty}z_n\;\&\;\exists m\in\mathbb N\;\forall n\in\mathbb N, n\geq m:x_n\leq y_n\leq z_n)\implies$
$$\lim_{n\to\infty} x_n=\lim_{n\to\infty} y_n=\lim_{n\to\infty} z_n$$
## Proof
$\displaystyle\lim_{n\to\infty}x_n$ exists $\;\&\;\displaystyle\lim_{n\to\infty}z_n$ exists $\;\&\;\displaystyle\lim_{n\to\infty}x_n = \lim_{n\to\infty}z_n=a\iff$ $\iff \forall \varepsilon\in\mathbb R, \varepsilon >0\;\exists m_x,m_z\in\mathbb N\;\forall n_x,n_z\in\mathbb N, n_x\geq m_x\;\&\;n_z\geq m_z: |x_{n_x}-a| \leq \varepsilon\;\&\;|z_{n_z-a}|\leq\varepsilon$ Let $N=\max\{m,m_x,m_z\}$ then
	$\forall n\in\mathbb N, n\geq N: |x_n-a|\leq\varepsilon\;\&\;|z_n-a|\leq\varepsilon\;\&\;x_n\leq y_n\leq z_n\implies|y_n-a|\leq\varepsilon\implies$
		$\displaystyle\lim_{n\to\infty}y_n=a=\lim_{n\to\infty}x_n = \lim_{n\to\infty}z_n, Q.E.D. \blacksquare$
	