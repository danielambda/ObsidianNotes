---
tags:
  - MathematicalAnalysis
  - Math
  - DifferetialForms
  - ExteriorAlgebra
  - GeometricAlgebra
---
## Definition
- An $m$-form on $T_p\mathbb R^n$ is a [[Function]] $\omega: (T_p\mathbb R^n)^m\to\mathbb R$
	- $\omega$ is multilinear
	- $\omega$ is alternating
## Multilinearity
- $u_i\in T_p\mathbb R^n$, $v,w\in T_p\mathbb R^n$, $a,b\in\mathbb R$
$\omega(u_1,...u_{i-1},av+bw,u_{i+1},...,u_m)=a\omega(u_1,...u_{i-1},v,...,u_m)+b\omega(u_1,...u_{i-1},w,u_{i+1},...,u_m)$
## Alternating
- Well, I'm lazy to write latex code for this, so, I'll just say, that this thing means that swapping 2 input vectors of $\omega$ will change the sign of the output. Similar, as in [[Determinant  of a Matrix]] 
## For [[1-Form]]s $\omega_1,...,\omega_m$
- Define $m$-form
$$(\omega_1\wedge...\wedge\omega_m)(v_1,...,v_m)=\left|\begin{matrix}
\omega_1(v_1)&...&\omega_m(v_1)\\
\vdots&\ddots&\vdots\\
\omega_1(v_m)&...&\omega_m(v_m)
\end{matrix}\right]$$
## Fact
- Every $m$-form on $T_p \mathbb R^n$ can be written 
$$\omega=\sum_{1\leq i_1\leq...\leq i_m\leq n}a_{i_1...i_m}dx_1\wedge...\wedge dx_m$$