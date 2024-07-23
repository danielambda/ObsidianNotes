---
tags:
  - Math
  - MathematicalAnalysis
slide: "3.31"
---
## Statement 
function $f: D\to\mathbb R$ is [[Derivative|differentiable]] at point $d\in D\implies$ function $f$ is [[Continuity|continuous]] at point $d$ 
## Proof
[[Continuity]] at point $d$:
$\displaystyle\lim_{x\to d}f(x)=f(d)\iff\lim_{x\to d}(f(x)-f(d))=0$
[[Derivative|Differentiability]] at point $d$:
$\displaystyle f'(x)=\lim_{\Delta\to 0}\frac{f(x+\Delta)-f(x)}{\Delta}=\lim_{x\to d}\frac{f(d)-f(x)}{x-d}$
$\displaystyle\lim_{x\to d}(f(x)-f(d))=0\impliedby\lim_{x\to d}\frac{f(x)-f(d)}{x-d}(x-d)=f'(x)\times 0=0$
$Q.E.D.\blacksquare$
## Another Proof 
Let $f:D\to\mathbb R$ be [[Derivative|differentiable]] at point $d\in D$
- $\displaystyle f'(d)=\lim_{\Delta\to0}\frac{f(d+\Delta)-f(d)}{\Delta}\iff$$$\iff\frac{f(d+\Delta)-f(d)}{\Delta}=f'(d)+o(1), as\;\Delta\to 0$$ 
- Hence, $\displaystyle\forall\Delta\in U=\;]-r;+r[\;, \Delta>0:\left|\frac{f(d+\Delta)-f(d)}{\Delta}\right|\leq|f'(d)|+1$ where $U$ is some [[Neighborhood of real points|Neighborhood]] of $0$ 
- In other words: $\forall\Delta\in\;]-r;+r[\;, \Delta>0:|f(d+\Delta)-f(d)|\leq(|f'(d)|+1)\times\Delta$ 
- So, $\forall\varepsilon\in\mathbb R,\varepsilon>0: \Delta< \min\left\{r,\frac{\varepsilon}{|f'(d)|+1}\right\}\implies$ $|f(d+\Delta)-f(d)|\leq(|f'(d)|+1)\times\Delta\leq\varepsilon\implies f$ is [[Continuity|continuous]] at point $d$ 