---
tags:
  - Math
  - MathematicalAnalysis
  - DifferetialForms
---
Let $\displaystyle\Sigma=\sum_i n_i\sigma_i$ be an [[m-Chain]] and $\omega$ be a [[Differential m-Form]]
- Then $$\int_\Sigma\omega=\sum_i n_i\int_{\sigma_i}\omega$$
## Examples
- Given 
	- differential 0-form $f(x,y)=3x+xy^2$
	- [[m-Cell|0-Cells]] $p=(0,3), q=(5,2)$
	- 0-Chain $\Sigma=2p-q$
	$$\int_{\Sigma}f=2\int_pf-\int_qf=2f(p)-f(q)=2f(0,3)-f(5,2)=0-35=-35$$
- Given 
	- differential 1-form $\omega=xy\,dx+(x^2+y)dy$
	- 1-Cells
![[Pasted image 20240511175135.png]]
- 1-Chain $\Sigma=2\sigma_2-3\sigma_2$
$$\sigma_1(t)=\langle\cos(\pi - t),\sin(\pi-t)\rangle, t\in[0,\pi]$$
$$\sigma_2(t)=\langle t,t-1\rangle, t\in[1,2]$$
$$\int_\Sigma\omega=2\int_{\sigma_1}(xy\,dx+(x^2+y)dy)-3\int_{\sigma_2}(xy\,dx+(x^2+y)dy)=$$
$$=2\int_{\sigma_1}\left(xy\,\frac{dx\,dt}{dt}+(x^2+y)\frac{dy\,dt}{dt}\right)-3\int_{\sigma_2}\left(xy\,\frac{dx\,dt}{dt}+(x^2+y)\frac{dy\,dt}{dt}\right)=$$
$$=2\int_{0}^\pi[\cos(\pi-t)\sin(\pi-t)\sin t+(\cos^2(\pi-t)+\sin(\pi-t))(-\cos t)]dt-$$$$-3\int_1^2((t^2-t)+(t^2+t-1))dt=$$