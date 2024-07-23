---
tags:
  - Math
  - MathematicalAnalysis
slide: "3.42"
a.k.a.: Chain Rule
---
## Statement
Let $f: D\to E\subseteq\mathbb R, g: E\to\mathbb R$ be any real functions and $d\in D$ be a point. If $f$ is [[Derivative|differentiable]] at $d$ and $g$ is [[Derivative|differentiable]] at $f(d)$, then the [[Function Composition|compound function]] $h=g\circ f=\lambda x\in D. g(f(x))$ is [[Continuity|continuous]] at point $d$ and $$h'(d)=g'(f(d))f'(d)$$
## Proof
$\displaystyle\lim_{\Delta\to0}\frac{(g\circ f)(d+\Delta)-(g\circ f)(d)}{\Delta}=\lim_{\Delta\to0}\frac{g(f(d+\Delta))-g(f(d))}{\Delta}=$
$\displaystyle=\lim_{\Delta\to0}\left(\frac{g(f(d+\Delta))-g(f(d))}{f(d+\Delta)-f(d)}\times\frac{f(d+\Delta)-f(d)}{\Delta}\right)=$
$\displaystyle(?)=\left(\lim_{\Delta\to0}\frac{g(f(d)+\Delta)-g(f(d))}{\Delta}\right)\times\left(\lim_{\Delta\to0}\frac{f(d+\Delta)-f(d)}{\Delta}\right)=$$$=g'(f(d))f'(d), Q.E.D.\blacksquare$$
## (?)
### Statement
$$\lim_{\Delta\to0}g(f(d+\Delta))=\lim_{\Delta\to0}g(f(d)+\Delta)$$
### Proof
Since $f$ is [[Derivative|differentiable]] at $d$ and $g$  is [[Derivative|differentiable]] at $f(d)$, they both are [[Continuity|continuous]] at points $d, f(d)$, respectively:
	$\displaystyle\lim_{x\to d}f(x)=f(d)\iff\lim_{\Delta\to 0}f(d+\Delta)=f(d)$
	$\displaystyle\lim_{x\to f(d)}g(x)=g(f(d))\iff\lim_{\Delta\to0}g(f(d)+\Delta)=g(f(d))$
$\implies \displaystyle\lim_{\Delta\to 0}g(f(d+\Delta))=g(f(d))=\lim_{\Delta\to0}g(f(d)+\Delta),Q.E.D.\blacksquare$ 