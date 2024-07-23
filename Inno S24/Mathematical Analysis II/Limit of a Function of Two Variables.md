---
tags:
  - Math
  - MathematicalAnalysis
---
## Definition
$$\forall \varepsilon\in\mathbb  R_+\;\exists \delta_\varepsilon\in\mathbb R\;\forall Y: ||Y-X||<\delta_\varepsilon:|F(Y)-A| < \varepsilon\implies \lim_{||Y-X||\to0}F(X) = A$$
## Examples
$$\lim_{X\to0}(x_1^2+x_2^2)=0$$
$$\lim_{X\to(2,1)}(x_1^2+x_2^2)=4+1=5$$
$$\lim_{x_1\to0}\lim_{x_2\to0}\frac{x_2x_2}{x_1^2+x_2^2}=\lim_{x_1\to0}0=0$$

$$\lim_{x_1\to0}\frac{x_2x_2}{x_1^2+x_2^2}\Bigg\vert_{x_2=kx_1}=\lim_{x_1\to0}\frac{x_1kx_1}{x_1^2+k^2x_1^2}=\frac{k}{1+k^2}$$
$$\lim_{r\to0}\frac{x_2x_2}{x_1^2+x_2^2}\Bigg\vert_{x_1=r\cos(\alpha),x_2=r\sin(\alpha)}=\lim_{r\to0}\frac{r^2\cos(\alpha)\sin(\alpha)}{r^2}=\frac{\sin(2\alpha)}{2}$$