---
tags:
  - Math
  - AGLA
---
## Definition
- $det(A)$ is defined only if $A$ is a square matrix
- for $A = \left[\begin{matrix}a\end{matrix}\right]: det(A) = a$
- for $A = \left[\begin{matrix}a&b\\ c&d\end{matrix}\right]: det(A) = ad - bc$
- for $A = \left[\begin{matrix}a&b&c\\ d&e&f\\ g&h&i\end{matrix}\right]:$$det(A) = a*det\left[\begin{matrix}e&f\\ h&i\end{matrix}\right] - b*det\left[\begin{matrix}d&f\\ g&i\end{matrix}\right] + c*det\left[\begin{matrix}d&e\\ g&h\end{matrix}\right]$= $a*e*i - a*f*h - b*d*i + b*f*h + c*d*h - c*e*g$
## [[Cramer's scheme]]