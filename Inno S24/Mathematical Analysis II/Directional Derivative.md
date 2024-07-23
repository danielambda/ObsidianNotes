---
tags:
  - Math
  - MathematicalAnalysis
  - Geometry
---
## Definition
- Directional derivative can be obtained by the following track:
	1. Define direction $\overline s=(s_1,...,s_N), ||\overline s||=1$
	2. Specify the certain point $A=(a_1,...,a_N)$
	3. Define the dependence of the coordinates:
		- $x_1=a_1+s_1t$
		- $\vdots$
		- $x_N=a_N+s_Nt$
	4. Substitute the dependence into the [[Function]]:
		- $f(x_1,...,x_N)=f(a_1+s_1t,...,a_n+s_nt))$
	5. Find full derivative on $t$:
$$\frac{df}{dt}=\frac{\partial f}{\partial x_1}\frac{dx+1}{dt}+...+\frac{\partial f}{\partial x_N}\frac{dx_N}{dt}=$$$$\large=\left(\frac{\partial f}{\partial x_1}s_1+...+\frac{\partial f}{\partial x_N}s_N\right)\bigg|_{(x_1,...x_N)=(a_1,...,a_N)}$$
