---
tags:
  - Math
  - AGLA
---
$$\Large
\left(\begin{matrix}
\cos\theta&-\sin\theta\\
\sin\theta&\cos\theta
\end{matrix}\right)$$
## Definition
- A matrix that represents rotation transformation
## Constructing
![[Rotation Matrix.excalidraw]]
$\overline r = \left(\begin{matrix}x\\y\end{matrix}\right)=|r|\left(\begin{matrix}\cos\phi\\\sin\phi\end{matrix}\right)$
$\overline r' = \left(\begin{matrix}x'\\ y'\end{matrix}\right)=|r|\left(\begin{matrix}\cos{(\phi+\theta)}\\\sin{(\phi+\theta)}\end{matrix}\right)$
---
$\displaystyle \frac{x'}{|r|}=\sin(\phi+\theta)=\cos\phi\cos\theta-\sin\phi\sin\theta$
$\displaystyle\frac{y'}{|r|}=\sin(\phi+\theta)=\sin\phi\cos\theta+\cos\phi\sin\theta$
---
$x'=|r|\cos\phi\cos\theta-r\sin\phi\sin\theta = x\cos\theta-y\sin\theta$
$y'=|r|\sin\phi\cos\theta+|r|\cos\phi\sin\theta=x\sin\theta+y\cos\theta$
$$\begin{cases}
x'=x\cos\theta-y\sin\theta\\
y'=x\sin\theta+y\cos\theta
\end{cases}\iff \left(\begin{matrix}x'\\y'\end{matrix}\right)=
\left(\begin{matrix}
\cos\theta&-\sin\theta\\
\sin\theta&\cos\theta
\end{matrix}\right)
\left(\begin{matrix}x\\y\end{matrix}\right)$$
## Theorem
$\forall A$ that is a rotation matrix: $A^{-1} = A^T$
## Proof for n=2
$A^{-1}=\displaystyle\frac{adj{A}}{|A|}=adj{A} = \left(\begin{matrix}\cos\theta&-\sin\theta\\\sin\theta&\cos\theta\end{matrix}\right)^T=\left(\begin{matrix}\cos\theta&\sin\theta\\-\sin\theta&\cos\theta\end{matrix}\right)$ = $A^T, Q.E.D. \blacksquare$ 