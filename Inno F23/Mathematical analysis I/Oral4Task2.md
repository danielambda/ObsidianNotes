## Task
Find any [[Antiderivative]]
1. for $\lambda x\in\mathbb R.(x^2-Mx+M)$ that gets value $M$ at point $x=1$
2. All [[Antiderivative]]s for $\displaystyle\lambda x\in]0,2[.\frac{x-2\sqrt x+M}{Mx^2\sqrt[3]x}$ that gets value $1$ at point $x=1$
## Solution 1.
$$\int (x^2-35x+35)dx=\frac{x^3}{3}-\frac{35x^2}{2}+35+C$$
$$\frac1 3-\frac{35}{2}+35+C=35\iff C=\frac{105}{6}-\frac{2}{6}=\frac{103}{6}$$
$$\frac{x^3}{3}-\frac{35x^2}{2}+35+\frac{103}{6}=\frac{2x^3-105x^2+313}{6}$$
Answer: $\frac{2x^3-105x^2+313}{6}$
## Solution 2.
$$\int\frac{x-2\sqrt x+35}{35x^2\sqrt[3]x}dx=\frac{1}{35}\int x^{-\frac{4}{3}}dx-\frac2{35}\int x^{-\frac{11}{6}}dx+\int x^{-\frac{7}{3}}dx=$$
$$=\frac{1}{35}\frac{x^{-\frac{1}{3}}}{-\frac{1}{3}}-\frac{2}{35}\frac{x^{-\frac5 6}}{-\frac{5}{6}}+\frac{x^{-\frac{4}{3}}}{-\frac{4}{3}}=\frac{-3}{35\sqrt[3]x}+\frac{12}{175\sqrt[6]{x^5}}-\frac{3}{4x\sqrt[3]x}+C$$
