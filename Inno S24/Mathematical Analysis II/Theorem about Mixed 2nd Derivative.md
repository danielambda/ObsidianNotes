---
tags:
  - Math
  - MathematicalAnalysis
---
## Theorem
- Let $f(X)$ be differentiable [[Function]] and all [[Derivative]]s of the first and second order are continuous
- Then $$\frac{\partial^2 f}{\partial x_ix_j}=\frac{\partial^2 f}{\partial x_j\partial x_i}$$
## Proof
- To be shorter, define $f_0=f(0,0)$
- For simplicity consider the [[Function]] of 2 variables $X=(x,y)$ and write the [[Function]] using [[Taylor Series]] for the first and second variable by [[Sequence]]:
$$f(x,y)=f(0,y)+\frac{\partial f}{\partial x}(0,y)x+\frac12\frac{\partial ^2f}{\partial x^2}(0,y)x^2+o(x^2)=$$$$=f_0+\frac{\partial f_0}{\partial y}y+\frac12\frac{\partial^2 f_0}{\partial y^2}y+O(y^2)+\left(\frac{\partial f_0}{\partial x}+\frac{\partial ^2f}{\partial y\partial x}y+o(y)z\right)+\frac12\left(\frac{\partial^2 f_0}{\partial x^2}+o(y)\right)x^2+o(x^2)$$
$$я\;устал$$