## Task
Find $\int f(x)dx$ for the following $f(x):$
1. $\frac{(M+x)^2}{M+x^2}$
2. $\frac{M}{x^2-Mx+6}$
## Solution 1.
$$\int\frac{(35+x)^2}{35+x^2}dx$$ Let us convert expression
$$\frac{(35+x)^2}{35+x}=\frac{35^2+70x+x^2}{35+x^2}=1+\frac{35\times34}{35+x^2}+\frac{70x}{35+x^2}=$$
$$=1+\frac{34}{1+\frac{x^2}{35}}+\frac{35\times2x}{35+x^2}$$
$$\int\frac{(35+x)^2}{35+x^2}dx=\int dx+34\int\frac{1}{1+\frac{x^2}{35}}dx+35\int\frac{2xdx}{35+x^2}$$
$t=\frac{x}{\sqrt{35}}, dt=\frac{dx}{\sqrt{35}}$
$z=35+x^2, dz=2xdx$
$$x+34\sqrt{35}\int\frac{1}{1+t^2}dt+35\int\frac{dz}{z}=x+34\sqrt{35}\tan^{-1}\frac{x}{\sqrt{35}}+35\ln(35+x^2)+C$$
## Solution 2.
$$\int\frac{35}{x^2-35x+6}dx=35\int\frac{dx}{(x-\frac{35+\sqrt{1201}}{2})(x-\frac{35-\sqrt{1201}}2)}$$
let $a=\frac{\sqrt{1201}+35}2,\overline a=\frac{35-\sqrt{1201}}2\implies a+\overline a=35,a-\overline a=\sqrt{1201}$
let us find $A,B$ such that for every $x$ is true:
$$\frac{1}{(x-a)(x-\overline a)}=\frac{A}{x-a}+\frac{B}{x-\overline a}$$
$$1=A(x-\overline a)+B(x-a)\implies A = -B$$
$$1=A(x-\overline a)-A(x-a)=A(a-\overline a)\implies$$
$$\implies A=\frac{1}{a-\overline a}=\frac{1}{\sqrt{1201}}\implies B=\frac{-1}{\sqrt{1201}}$$
$$35\left(\int\frac{dx}{\sqrt{1201}(x-\frac{35+\sqrt{1201}}{2})}+\int\frac{-dx}{\sqrt{1201}(x-\frac{35-\sqrt{1201}}{2})}\right)=$$
$$=\frac{35}{\sqrt{1201}}\left(\int\frac{dx}{(x-\frac{35+\sqrt{1201}}{2})}-\int\frac{dx}{(x-\frac{35-\sqrt{1201}}{2})}\right)=$$
$$=\frac{35}{\sqrt{1201}}\left(\ln\left|x-\frac{35+\sqrt{1201}}{2}\right|-\ln\left|x-\frac{35-\sqrt{1201}}{2}\right|\right)+C=$$
$$=\frac{35}{\sqrt{1201}}\left(\ln\left|\frac{2x-35+\sqrt{1201}}{2x-35-\sqrt{1201}}\right|\right)=\frac{35}{\sqrt{1201}}\left(\ln\left|1+\frac{2\sqrt{1201}}{2x-35-\sqrt{1201}}\right|\right)$$
$$\Large+C$$
