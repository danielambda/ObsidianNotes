---
tags:
  - Math
  - MathematicalAnalysis
---
- Let us consider the iterated limits as $||x||\to0$
$$\lim_{x_1\to0}\lim_{x_2\to0}\frac{x_1}{x_1+x_2}=\lim_{x_1\to0}\frac {x_1}{x_1}=1$$

$$\lim_{x_2\to0}\lim_{x_1\to0}\frac{x_1}{x_1+x_2}=\lim_{x_2\to0}0=0$$

$$\lim_{r\to0}\frac{x_1}{x_1+x_2}=\lim_{r\to0}\frac{r\cos(\theta)}{r\cos(\theta)+r\sin(\theta)}=\frac{\cos(\theta)}{\cos(\theta)+\sin(\theta)}$$
- One can see both iterated limits exist but they are different and a limit as $||x|| \to 0$ does not exists. 
- This examples show that the changing of the iterated limits can change the answer. 
- The question is: When can be changed the iterated limits?
## Theorem
$$\exists\lim_{X\to0}=A\;\&\;\forall x_2\in\mathbb R_{\setminus\set0}\;\exists\lim_{x_1\to0}f(x_1,x_2)=f(0,x_2)$$$\implies$
$$\lim_{x_1\to0}\lim_{x_2\to0}f(x_1,x_2)=\lim_{x_2\to0}\lim_{x_1\to0}f(x_1,x_2)=A$$
## Proof 
$$||X||<\delta_\varepsilon\implies|f(x_1,x_2)-A|<\varepsilon\implies|f(x_1,0)-A|<\varepsilon\implies \lim_{x_1\to0}=A\implies$$
$$\implies \lim_{x_{1}\to0}\lim_{x_2\to0}f(x_1,x_2)=A$$