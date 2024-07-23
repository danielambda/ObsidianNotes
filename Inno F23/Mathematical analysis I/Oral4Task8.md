## Task
Using [[Definite Integral|integration]] compute the area of the region between [[Hyperbola]]
$x^2-\frac{y^2}{M}=1$ and [[Line]] $x=M$
## Solution
$$x^2-\frac{y^2}{35}=1, x=35$$
![[Pasted image 20231205222019.png]]
## Variant 1:
Let us apply linear transformation with [[Matrix]] $\left[\begin{matrix}1&0\\0&1/35\end{matrix}\right]$
Line stays the same, new Hyperbola: $$x^2-y^2=1$$
![[Pasted image 20231205222815.png]]
Let us find intersection of the hyperbola with the line: $$\begin{cases}x^2-y^2=1\\x=35\end{cases}\implies 1225-y^2=1\implies y=\pm\sqrt{1224}=\pm6\sqrt{34}$$
Let us consider triangle with vertices $(0,0), (35,0), (35, 6\sqrt{34})$
Its area is $\displaystyle\frac{1}{2}35\times6\sqrt{34}=104\sqrt{34}$
Required area is equal to double difference of triangle's area and area between hyperbola and line connecting points $(0,0)$ and $(35,6\sqrt{34})$ in first quadrant (let it be called $\frac t2$)
![[Pasted image 20231205223559.png]]
we know that $\cosh t=35$
$\implies t=\cosh^{-1}35$
Required area: $$2\left(104\sqrt{34}-\frac{\cosh^{-1}35}2\right)=208\sqrt{34}-\cosh^{-1}35$$
We should transform it back, and area will be $35$ times greater.
Answer $7280\sqrt{34}-35\cosh^{-1}35$
- In general:
$\sqrt M(M\sqrt{M^2-1}-\cosh^{-1}M)=\sqrt M(M\sqrt{M^2-1}-\ln(M+\sqrt{M^2-1}))$
## Variant 2
let us define a couple of functions and make some derivations:
$$\cosh x=\frac{e^x+e^{-x}}{2},\sinh x=\frac{e^x-e^{-x}}{2}, \cosh^{-1}x-inverse\;of\cosh x$$
$$(\cosh x)'=\frac{1}{2} (e^x-e^{-x})=\sinh x$$
$$(\cosh x)^2-(\sinh x)^2=\left(\frac{e^x+e^{-x}}{2}\right)^2-\left(\frac{e^x+e^{-x}}{2}\right)^2=\frac{e^{2x}+2+e^{-2x}}{4}-\frac{e^{2x}-2+e^{-2x}}{4}=1$$
$$(\sinh x)^2=(\cosh x)^2-1$$
$$\int\sqrt{x^2-1}dx$$
$x=\cosh t\implies t=sign(x)\cosh^{-1}x$
$dx=\sinh t\,dt$
тут можно ассуме что х больше 1 и все чики пуки должно быть
$$\int\sqrt{x^2-1}dx=\int\sqrt{(\cosh t)^2-1}\sinh t\,dt=t=\int|\sinh t|\sinh t\,dt=$$
$$=sing(\sinh t)\int((\cosh t)^2-1)dt=sign(\sinh t)\left(\int(\cosh t)^2dt-\int dt\right)=$$
$$sign(\sinh t)\left(\sinh t\cosh t-\int(\sinh t)^2dt-t\right)=|\sinh t| \cosh t-\int|\sinh t|\sinh t\,dt-sign(\sinh t)t$$
$$\implies \int|\sinh t|\sinh t\,dt=|\sinh t|\cosh t-\int|\sinh t|\sinh t\,dt-sign(\sinh t)t\implies$$
$$\int|\sinh t|\sinh t\,dt=\frac{|\sinh t|\cosh t-sign(\sinh t)t}{2}+C=\frac{\sqrt{(\cosh t)^2-1}\cosh t-sign(\sinh t)t}{2}+C=$$
$$=\frac{x\sqrt{x^2-1}- sign(x)sign(x)\\cosh^{-1}x}{2}+C=$$
$$\LARGE =\frac{x\sqrt{x^2-1}-\ln(x+\sqrt{x^2-1})}{2}+C$$
