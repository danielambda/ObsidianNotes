---
tags:
  - Math
  - AGLA
---
$$\large Ax+By+Cz+D = 0$$
## From [[Determinant  of a Matrix|determinant]]
$$\left|\begin{matrix}
x-x_0&y-y_0&z-z_0\\
p_x&p_y&p_z\\
q_x&q_y&q_z
\end{matrix}\right| = 0$$
this equation should define a plane because a volume of a shape defined by this 3 vectors is 0 because these 3 vectors are coplanar.
$(x-x_0)A + (y-y_0)B+(z-z_0)C=0$
$A = p_yq_z-p_zq_y; B=p_zq_x-p_zq_x;C=p_xq_y-p_yq_x$
$Ax+By+Cz-Ax_0-By_0-Cz_0 = Ax+By+Cz+D = 0$
## From [[Three Point Equation of a Plane|3 points]]
$P$ is the plane to define
$M_1(x_1, y_1, z_1), M_2(x_2, y_2, z_2), M_3(x_3, y_3, z_3)\in P$

$\overline{MM_1}(x_1-x,y_1-y,z_1-z)$
$\overline{MM_2}(x_2-x,y_2-y,z_2-z)$
$\overline{MM_3}(x_3-x,y_3-y,z_3-z)$
these 3 vectors have to be coplanar 
$$\left|\begin{matrix}
x_1-x&y_1-y&z_1-z\\
x_2-x&y_2-y&z_2-z\\
x_3-x&y_3-y&z_3-z
\end{matrix}\right| = 0$$
from this thing we can get a general equation of a plane
	but it is of degree 3 0_o
### or
$\overline{M_1M}(x-x_1,y-y_1,z-z_1)$
$\overline{M_1M_2}(x_2-x_1,y_2-y_1,z_2-z_1)$
$\overline{M_1M_3}(x_3-x_1,y_3-y_1,z_3-z_1)$
these 3 vectors have to be coplanar 
$$\left|\begin{matrix}
x-x_1&y-y_1&z-z_1\\
x_2-x_1&y_2-y_1&z_2-z_1\\
x_3-x_1&y_3-y_1&z_3-z_1
\end{matrix}\right| = 0$$
this thing looks much prettier