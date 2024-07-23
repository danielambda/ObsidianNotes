## Task
The first example (in the lecture notes) illustrating origins and applications of the derivatives is about tangent line. The example uses infinitesimal values (numbers). Are the infinitesimal values valid “citizens (with full rights)” or contradictory objects in our course “Mathematical Analysis”? Explain (prove) your answer!
![[Pasted image 20231111190703.png]]

## Answer
In our course of Mathematical Analysis we use [[Tarski's Axiomatization]] for the set of real numbers. Therefore, we know that [[All Reals are Ceiled by Naturals]]:
$$\forall x\in\mathbb R\;\exists a:|x|<a$$
Let us assume existing of infinitesimal value:
$$\exists\varepsilon\in\mathbb R:\forall x\in\mathbb R:0<\varepsilon < |x|$$
$$0<\varepsilon < |x|\iff\frac{1}{\varepsilon}>\frac{1}{|x|}$$
$$\frac 1{|x|}\in\mathbb R\implies\exists a: \left|\frac{1}{|x|}\right|<a$$
дальше мне лень, конец