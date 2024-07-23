---
tags:
  - Math
  - AGLA
---
## 3D case [[Projection]] [[Matrix]] 
### Project $b$ onto a [[Plane]] with [[Basis]] $x,y$
- Let $A=\left[\begin{matrix}x&y\end{matrix}\right]=\left[\begin{matrix}x_1&&y_1\\ x_2&&y_2\end{matrix}\right]$
$$proj\;b=\hat b=Ax\implies e=b-\hat b\perp \hat b\implies A^\intercal(b-Ax)=0$$
$$A^\intercal b=A^\intercal Ax\implies x=(A^\intercal A)^{-1}A^\intercal b\implies Ax=\hat b=A(A^\intercal A)^{-1}A^\intercal b$$
$$\Large P=A(A^\intercal A)^{-1}A^\intercal$$
### Project $b$ onto a $d\perp$ to a [[Plane]] with [[Basis]] $x, y$
- Let $A=\left[\begin{matrix}x&y\end{matrix}\right]=\left[\begin{matrix}x_1&&y_1\\ x_2&&y_2\end{matrix}\right]$
$$\Large P_d=I-P$$
Well, just have to think about it a bit