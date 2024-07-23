---
tags:
  - Math
  - AGLA
---
## Definition
- For given [[Matrix]] $A$ decomposition $$A=U\Sigma V^H$$
- Where $U, V$ are [[Orthonormal Matrix|orthonormal]], $\Sigma$ is [[Diagonal Matrix]]
- Is called Singular Value Decomposition
## Further Notation
$$U=\left[\begin{matrix}
|&...&|\\
\overline u_1&...&\overline u_n\\
|&...&|
\end{matrix}\right], V=\left[\begin{matrix}
|&...&|\\
\overline v_1&...&\overline v_n\\
|&...&|
\end{matrix}\right], \Sigma=\left[\begin{matrix}
\sigma_1&0&\dots&0\\
0&\sigma_2&\dots&0\\
\vdots&\vdots&\ddots&\vdots\\
0&0&\dots&\sigma_n
\end{matrix}\right]$$
## Some Notes
$$A^HA=\left(U\Sigma V^H\right)U\Sigma V^H=V\Sigma^H U^HU\Sigma V^H=V\Sigma^H \Sigma V^H=V\Sigma^2 V^H=V\Sigma^2 V^{-1}=S\Lambda S^{-1}$$
$$AA^H=U\Sigma^2U^{-1}$$
## Example
$$A=\left[\begin{matrix}4&4\\-3&3\end{matrix}\right]$$
$$A^\intercal A=\left[\begin{matrix}4&-3\\4&3\end{matrix}\right]\left[\begin{matrix}4&4\\-3&3\end{matrix}\right]=\left[\begin{matrix}25&7\\7&25\end{matrix}\right]$$
$$\lambda_1=25-7=18,\lambda_2=25-(-7)=32$$
$$(A^\intercal A-\lambda_1I)=\left[\begin{matrix}7&7\\7&7\end{matrix}\right], (A^\intercal A-\lambda_2I)=\left[\begin{matrix}-7&7\\7&-7\end{matrix}\right]$$
$$v_2=\left[\begin{matrix}1\\1\end{matrix}\right], v_1=\left[\begin{matrix}1\\-1\end{matrix}\right]$$
$$V=S=\frac1{\sqrt2}\left[\begin{matrix}1&1\\1&-1\end{matrix}\right]$$
$$\Sigma^2=\Lambda=\left[\begin{matrix}32&0\\0&18\end{matrix}\right]\implies\Sigma=\left[\begin{matrix}4\sqrt2&0\\0&3\sqrt2\end{matrix}\right]$$
Here I could've do the same thing for $AA^\intercal$ to find $U$ but I'm lazy and can do another thing: $$A=U\Sigma V^\intercal=U\left[\begin{matrix}4\sqrt2&0\\0&3\sqrt2\end{matrix}\right]\frac1{\sqrt2}\left[\begin{matrix}1&1\\1&-1\end{matrix}\right]$$
$$\left[\begin{matrix}4&4\\-3&3\end{matrix}\right]=U\left[\begin{matrix}4\sqrt2&0\\0&3\sqrt2\end{matrix}\right]\frac1{\sqrt2}\left[\begin{matrix}1&1\\1&-1\end{matrix}\right]=U\left[\begin{matrix}4&0\\0&3\end{matrix}\right]\left[\begin{matrix}1&1\\1&-1\end{matrix}\right]=U\left[\begin{matrix}4&4\\3&-3\end{matrix}\right]\implies$$
$$\implies U=\left[\begin{matrix}1&0\\0&-1\end{matrix}\right]$$
$$\left[\begin{matrix}4&4\\3&-3\end{matrix}\right]=\left[\begin{matrix}1&0\\0&-1\end{matrix}\right]\left[\begin{matrix}4\sqrt2&0\\0&3\sqrt2\end{matrix}\right]\left[\begin{matrix}\frac1{\sqrt2}&\frac1{\sqrt2}\\\frac1{\sqrt2}&\frac{-1}{\sqrt2}\end{matrix}\right]$$