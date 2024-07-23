---
tags:
  - Math
  - MathematicalAnalysis
slide: "3.63"
a.k.a.: Bernoulli's Rule
---
## Statement
For $d\in\mathbb R_{\pm\infty},\displaystyle \lim_{x\to d}\frac{f(x)}{g(x)}$ 
$\left[\displaystyle\begin{gathered}\lim_{x\to d}f(x)=\lim_{x\to d}g(x)=0\\ \lim_{x\to d}f(x),\lim_{x\to d}g(x) \in \{+\infty, -\infty\}\end{gathered}\right.$
$f(x), g(x)$ are [[Derivative|differentiable]] at point $d\implies$ $$\lim_{x\to d}\frac{f(x)}{g(x)}=\lim_{x\to d}\frac{f'(x)}{g'(x)}$$
## Proof (partial)
$\displaystyle\lim_{x\to d}\frac{f(x)}{g(x)}=\lim_{x\to d}\frac{(f(x)-0)/(x-d)}{(g(x)-0)/(x-d)}=$
$\displaystyle=\lim_{x\to d}\left(\frac{f(x)-f(d)}{x-d}/\frac{g(x)-g(d)}{x-d}\right)=\frac{f'(d)}{g'(d)}=\lim_{x\to d}{f'(x)}{g'(x)}$ 