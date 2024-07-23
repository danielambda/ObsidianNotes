$$\Large M=35$$
## Task
Knowing that $\displaystyle\tan x=\frac{\sin x}{\cos x}\;\&\;\cot x=\frac{\cos x}{\sin x}$, prove (using any theory from lecture notes) that $$(\tan(Mx))'=\frac{M}{(\cos(Mx))^2}$$
$$(\cot(M/x))'=\frac{M}{(x\sin(M/x))^2}$$
## Solution
Firstly, let us find [[Derivative]] of $\tan x$
0. $\displaystyle(\tan x)'=\left(\frac{\sin x}{\cos x}\right)'=^0\frac{(\sin x)'\cos x-\sin x(\cos x)'}{\cos^2 x}=$
$=\displaystyle\frac{\cos x\cos x-\sin x(-\sin x)}{\cos^2 x}=\frac{\cos^2x+\sin^2x}{\cos^2x}=\frac{1}{\cos^2x}$
	(0 - [[Arithmetic operations with Derivatives|slide 41]])
1. $\displaystyle(\tan(35x))'=^1(\tan)'(35x)\times(35x)'=\frac{1}{\cos^2(35x)} 35=\frac{35}{\cos^2(35x)}Q.E.D.\square$
	(1 - [[Differentiation of Composition|slide 42]]) 
2. $\displaystyle(\cot(35/x))'=\left(\frac{1}{\tan(35/x)}\right)'=^1\left(\frac{1}{\tan}\right)'(35/x)\times(35/x)'=^2$
$=^2\displaystyle \left(\frac{-\tan'}{\tan^2}\right)(35/x)\times\frac{-35}{x^2}=\left(\frac{\cos^2}{-\cos^2\times \sin^2}\right)(35/x)\times\frac{-35}{x^2}=$
$=\displaystyle\frac{-35}{x^2(-\sin^2(35/x))}=\frac{35}{(x\sin(35/x))^2}, Q.E.D.\square$
	(2 - [[Arithmetic operations with Derivatives|slide 40]])
	$\blacksquare$ 