---
tags:
  - Math
  - MathematicalAnalysis
---
## Definition
- A partial derivative of a [[Function]] $f(X):$
$$\frac{\partial f}{\partial x_i}=\lim_{\Delta\to0}\frac{f(x_1,\dots,x_i+\Delta,\dots,x_N)}{\Delta}$$
- The linear part of the [[Function]] change is called *differential*
$$f(X+\Delta X)-f(X)-\sum_{i=1}^N\frac{\partial f}{\partial x_i}\Bigg|_x \Delta x_i+ o(||\Delta X||)$$
$$\implies df=\sum_{i=1}^N\frac{\partial f}{\partial x_i}dx_i$$
## Notation
$$\Large\frac{\partial f}{\partial x}=f_x=\partial _xf$$