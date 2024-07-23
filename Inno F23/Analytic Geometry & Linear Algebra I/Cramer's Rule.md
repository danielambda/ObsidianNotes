---
tags:
  - Math
  - AGLA
---
## General Case
$A\overline x=\overline b$
$A$ is a $n\times n$ [[Matrix]] with nonzero [[Determinant  of a Matrix|determinant]]
$\overline x=(x_1,...,x_n)^\top$ is the column [[Vector]] of the variables
$$x_i=\frac{det(A_i)}{det(A)}$$ where $A_i$ is the matrix formed be replacing $i$-th column of $A$ by column vector $\overline b$ 
## Example
$$
\begin{cases}
2x+y-z=4\\
4x-y+2z=23\\
-x+3y-2z=0
\end{cases}\iff\left[
\begin{matrix}
2&1&-1\\ 
4&-1&2\\
-1&3&-2
\end{matrix}\right]
\left(\begin{matrix}x\\y\\z\end{matrix}\right)=\left(\begin{matrix}4\\23\\0\end{matrix}\right)
$$
$det(A)=2(-1)(-2)+1*2(-1) +(-1)4*3-2*2*3-1*4(-2)-(-1)(-1)(-1)=$$=4-2-12-12+8+1=-13$ 
$det(A_x)=\left|\begin{matrix}4&1&-1\\23&-1&2\\0&3&-2\end{matrix}\right|=8+0-69-24+46-0=-39$
$det(A_y)=-92-8+0-0+32-23=-91$
$det(A_z)=0-23+48-138-0-4=-117$
$$\begin{cases}x=\frac{-39}{-13}=3 \\ y=\frac{-91}{-13}=7\\z=\frac{-117}{-13}=9\end{cases}$$
### Alternative Solution ([[Inverse Matrix]])
$$
\begin{cases}
2x+y-z=4\\
4x-y+2z=23\\
-x+3y-2z=0
\end{cases}\iff\left[
\begin{matrix}
2&1&-1\\ 
4&-1&2\\
-1&3&-2
\end{matrix}\right]
\left(\begin{matrix}x\\y\\z\end{matrix}\right)=\left(\begin{matrix}4\\23\\0\end{matrix}\right)
$$
$$
\left(\begin{matrix}x\\y\\z\end{matrix}\right)=\left[
\begin{matrix}
2&1&-1\\ 
4&-1&2\\
-1&3&-2
\end{matrix}\right]^{-1}\left(\begin{matrix}4\\23\\0\end{matrix}\right)$$

$det(A)=2(-1)(-2)+1*2(-1) +(-1)4*3-2*2*3-1*4(-2)-(-1)(-1)(-1)=$$=4-2-12-12+8+1=-13$ 
$A^{-1}=\frac{1}{-13}\left[\begin{matrix}-4&6&11\\-1&-5&-7\\1&-8&-6\end{matrix}\right]^\top=\frac{1}{13}\left[\begin{matrix}4&1&-1\\-6&5&8\\-11&7&6\end{matrix}\right]$
$\left(\begin{matrix}x\\y\\z\end{matrix}\right)=\frac{1}{13}\left[\begin{matrix}4&1&-1\\-6&5&8\\-11&7&6\end{matrix}\right]\left(\begin{matrix}4\\23\\0\end{matrix}\right)=\frac{1}{13}\left(\begin{matrix}16+23+0\\-24+115+0\\-44+161+0\end{matrix}\right)=\frac{1}{13}\left(\begin{matrix}39\\91\\117\end{matrix}\right)=$
$$\left(\begin{matrix}3\\7\\9\end{matrix}\right)$$
