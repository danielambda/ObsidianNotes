---
tags:
  - Math
  - MathematicalAnalysis
---
## Definition
- The point of differentiable [[Function]] $f(X)$ where all [[Derivative]]s of first order are 0 is called *extreme point*
## Examples
- For following [[Function]] point $A=(0,0)$ is an extreme point:
	- $f(x,y)=3x^2+x^2$
	$$\frac{\partial f}{\partial x}=6x, \frac{\partial f}{\partial y}=2y$$
## Necessary Condition for Extreme Points
### Theorem
- $f(X)$ is differentiable $\implies\forall i\in\set{1,...,N}:\frac{\partial f}{\partial x_i}$ at the interior [[Local Maxima|maxima]] or [[Local Minima|minima]] point
### Proof
- Suppose $A=(0,0)$ is [[Local Maxima]], and one of the [[Partial Derivative]]s is not 0. 
- Then in the maxima point: $$f(X)=f(0,0)+\frac{\partial f}{\partial x}(0,0)x+o(|x|+|y|)$$
- Then for $\frac{\partial f}{\partial x}(0,0)x>0$ the $f(x,y)>f(0,0)$ which contradict to the initial claim. For the another partial derivative one can consider by the same way. As result one gets the claim of the theorem.