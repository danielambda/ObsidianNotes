---
tags:
  - Math
  - MathematicalAnalysis
  - AGLA
---
## Definition
- Let's consider the changing of variables: $y_i=f_i(x)$
- The [[Matrix]] $$\large\left[\begin{matrix}(f_1)_{x_1}&\dots&(f_1)_{x_n}\\
\vdots&\ddots&\vdots\\
(f_n)_{x_1}&\dots&(f_n)_{x_n}\end{matrix}\right]$$
is called Jacobian
### Or
$\displaystyle J(f(X))_{i,j}=\frac{\partial f_i}{\partial x_j}=(f_i)_{x_j}$
## Notation
$$\large\frac{\partial (y_1,y_2,y_3)}{\partial (x_1,x_2,x_3)}=\left[\begin{matrix}\frac{\partial y_1}{\partial x_1}&\frac{\partial y_1}{\partial x_2}&\frac{\partial y_1}{\partial x_3}\\
\frac{\partial y_2}{\partial x_1}&\frac{\partial y_2}{\partial x_2}&\frac{\partial y_2}{\partial x_3}\\
\frac{\partial y_3}{\partial x_1}&\frac{\partial y_3}{\partial x_2}&\frac{\partial y_3}{\partial x_3}\end{matrix}\right]
=\left[\begin{matrix}(y_1)_{x_1}&(y_1)_{x_2}&(y_1)_{x_3}\\
(y_2)_{x_1}&(y_2)_{x_2}&(y_2)_{x_3}\\
(y_3)_{x_1}&(y_3)_{x_2}&(y_3)_{x_3}\\
\end{matrix}\right]$$