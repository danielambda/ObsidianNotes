---
tags:
  - Math
  - MathematicalAnalysis
slide: 3.37-3.40
---
## Statement (+, -)
Let $f, g: D\to\mathbb R$ be functions [[Derivative|differentiable]] at some point $d \in D$. 
Then $(f+g)=\lambda x\in D.(f(x)+g(x)), (f-g)=\lambda x\in D.(f(x)-g(x))$ are [[Derivative|differentiable]] at point $d$
$$(f+g)'(d)=f'(d)+g'(d), (f-g)'(d)=f'(d)-g'(d)$$
## Proof (+, -)
$\displaystyle\lim_{\Delta\to0}\frac{(f+g)(d+\Delta)-(f+g)(d)}{\Delta}=\lim_{\Delta\to0}\frac{(f(d+\Delta)+g(d+\Delta))-(f(d)+g(d))}{\Delta}=$
$\displaystyle=\lim_{\Delta\to0}\frac{f(d+\Delta-f(d))}{\Delta}+\lim_{\Delta\to0}\frac{g(d+\Delta-g(d))}{\Delta}=$ $$=f'(d)+g'(d), Q.E.D.\blacksquare$$
---
## Statement (x)
Let $f, g: D\to\mathbb R$ be functions [[Derivative|differentiable]] at some point $d \in D$. 
Then $(f\times g)=\lambda x\in D.(f(x)\times g(x))$ is [[Derivative|differentiable]] at point $d$
$$(f\times g)'(d)=f'(d)g(d)+f(d)g'(d)$$
## Proof (x)
$\displaystyle\lim_{\Delta\to0}\frac{(f\times g)(d+\Delta)-(f\times g)(d)}{\Delta}=\lim_{\Delta\to0}\frac{(f(d+\Delta)g(d+\Delta))-(f(d)g(d))}{\Delta}=$
$=\displaystyle\lim_{\Delta\to0}\frac{(f(d+\Delta)g(d+\Delta)-f(d)g(d+\Delta)+f(d)g(d+\Delta)-f(d)g(d))}{\Delta}=$
$=\displaystyle\lim_{\Delta\to0}\left(\frac{f(d+\Delta)-f(d)}{\Delta}\times g(d+\Delta)\right)+\lim_{\Delta\to0}\left(f(d)\times\frac{g(d+\Delta)-g(d)}{\Delta}\right)=$$=\displaystyle\lim_{\Delta\to0}\frac{f(d+\Delta)-f(d)}{\Delta}\lim_{\Delta\to0}g(d+\Delta)+f(d)\lim_{\Delta\to0}\frac{g(d+\Delta)-g(d)}{\Delta}=$$$=f'(d)g(d)+f(d)g'(d), Q.E.D. \blacksquare$$
---
## Statement (1/)
Let $f: D\to\mathbb R$ be function [[Derivative|differentiable]] at some point $d \in D$. 
Then $(1/f)=\lambda x\in D.(1/f(x)$ is [[Derivative|differentiable]] at point $d$
$$\displaystyle(1/f)'(d)=-\frac{f'(d)}{(f(d))^2}$$
## Proof (1/)
$\displaystyle\lim_{\Delta\to0}\frac{(1/f)(d+\Delta)-(1/f)(d)}{\Delta}=\lim_{\Delta\to0}\frac{\frac{1}{f(d+\Delta)}-\frac{1}{f(d)}}{\Delta}=$
$=\displaystyle\lim_{\Delta\to0}\frac{f(d)-f(d+\Delta)}{\Delta f(d)f(d+\Delta)}=\left(\lim_{\Delta\to0}\frac{f(d)-f(d+\Delta)}{\Delta}\right)\times\left(\lim_{\Delta\to0}\frac{1}{f(d)f(d+\Delta)}\right)=$$$-\frac{f'(d)}{(f(d))^2}, Q.E.D. \blacksquare$$