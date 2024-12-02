---
tags:
  - Math
  - MathematicalAnalysis
---
## Definition
- Let $f,q:D\to\mathbb R, D\subseteq\mathbb R_{\pm\infty}\;\&\;d\in\mathbb R_{\pm\infty};$ function $f$ is said to be little $o$ of the function $g$ as the argument tends to $d$ ($f(x)\in o(g(x)), x\to d$)
- If $\forall\varepsilon\in\mathbb R, \varepsilon>0\;\exists$ a neighborhood $U$ of $d:\;\forall x\in U\;|f(x)|\leq\varepsilon\times|g(x)|$ 
## Statement
$\displaystyle\frac{1}{x} \in o(1)\;as\;x\to+\infty$
## Proof
Let $\displaystyle\varepsilon\in\mathbb R, \varepsilon>0: \left|\frac{1}{x}\right|\leq\varepsilon *1 =\varepsilon$  
$\displaystyle\forall x\geq\frac{1}{\varepsilon}:\frac{1}{x}\geq\varepsilon$
Let $\displaystyle U = \left[\frac{1}{\varepsilon};+\infty\right[$ 
Therefore, statement is true by definition, $\blacksquare$
## Transitivity
$x\to d: f(x)\in o(g(x))\;\&\;g(x)\in o(h(x))\implies f(x)\in o(h(x))$
#### Proof
$(1)$ Let $f(x)\in o(g(x)), x\to d\iff$
$\iff (2)\forall\varepsilon_2>0\;\exists$ [[Neighborhood of real points|neighborhood]] $U$ of $d: \forall x\in U|f(x)|\leq\varepsilon_2|g(x)|$
$(3)$ Let $g(x)\in o(h(x)), x\to d\iff$
$\iff (2)\forall\varepsilon_4>0\;\exists$ [[Neighborhood of real points|neighborhood]] $V$ of $d: \forall x\in U|g(x)|\leq\varepsilon_4|h(x)|$
$(5)$ Let $\varepsilon>0$
	according to $(4)$: $\exists V: |g(x)|\leq\varepsilon|h(x)|$
	according to $(2)$: $\exists U: |f(x)|\leq1|g(x)|$
$(6)$ Let $W =U\cap V$, $W$ is a neighborhood of $d$
	$\forall x\in W:|f(x)|\leq|g(x)|\leq\varepsilon|h(x)|\implies\forall x\in W:|f(x)|\leq\varepsilon|h(x)|, Q.E.D.\blacksquare$
## Notes
- $\displaystyle f(x)\in o(g(x))\iff\lim_{x\to\infty}\frac{f(x)}{g(x)} = 0$