$$\Large M=35$$
## Task 
Prove (using the definition of the [[Derivative]]) that 
$$(𝑥 𝑀) ′ = 𝑀𝑥 𝑀−1 and ( 1⁄ 𝑥𝑀) ′ = − 𝑀 𝑥 ⁄ (𝑀+1)$$
$$(x^M)'=Mx^{M-1}\;\&\;\left(\frac{1}{x^M}\right)'=\frac{-M}{x^{(M+1)}}$$
## Solution 
$M=10+25=35$
1. $f(x)=x^{35}$:
[[Derivative|Definition:]]
$$f'(x)=\lim_{\Delta\to0}\frac{f(x+\Delta)-f(x)}{\Delta}$$
$\displaystyle f'(x)=\lim_{\Delta\to0}\frac{(x+\Delta)^{35}-x^{35}}{\Delta}=$
$=\displaystyle\lim_{\Delta\to0}\frac{x^{35}+35x^{34}\Delta+a_2x^{33}\Delta^2+...+a_{33}x^2\Delta^{33}+a_{34}x\Delta^{34}+\Delta^{35}-x^{35}}{\Delta}=$
$=\displaystyle\lim_{\Delta\to0}\left(35x^{34}+a_2x^{33}\Delta+...+a_{33}x^2\Delta^{32}+a_{34}x\Delta^{33}+\Delta^{34}\right)=$
$=\displaystyle(35x^{34}+a_2x^{33}0+...+a_{33}x^2 0^{32}+a_{34}x0^{33}+0^{34})=35x^{34}, \square$
2. $\displaystyle f(x)=\frac{1}{x^{35}}$
[[Derivative|Definition]]:
$$f'(x)=\lim_{x\to x_0}\frac{f(x_0)-f(x)}{x_0-x}$$
$\displaystyle f'(x)=\lim_{x\to x_0}\frac{\frac{1}{x_0^{35}}-\frac{1}{x^{35}}}{x_0-x}=$ 
$=\displaystyle\lim_{x\to x_0}\frac{x^{35}-x_0^{35}}{(x_0-x)(x_0x)}=$
$=\displaystyle\lim_{x\to x_0}\frac{-(x_0-x)(x^{34}+x^{33}x_0+x^{32}x_0^2+...+x^2x_0^{32}+xx_0^{33}+x_0^{34})}{(x_0-x)(x^{35}_0x^{35})}=$
$=\displaystyle\lim_{x\to x_0}\frac{-(x^{34}+x^{33}x_0+x^{32}x_0^2+...+x^2x_0^{32}+xx_0^{33}+x_0^{34})}{x^{35}_0x^{35}}=$
$=-\displaystyle\lim_{x\to x_0}\left(\frac{1}{x_0^{35}x}+\frac{1}{x_0^{34}x^2}+\frac{1}{x_0^{33}x^3}+...+\frac{1}{x_0^{3}x^{33}}+\frac{1}{x_0^{2}x^{34}}+\frac{1}{x_0x^{35}}\right)=$
$=-\displaystyle\left(\frac{1}{x^{35}x}+\frac{1}{x^{34}x^2}+\frac{1}{x^{33}x^3}+...+\frac{1}{x^{3}x^{33}}+\frac{1}{x^{2}x^{34}}+\frac{1}{xx^{35}}\right)=\frac{-35}{x^{36}},\square$
$\blacksquare$ 