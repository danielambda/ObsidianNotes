---
tags:
  - Math
  - AGLA
  - Optimization
---
## Task
- A guy drew the [[Line]] on the floor. We want to know the [[General Equation of a Line|Equation of this Line]]. We send a robot which follows the line and obtain a dataset from GPS.
- Equation of the line is $y=kx+t$. Hence, there are 2 unknows variables. But we obtain 3 equations from 3 points. Our system is overdetermined (more equations than variables)
- We have to reformulate our task. Let's fit all the points on the [[Line]], where the distance between points and our resulted line will be minimal.
- There are two ways of thinking
	1. Calculus ([[Derivative]])
		- $\displaystyle\frac{dE^2}{dm}=0$
	2. Linear Algebra way ([[Projection]])
		- $A^\intercal Am=A^\intercal y$
## [[1. Analytic Geometry & Linear Algebra II|Linear Algebra]] Approach
### Application
$$y=kx+t\iff\begin{cases}t+k\cdot 1=1\\t+k\cdot 2=2\\t+k\cdot 3=1\end{cases}\implies Ax=b\iff\left[\begin{matrix}1&1\\1&2\\1&3\end{matrix}\right]\left[\begin{matrix}t\\k\end{matrix}\right]=\left[\begin{matrix}1\\2\\1\end{matrix}\right]$$
$$A^\intercal A x=A^\intercal b\iff \left[\begin{matrix}1&1&1\\1&2&3\end{matrix}\right]\left[\begin{matrix}1&1\\1&2\\1&3\end{matrix}\right]\left[\begin{matrix}t\\k\end{matrix}\right]=\left[\begin{matrix}1&1&1\\1&2&3\end{matrix}\right]\left[\begin{matrix}1\\2\\1\end{matrix}\right]\iff\left[\begin{matrix}3&6\\6&14\end{matrix}\right]\left[\begin{matrix}t\\ k\end{matrix}\right]=\left[\begin{matrix}4\\8\end{matrix}\right]\iff$$
$$\iff \left[\begin{matrix}t\\k\end{matrix}\right]=\left[\begin{matrix}\displaystyle\frac43 \\0\end{matrix}\right]$$
## [[1. Mathematical Analysis II|Math Analysis]] Approach
- Define the sum of squared residuals: $$S(k, b)=\sum_{i=1}^n(y_i-kx_i-b)^2$$
- The minimum of the [[Function]] with respect to parameters $k, b$ defines the best approximation. The conditions are: $$\begin{cases}\displaystyle\frac{\partial S}{\partial k}=2\sum_{i=1}^nx_i(y_i-kx_i-b)=0\\\displaystyle\frac{\partial S}{\partial b}=2\sum_{i=1}^n(y_i-kx-b)=0\end{cases}$$ 
### Example
- Consider the set of points $(1,2),(2,1),(3,3)$. Define the sum of squared residuals: $$S(k,b)=(k+b-2)^2+(2k+b-1)^2+(3k+b-3)^2$$$$\begin{cases}\displaystyle\frac{\partial S}{\partial k}=28k+12b-26=0\\\displaystyle\frac{\partial S}{\partial b}=12k+6b-12=0\end{cases}\iff\begin{cases}14k+6b=13\\12k+6b=12\end{cases}\implies\begin{cases}k=1/2\\b=1\end{cases}$$