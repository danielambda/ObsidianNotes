---
tags:
  - Math
  - Optimization
---
## Objective
- Solving specific [[Linear Programing Problem]]s
## Requirements
- The [[Linear Programing Problem]] has to satisfy
	- All the constraints are equations with nonnegative right-hand side
	- All the variable are nonnegative
## Example
#### Problem
$$\text{Maximize } z = 5x_1+4x_2+3x_3$$
$$\text{Subjected to }
\\
\begin{cases}
2x_1+3x_2+x_3\leq5 \\
4x_1+x_2+2x_3\leq11\\
3x_1+4x_2+2x_3\leq 8
x_1,x_2,x_3\geq0
\end{cases}$$
#### Solution
- For each of the less-than inequalities we use *slack variables* that represents the difference between the right-hand side and the left-hand side. For example, for the first inequality, we introduce the slack variable $s_1$ defined by $$
s_1=5-2x_1-3x_2-x_3$$
- We carry out this procedure for each of the less-than constraints to get an equivalent representation of the problem:  $$
\text{Maximize } z = 5x_1+4x_2+3x_3
$$$$\text{Subjectd to} \begin{cases}
s_1=5-(2x_1+3x_2+x_3)\\
s_2 = 11 - (4x_1+x_2+2x_3)\\
s_3 = 8 - (3x_1+4x_2+2x_3)
\end{cases}$$
- The simplex method is an iterative process in which we start with a solution $x_1, x_2, ...,s_3$ that satisfies the equations and non-negativities and then look for a new solution $\overline x_1,\overline x_2,...,\overline s_3$, which is better in the sense that it has a larger objective function value (in maximization problems):$$
5\overline{x}_1 +4\overline x_2+3\overline x_3>5x_1+4x_2+3x_3
$$ When we stop? We continue this process until we arrive at a solution that can’t be improved. This final solution is then an optimal solution