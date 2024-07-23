---
tags:
  - MathematicalAnalysis
  - Math
  - AGLA
  - Geometry
---
## Geometry
- Let [[Function]] $f(x,y)$ be a definition of some surface in $\mathbb R^3: z=f(x,y)$
- Define the inclination along the direction of $x$ axis: $f_x=\frac{\partial f}{\partial x}$
- Define the inclination along the direction of $y$ axis: $f_y=\frac{\partial f}{\partial y}$
- The [[Vector]] $\overline\phi=(f_x, f_y)$ defines a [[Projection]] on the [[Plane]] $(x,y)$ of the surface inclination at the current point $(x,y)$
## Normal [[Vector]]
- Rewrite the equation for the surface in the form: $$z-f(x,y)=0$$
 - The differential on the surface should be following: $$dz-\frac{\partial f}{\partial x}dx-\frac{\partial f}{\partial y}dy=0$$
 - This equality should be fulfilled for any curve on this surface $(x(t),y(t),z(t))$.
 - This equality is the [[Vector Dot Product]] for the [[Vector]] $$\overline N=\left(\frac{\partial f}{\partial x},\frac{\partial f}{\partial y}, -1\right)$$ and the [[Vector]] of differential for any curve on the surface. As well as the differential defines the tangent lines for the surface, then $\overline N$ is a normal [[Vector]] for the surface at the point $(x_0, y_0, f(x_0, y_0))$
## Tangent [[Plane]]
- Tangent [[Plane]] can be derived from Normal [[Vector]]
- For surface $z=f(x,y)$ tangent [[Plane]] at the point $(x_0, y_0, f(x_0, y_0)):$
$$\large\frac{\partial f}{\partial x}(x_0, y_0)(x-x_0)+\frac{\partial f}{\partial y}(x_0, y_0)(y-y_0)-(z-f(x_0, y_0)=0)$$
## Tangent [[Plane]] for Implicit case
- The [[Function]] $F(x,y,z)=0$ defines 2D manifold in general case. $$dF=\frac{\partial F}{\partial x}dx+\frac{\partial F}{\partial y}dy+\frac{\partial F}{\partial z}dz$$
- For any curve on this surface $(x(t), y(t),z(t)):$ $$\frac{\partial F}{\partial x}dx+\frac{\partial F}{\partial y}dy+\frac{\partial F}{\partial z}dz=0$$
- The $\overline V=(x',y', z')$ define the differential of the curve, then $$\overline N=\left(\frac{\partial F}{\partial x}, \frac{\partial F}{\partial y}, \frac{\partial F}{\partial z}\right)$$
- Is the normal [[Vector]] for the surface. The tangent plane at point $(x_0, y_0, z_0)$ has the form: $$\frac{\partial F}{\partial x}(x_0,y_0,z_0)(x-x_0)+\frac{\partial F}{\partial y}(x_0,y_0,z_0)(y-y_0)+\frac{\partial F}{\partial z}(x_0,y_0,z_0)(z-z_0)=0$$