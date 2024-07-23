---
tags:
  - Math
  - AGLA
---
## Definition
- Cross-product $\overline a\times\overline b$ is a vector $\overline c$ that is perpendicular to both $\overline a$ and $\overline b$ and its length is equal to the area of the parallelogram with  $\overline a$ and $\overline b$ as its sides.
- $\overline a\times\overline b$ is defined only in 3D space
## Computation
### Classical method
$\overline a\times\overline b = det\left(\begin{matrix}\overline i & \overline j & \overline k\\ a_x&a_y&a_z\\ b_x&b_y&b_z\end{matrix}\right) = \left|\begin{matrix}\overline i & \overline j & \overline k\\ a_x&a_y&a_z\\ b_x&b_y&b_z\end{matrix}\right| =$ see on [[Determinant  of a Matrix]]
### Skew-symmetric matrix method
$\hat {\overline a} = \left[\begin{matrix}0&-a_z&a_y\\ a_z&0&-a_x\\ -a_y&a_x&0\end{matrix}\right]$
- $\overline a\times\overline b = \hat{\overline a} * \overline b$
	- since $\hat{\overline a}$ is a matrix $\hat{\overline a} * \overline b$ is a simple vector-matrix multiplication
$\overline a\times\overline b = \hat{\overline a} * \overline b = \left[\begin{matrix}0&-a_z&a_y\\ a_z&0&-a_x\\ -a_y&a_x&0\end{matrix}\right]\left[\begin{matrix}b_x\\ b_y\\ b_z\end{matrix}\right] = \left[\begin{matrix} допишуКогдаБудетСкучно\end{matrix}\right]$
### Geometrical method ||magnitude only||
- $||\overline a \times \overline b|| = ||\overline a|| * ||\overline b|| * sin\angle(\overline a, \overline b)$
## Properties
- $\overline a\times\overline b = -\overline b \times \overline a$
- $\overline a\times(\overline b + \overline c) = \overline a\times\overline b + \overline a \times \overline c$
- $\lambda\overline a\times\overline b = \lambda(\overline a \times\overline b)$
- $\overline a \times\overline a = \overline 0$
- $\overline a \times\overline b = 0\iff\overline a \parallel \overline b$
