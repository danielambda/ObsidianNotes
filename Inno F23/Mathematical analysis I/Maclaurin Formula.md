---
tags:
  - Math
  - MathematicalAnalysis
a.k.a.: Taylor Series or Taylor Expansion
slide: "3.71"
---
## Definition
- Let $n\in\mathbb N, f\in C^n (U(0))$
$M_{n,f}(x)=T_{n,f,0}=\displaystyle\sum_{k=0}^n \frac{f^{(k)}(0)}{k!} x^k$ is its Maclaurin Formula of degree $n$
## Then 
- function $(f-M_{n,f})$ is an [[Infinitesimal]] of order $n$ at the origin:
$$\lim_{x\to d}\frac{f(x)-M_{n,f}(x)}{x^n}=0$$
- Let $n\in\mathbb N; a,b\in\mathbb R;f\in C^{n+1}]a,b[; d\in]a,b[;T_{n,f,d}(x)$
- Then $\forall x\in]a,b[\exists c \in[d,x]:$ 
$$f(x)=\left(\sum_{k=0}^n\frac{f^{(k)}(d)}{k!}(x-d)^k\right)+\left(\frac{f^{(n+1)}(c)}{n+1}(x-d)^{n+1}\right)$$ $\implies$ the remainder of residual term of the Taylor approximation is 
$$\frac{f^{(n+1)}(c)}{(n+1)!}(x-d)^{n+1}$$
## Example
- ### Task
	- Approximate $f(x)=\sin x$ by Maclaurin formula of third degree and estimate the truncation error
- ### Solution
	- $\forall x\in\mathbb R;c\in[d,x]:$
$$\sin x=f(0)+f'(0)x+\frac{f(0)''}{2}x^2+\frac{f'''(0)}{6}x^3+\frac{f''''(c)}{24}x^4=$$
$$=\sin0+(\cos0)x+\frac{-\sin0}{2}x^2+\frac{-\cos0}{6}x^3+\frac{\sin(c)}{24}x^4=x-\frac{x^3}{6}+\frac{\cos(c)}{24}x^4$$