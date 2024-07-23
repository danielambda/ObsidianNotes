---
tags:
  - Math
  - Logic
---
## Definitions
- $\forall x\, P(x) \equiv P(x_1)\;\&\;P(x_2)\;\&\;P(x_3)\;\&...\&P(x_n)$
- $\exists x\, P(x) \equiv P(x_1)\lor P(x_2)\lor P(x_3)\lor ...\lor P(x_n)$
- $\exists$
## Properties
- [[De Morgan's Laws]]
- $\forall x\,(P_1(x)\;\&\;P(x_2))\equiv\forall x\, P_1(x)\;\&\;\forall x\,P_2(x)$ 
- $\exists x\,(P_1(x)\lor P(x_2))\equiv\exists x\, P_1(x)\lor\exists x\,P_2(x)$ 
## [[Nested Quantifiers]]
## [[Uniqueness quantifier]]

## Translating to English
- $\neg\exists x\,P(x)$ - there is no person who likes orange
- $\forall x\,\neg R(x)$ -all people does not know C++
- $\forall x(P(x)\implies R(x))$ - if a person likes orange than he knows C++
- $\forall x(P(x)\;\&\;R(x))$ - everybody like orange and know C++
- $\exists x(P(x)\lor R(x))$ - there is a person, who likes oranges or knows C++ $\exists x (P(x)\;\&\;R(x))$ - there is a person, who likes oranges and knows C++
## Exercise 2
- $\exists x(x^3 = -1)$ - there is a real number which cubed is equal to -1 - $true$
- $\forall x(x=-x)$ - for any $x$ it is equal to $-x$ - $false$
- $\exists x\,\forall y(x>y)$ - there is a real number $x$ that is greater than any real number $y$ - $false$
- $\forall x\,\exists y(x+y=0)$ - for any real number $x$ there is a real number $y$ such that $x + y = 0$ - $true$ 
### DNF of Ex2:
$T = (1001)$ 
DNF - $(\neg x \lor\neg y)\;\&\;(x\lor y)$
## Getting rid of negations
- $\neg\forall x((x>0)\lor(x<0))\equiv\exists x((x \leq 0)\;\&\;(x\geq0))\equiv true$ for the domain of $\mathbb R$
- $\neg\exists x\,\exists y\,P(x, y)\equiv\forall x\,\forall y\,\neg P(x, y)$
- $\neg\forall x\,\exists y((x\geq0)\;\&\;(y<0)) \equiv\exists x\,\forall y((x < 0)\lor(y\geq0))$
- $\neg\exists y(R(y)\;\&\;\forall x\,\neg P(x, y))\equiv\forall y(\neg R(y)\lor\exists x\,P(x,y))$
- $\neg\exists y\,(\exists x\,S(x,y)\lor\forall y\,T(x,y))\equiv\forall y\,(\forall x\,\neg S(x,y)\;\&\;\exists y\,\neg T(x,y))$