---
tags:
  - Math
  - MathematicalAnalysis
---
## Definition
- Suppose $f: \mathbb R^n\to \mathbb R$ is a [[Function]] taking as input a vector $X\in\mathbb R^n$ and outputting some scalar $f(X)\in\mathbb R$
- The [[Matrix]] $$\left[\begin{matrix}f_{x_1x_1}&\dots&f_{x_1x_n}
 \\\vdots&\ddots&\vdots
 \\f_{x_nx_1}&\dots& f_{x_nx_n}
 \end{matrix}\right]$$
 is called Hessian
### Or
$\displaystyle H(f(X))_{i,j}=\frac{\partial^2 f}{\partial x_i\partial x_j}=f_{x_i x_j}$
## Notation
$$\large\nabla\nabla f(x,y,z)=
\left[\begin{matrix}f_{x_1x_1}&\dots&f_{x_1x_n}
 \\\vdots&\ddots&\vdots
 \\f_{x_nx_1}&\dots& f_{x_nx_n}
 \end{matrix}\right]=
 \left[\begin{matrix}
\frac{\partial^2 f}{\partial x\partial x}&\frac{\partial^2 f}{\partial x\partial y}&\frac{\partial^2 f}{\partial x\partial z}
 \\\frac{\partial^2 f}{\partial y\partial x}&\frac{\partial^2 f}{\partial y\partial y}&\frac{\partial^2 f}{\partial y\partial z}
 \\\frac{\partial^2 f}{\partial z\partial z}&\frac{\partial^2 f}{\partial z\partial y}&\frac{\partial^2 f}{\partial z\partial z}
 \end{matrix}\right]$$