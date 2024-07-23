---
tags:
  - Math
  - DiscreteMath
---
## Theorem
Let $a_{n+2} = t_1a_{n+1}+t_2a_n\;\&\;t_1^2+t_2^2\not=0\;\&\;\chi(p_1)=\chi(p_2)=0\implies$
1. $p_1\not=p_2\implies x_n=\alpha p_1^n+\beta p_2^n$ is a [[Solution of a Linear Recurrence sequence]]
2. $p_1=p_2\implies x_n=(\alpha n+\beta)p_1^n$ is a [[Solution of a Linear Recurrence sequence]]
## Example
$a_{n+2} = a_{n+1}+a_n, \chi(\lambda) = \lambda^2-\lambda-1$
$\displaystyle p_1 =\frac{1+\sqrt 5}{2}, p_2 =\frac{1-\sqrt5}{2}$
$$\large a_n=\alpha\left(\frac{1+\sqrt5}{2}\right)^n+\beta\left(\frac{1-\sqrt5}{2}\right)^n$$
## Proof
1. $p_1\not=p_2$
	From the [[Character of Linear recurrence sequence|lemma]] it follows that
		$x_n=\alpha p_1^n+\beta p_2^n$ is a solution
	Let $\{x_0, x_1, x_2, ...\}$ be any solution. The solution is defined by $x_0, x_1$, where 
	$$\begin{cases} \alpha p_1^0 + \beta p_2^0 = x_0\\ \alpha p_1^1+\beta p_2^1 = x_1\end{cases}$$
	$\displaystyle\alpha = \frac{x_0p_2-x_1}{p_2-p_1}, \beta=\frac{x_1-p_1x_0}{p_2-p_1}$
2. $p_1=p_2=p, \chi(\lambda)=\lambda^2-t_1\lambda-t_2=(\lambda-p)^2 = \lambda^2-2p\lambda+p^2$ $$\implies \begin{cases}t_1=2p\\ t_2=-p^2\end{cases}$$
Show that $np^n$ is a solution:
- $t_1a_{n+1}+t_2a_n=2p(n+1)p^{n+1}-p^2np^n=$
$=2(n+1)p^{n+2}-np^{n+2}=(n+2)p^{n+2}=a_{n+2}$
Let $p_1=p_2=p$ and $\{x_0, x_1, x_2, ...\}$ be any solution. The solution. The solution is defined by $x_0, x_1$, where $$\begin{cases}(\alpha0+\beta)p^0=x_0\\ (\alpha1+\beta)p^1=x_1\end{cases}$$
$\displaystyle\alpha = \frac{x_1-px_0}{p}, \beta=x_0$

## Algorithm
$a_{n+2} = t_1a_{n+1}+t_2a_n$ is a given [[Linear Recurrence Sequence]]
1. Find the [[Character of Linear recurrence sequence]] (replacing $a_{n+1}\to\lambda^i$) $$\chi(\lambda)=\lambda^2-t_1\lambda-t_2$$
2. Find the roots: $p_1, p_2$
3. Two cases:
	1. If $p_1\not=p_2 \implies a_n=c_1p_1^n+c_2p_2^n$
	2. If $p_1=p_2 \implies a_n=(c_1n+c_2)p^n$
4. Using $a_0, a_1$ find $c_0, c_1$:
	$$\begin{cases}a_0=c_1+c_2\\ a_1=c_1p_1+c_2p_2\end{cases}\;or\;\begin{cases}a_0=c_2\\a_1=(c_1+c_2)p \end{cases}$$
