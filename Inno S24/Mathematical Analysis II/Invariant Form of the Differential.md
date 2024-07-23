---
tags:
  - Math
  - MathematicalAnalysis
---
## 2D case
- Consider the changing of coordinated for $x,y$: $$x=x(u,v), y=y(u,v)$$
- Suppose $x(u,v), y(u,v)$ are [[Derivative|differentiable]]
$$df=\frac{\partial f}{\partial x}dx+\frac{\partial f}{\partial y}dy=$$
$$=\frac{\partial f}{\partial x}\left(\frac{\partial x}{\partial u}du + \frac{\partial x}{\partial v}dv\right)+\frac{\partial f}{\partial y}\left(\frac{\partial y}{\partial u}du + \frac{\partial y}{\partial v}dv\right)=$$
$$=\left(\frac{\partial f}{\partial x}\frac{\partial x}{\partial u}+\frac{\partial f}{\partial y}\frac{\partial y}{\partial u}\right)du+\left(\frac{\partial f}{\partial x}\frac{\partial x}{\partial v}+\frac{\partial f}{\partial y}\frac{\partial y}{\partial v}\right)dv=$$
$$\large=\frac{\partial f}{\partial u}du+\frac{\partial f}{\partial v}dv$$
## N-D case
- The changing of variables in general form looks like:
- $X=X(U), X(U)=(x_1,(u_1,...u_N),...,x_N(u_1,...,u_N))$
- In this case the differential has the same form: 
$$df=\sum_{i=1}^N\frac{\partial f}{\partial x_i}dx_i=\sum_{i=1}^N\frac{\partial f}{\partial u_i}du_i$$
## Vector $\overline S$
- [[Vector]] $\overline S$ defines the direction the [[Function]] grows for the given point $X$
$$\overline S=\left(\frac{\partial f}{\partial x_1},...,\frac{\partial f}{\partial x_N}\right)$$
- Actually, $\overline S$ is the [[Gradient of the Function]] 