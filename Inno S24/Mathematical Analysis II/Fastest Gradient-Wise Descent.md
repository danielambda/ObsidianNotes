---
tags:
  - Math
  - MathematicalAnalysis
  - Optimization
---
## Method
- Change the [[Gradient-Wise Descent]] method for the opposite gradient direction as [[Function]] of the variable $\Delta$: $$\Phi(\Delta)=F(X-\overline\nabla F(X)\cdot\Delta),\set{x_1,...x_N}=\text{const}$$
- So we seek the minimum of the 1D [[Function]] $\Phi(\Delta)$ on the given direction
	1. Define an interval $\Delta\in[0,b]$ such that $\Phi(\Delta)\leq\Phi(0)$
	2. Find a minimum $\Phi(\Delta^*), \Delta^*\in[0,b]$
	3. The point $Y=X-\overline\nabla F(X)\cdot\Delta^*$ is considered as next position for the next step.
	4. If $||X-Y||>\delta$ then this process repeats
## Example
- Consider [[Function]] $$f(x,y)=(x+y)^2+3(x-y)^2$$
- The level curves are [[Ellipse]]s with big semi axis along the straight [[Line]] $x=y$ and the minimum is $(0,0)$
---
- Let the initial point to be $A=(2,3)$ 
	- then $f(2,3)=28$
- Find the [[Derivative]]s and the [[Gradient of the Function]]: $$\frac{\partial f}{\partial x}=8x-4y,\;\frac{\partial f}{\partial y}=-4x+8y,\;\overline\nabla f(2,3)=(4,16)$$
- Then the descent direction starting at the point $A$ is: $$\begin{cases}x=2-4t\\ y=3-16t\end{cases}, t>0$$
- The minimized 1D [[Function]] is: $$f(x(t),y(t))=832t^2-272t+28=...$$
- Minimum of the [[Function]] is at the $t=\frac{272}{2\cdot 832}$
- $x=2-4t\approx 1.35$, $y=3-16t\approx 0.38$, $f(x,y)\approx 5.77$
- And then you have to do the same thing a couple more infinities times