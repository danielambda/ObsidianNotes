---
tags:
  - Math
  - MathematicalAnalysis
slide: "3.44"
---
## Statement
Let $f: D\to E$ be a real function differentiable at some point $d\in D$ such that there exists an inverse function $f^-:E\to D$
	$(f^-\circ f=\lambda x\in D. x)$, $f'(d)\not=0\implies f^-$ is [[Derivative|differentiable]] at point $f(d)$ and $(f^-)'(f(d))=1/f'(d)$ 
## Proof
$f(f^-(x))=x\iff(f(f^-(x)))'=x'\iff(f^-(x))'\times f'(f^-(x))=1\iff$
$$\iff (f^-(x))'=\frac{1}{f'(f^-(x))}$$