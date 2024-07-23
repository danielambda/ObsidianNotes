---
tags:
  - Math
  - AGLA
---
$l_1\;\&\;l_2$ - lines
$\displaystyle l_1=\frac{x-x_1}{p_x}=\frac{y-y_1}{p_y}=\frac{z-z_1}{p_z}$
$\displaystyle l_2=\frac{x-x_2}{q_x}=\frac{y-y_2}{q_y}=\frac{z-z_2}{q_z}$
$$\Large\begin{cases}
\frac{x-x_1}{p_x}=\frac{y-y_1}{p_y}\\
\frac{x-x_1}{p_x}=\frac{z-z_1}{p_z}\\
\frac{x-x_2}{q_x}=\frac{y-y_2}{q_y}\\
\frac{x-x_2}{q_x}=\frac{z-z_2}{q_z}
\end{cases}$$

4 equations and 3 variables $x, y, z$
### Cases
- System is consistent and Exactly 1 solution
	- Rank = 3, 1 point of intersection
- System is inconsistent and 0 solutions
	- $\displaystyle\frac{p_x}{q_x}=\frac{p_y}{q_y}=c_1, \frac{p_z}{q_z}=c_2$
		- $c_1=c_2\iff l_1\parallel l_2$
		- $c_1\not=c_2\iff l_1-/-l_2$
- System is consistent and infinite amount of solutions
	- Rank = 2