## Task 1 Model 2
- Find the area limited by the region $$R=\set{x=1,y=a^2x,xy=b^2}$$where $a > 0, b>0$
## Solution
- Since $b>0$, $xy=b^2\iff y=\frac{b^2}{x}$
- Intersection of $y=a^2x$ and $y=\frac{b^2}{x}:$ $$a^2x=\frac{b^2}{x}\implies x^2=\frac{b^2}{a^2}\implies x=\pm\frac{b}{a}$$
- Тут надо несколько слов сказать про то, что область ограничивается именно около $+\frac ba$, а про $-\frac ba$ можно забыть и т.д.
- 3 cases:
- $\displaystyle \frac b a = 1:$ all lines intersect in single point, hence, the area of region $R$ is 0.
- $\displaystyle \frac ba>1:$
$$\text{Area}=\int_1^{b/a}\int_{a^2x}^{b^2/x}dydx$$
- $\displaystyle\frac b a < 1:$ $$\text{Area}=\int_{b/a}^1\int_{b^2/x}^{a^2x}dydx=-\int^{b/a}_1\int_{b^2/x}^{a^2x}dydx=-\left(-\int_{b/a}^1\int^{b^2/x}_{a^2x}dydx\right)$$
As we can see, we obtained the exact same expression for last 2 cases:
$$\int_1^{b/a}\int_{a^2x}^{b^2/x}dydx=\int_1^{b/a}\left(\frac{b^2}{x}-a^2x\right)dx=\left[b^2\ln x-\frac{a^2x^2}{2}\right]_1^{b/a}=$$
$$=\left(b^2\ln\frac{b}{a}-\frac{b^2}{2}\right)-\left(0-\frac{a^2}{2}\right)=\Large b^2\ln\frac b a+\frac{a^2-b^2}{2}$$