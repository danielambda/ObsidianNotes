---
tags:
  - Math
  - DiscreteMath
---
## Definition
- Let $a_{n+k} = t_1a_{n+k-1} +...+t_ka_n$ be a [[Linear Recurrence Sequence]]. That is $a_{n+k} - t_1a_{n+k-1} -...-t_ka_n=0$. Then the *character* of it is $$\chi(\lambda) = \lambda^k-t_1\lambda^{k-1}-t_2\lambda^{k-2}-...-t_{k-1}\lambda^1-t_k\lambda^0$$$$\chi(\lambda) = \lambda^k-\sum^k_{i=1}t_i\lambda^{k-i}$$
## Example
$$a_{n+2} = a_{n+1}+a_n$$
$$a_{n+2}-a_{n-1}-a_n = 0$$
$$\chi(\lambda) = \lambda^2-\lambda - 1$$
## Lemma
Let $a_{n+k} = t_1a_{n+k-1} +...+t_ka_n$ be a [[Linear Recurrence Sequence]], $\chi(\lambda)$ be its character, and $p$ be a root of $\chi(\lambda)$. Then the sequence $$1,p,p^2,...,p^n,...$$ is its solution.
## Proof 
Since $p$ is a root of $\chi, \chi(p) = 0 \implies$
$\displaystyle p^{n+k}-\sum^k_{i=1}t_ip^{n+k-i} =p^n\left(p^k-\sum^k_{i=1}t_ip^{k-i}\right)=p^n\chi(p)=0$
Therefore, $\displaystyle p^{n+k} = \sum^k_{i=1}t_ip^{n+k-i}$, that is, $p^n$ is a solution of a given [[Linear Recurrence Sequence]] by definition.
## Example 
$a_{n+2} = a_{n+1}+a_n, \chi(\lambda) = \lambda^2-\lambda-1$
$\displaystyle p_1 =\frac{1+\sqrt 5}{2}, p_2 =\frac{1-\sqrt5}{2}$
1. $\displaystyle 1, \frac{1+\sqrt5}{2}, \left(\frac{1+\sqrt5}{2}\right)^2, \left(\frac{1+\sqrt5}{2}\right)^3$
2. $\displaystyle 1, \frac{1-\sqrt5}{2}, \left(\frac{1-\sqrt5}{2}\right)^2, \left(\frac{1-\sqrt5}{2}\right)^3$
## Lemma
If both $x_0, x_1, x_2,...$ and $y_0, y_1, y_2, ...$ are [[Solution of a Linear Recurrence sequence|solutions of a Linear Recurrence sequence]], then $$\alpha x_0+\beta y_0, \alpha x_1+\beta y_1, \alpha x_2+\beta y_2, ...$$
is also a [[Solution of a Linear Recurrence sequence]]
		well, this is actually obvious