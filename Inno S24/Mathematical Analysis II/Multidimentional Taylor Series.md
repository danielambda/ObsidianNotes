---
tags:
  - MathematicalAnalysis
  - Math
---
## Recall [[Taylor Series]]
## Formula
$\displaystyle T_f(X, P)=$
$\displaystyle f(P)+$
$\displaystyle \frac{1}{1!}\sum_{i=1}^n\frac{\partial f(P)}{\partial x_i}\cdot(x_i-p_i)+$
$\displaystyle \frac{1}{2!}\sum_{i=1}^n\sum_{j=1}^n\frac{\partial^2 f(P)}{\partial x_i\partial x_j}\cdot(x_i-p_i)(x_j-p_j)+$
$\displaystyle \frac{1}{3!}\sum_{i=1}^n\sum_{j=1}^n\sum_{k=1}^n\frac{\partial^3 f(P)}{\partial x_i\partial x_j\partial x_k}\cdot(x_i-p_i)(x_j-p_j)(x_k-p_k)+\dots$
### Or
$$T_f(X,P)=\sum_{i=0}^\infty\frac{1}{i!}((X-P)\cdot\nabla)^i f(P)$$
### Or
$$T_f(X,P)=\frac{f(P)}{0!}+\frac{(X-P)^\intercal\nabla f(P)}{1!}+\frac{(X-P)^\intercal\nabla\nabla f(P)(X-P)}{2!}+...$$
## Example
$f(x,y)=(x+y)^2\sin(y)$ at $P=(1,0)$
- $f(P)=0$
- $\overline\nabla f(x,y)=(2x(x+y)\sin(y),2y(x+y)\sin(y)+(x+y)^2\cos(y))$
	- $\overline\nabla f(P)=(0,1)$
- $(X-P)^\intercal\overline\nabla f(P)=(x-1\;y-0)\left(\begin{matrix}0\\1\end{matrix}\right)=y$ $$\overline{\nabla\nabla}f(x,y)=\left[\begin{matrix}f_{xx}&f_{xy}\\ f_{yx}&f_{yy}\end{matrix}\right]=\left[\begin{matrix}2\sin(y)&2\sin(y)+2(x+y)\cos(y)\\ 2\sin(y)+2(x+y)\cos(y)&2\sin(y)+2(x+y)\cos(y)+2(x+y)\cos(y)-(x+y)^2\sin(y)\end{matrix}\right]=$$
$$=\left[\begin{matrix}0&2\\ 2&4\end{matrix}\right]$$
$$\frac12(X-P)^\intercal\left[\begin{matrix}0&2\\ 2&4\end{matrix}\right](X-P)=\left(\begin{matrix}x-1\\ y\end{matrix}\right)\left[\begin{matrix}0&2\\ 2&4\end{matrix}\right](x-1\;y)=(x-1)y+(x-1)y+2y=2xy$$
$f(x,y)=y+xy+R_3$
