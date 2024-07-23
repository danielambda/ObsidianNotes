---
tags:
  - Math
  - MathematicalAnalysis
---
## Definition
$$sinc(x) = \begin{cases}1, if \; x = 0\\ {\Large\frac{\sin x}{x}}, if\; x \not=0\end{cases}\ $$

## Proof 
### Statement
- $\displaystyle\lim_{x\to0}\frac{\sin x}{x} = 1$
### Proof
![[Pasted image 20231002130632.png]]
- $AB = AC = 1$
- $S_{ABC} = \frac{1}{2}AB*CH=\frac{1}{2} * 1 * \sin x = \frac{1}{2}\sin x$
- $S_{\circ_{ABC}} = \frac{x}{2\pi} S_\circ = \frac{x}{2\pi} \pi r = \frac{x}{2}$
- $S_{ABD} = \frac{1}{2}AB*BD = \frac{1}{2} 1 * \tan x = \frac{1}{2}\tan x$
- $S_{ABC} < S_{\circ_{ABC}} < S_{ABD} \iff \frac{1}{2}\sin x < \frac{x}{2}<\frac{1}{2}\tan x \iff \sin x < x < \tan x$
$$\iff 1 < \frac{x}{\sin x}<\frac{1}{\cos x} \iff \cos x < \frac{\sin x}{x}<1 $$
- $\lim_\limits{x\to0} \cos x = 1$
- $\lim_\limits{x\to0} 1 = 1$
- Using [[Squeezing lemma]], it results: $$\lim_\limits{x\to0} \frac{\sin x}{x} = 1, Q.E.D. \blacksquare$$