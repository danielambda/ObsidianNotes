---
tags:
  - MathematicalAnalysis
  - Math
---
## Statement
$\forall f: D\to\mathbb R\;\forall d\in\mathbb R_{\pm\infty}$not-lost-in-space for$f\;\forall y\in\mathbb R_{\pm\infty}: (y=\displaystyle\lim_{x\to d}f(x))\iff(y=\lim_{n\to\infty}f(d_n)$ for every $(d_n)_{n\in\mathbb N}$ that $d=\displaystyle\lim_{n\to\infty}d_n$
## Proof $(a \implies b)$
Let $(d_n)_{n\in\mathbb N}$ be a [[Sequence]] such that $\displaystyle d = \lim_{n\to\infty}d_n$ and $\varepsilon >0$ be a positive real
Since $\displaystyle y = \lim_{x\to d}f(x)\implies\exists\delta>0\;\forall x\in D:|x-d|\leq\delta\implies|f(x)-y|\leq\varepsilon$
Since $d=\displaystyle\lim_{n\to\infty}d_n\implies\exists m\in\mathbb N:\forall n_m\in\mathbb N, n > m: |d-d_n|\leq\delta$
Hence $\forall n_m>m: |f(d_n)-y|\leq\varepsilon$ 
Summary: $\forall\varepsilon>0\;\exists m\in\mathbb N:\forall n_m\in\mathbb N, n_m>m:|f(d_n)-y|\leq\varepsilon\implies$
$$y=\lim_{n\to\infty}f(d_n), Q.E.D.\blacksquare$$
## Proof $(b\implies a)$
By contradiction
Let $\displaystyle y=lim_{n\to\infty}f(d_n)$ for every sequence $(d_n)_{n\in\mathbb N}$ and $\displaystyle d = \lim_{n\to\infty} d_n$.
	But let us assume $y\not =\displaystyle\lim_{x\to d} f(x)$
Since $y\not =\displaystyle\lim_{x\to d} f(x)\implies \neg(\forall\varepsilon>0\;\exists\delta>0\;\forall x:|x-d|\leq\delta\implies|f(x)-y|\leq\varepsilon)\iff$
$\iff\exists\varepsilon >0\;\forall\delta>0\;\exists x: |x-d|\leq\delta\;\&\;|f(x)-y|>\varepsilon$
Let $d_n$ be a point in support of $f$ such that $\displaystyle|d_n-d|\leq\frac 1{(n+1)}\;\&\;|f(d_n)-y|>\varepsilon\implies d=\lim_{n\to\infty}f(d_n)\;\&\;y\not=\lim_{n\to \infty}f(d_n).$
Because of contradiction with (b), assumption $y\not =\displaystyle\lim_{x\to d} f(x)$ is wrong. $Q.E.D.\blacksquare$ 