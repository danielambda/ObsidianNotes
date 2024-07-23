---
tags:
  - Math
  - MathematicalAnalysis
---
## Theorem
- Consider the [[Numeric Series]] $$S=\sum^\infty_{n=0}(-1)^nu_n$$
where $0<u_{n+1}<u_n, u_n\to0$ as $n\to\infty$ and both $$\displaystyle s_+=\sum^\infty_{n=0}u_{2n}, s_-=\sum^\infty_{n=0}u_{2n+1}$$ diverge
- Then one can rearrange the series in such a wayввв that the sum might be any real number
## Proof
- Take a positive number $A, k_1$ and $l_1$ such that
	$$s_1=u_0+u_2+...+u_{2k_1}>A$$$$u_0+u_2+...+u_{2k_1-2}<A$$$$s_2=u_0+u_2+...+u_{2k_1}-u_1-u_3-...-u_{2l_1+1}<A$$$$u_0+u_2+...+u_{2k_1-2}-u_1-u_3-...-u_{2l_1-1}>A$$
- Further: $$s_3=\sum^{k_1}_{n=0}u_{2n}-\sum^{l_1}_{n=0}u_{2n+1}+\sum^{k_2}_{n=k_1+1}u_{2n}>A$$ $$s_4=\sum^{k_1}_{n=0}u_{2n}-\sum^{l_1}_{n=0}u_{2n+1}+\sum^{k_2}_{n=k_1+1}u_{2n}-\sum^{l_2}_{n=l_1+1}<A$$ $$s_5=...>A, s_6=...< A$$
---
$$\lim_{n\to\infty} u_n=0\implies \lim_{n\to\infty} s_n = A$$