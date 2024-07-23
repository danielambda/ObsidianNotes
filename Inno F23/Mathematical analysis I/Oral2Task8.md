---
tags:
  - Math
  - MathematicalAnalysis
---
$M = 25 + 10 = 35$

---
## Task
- Indicate which of the following limits does exist and what is the limit in this case? 
- Prove your answer for any two of these limits using any theory covered in the lectures.
1. $\displaystyle\lim_{x\to M}\frac{x^2-(1+\sqrt M)x+\sqrt M)}{x^2-M}$ 
2. $\displaystyle\lim_{x\to \sqrt M}\frac{x^2-(1+\sqrt M)x+\sqrt M)}{x^2-M}$ 
3. $\displaystyle\lim_{x\to +\infty}\frac{x^2-3x+2}{Mx^2-1}$ 
4. $\displaystyle\lim_{x\to 0}(1-Mx)^\frac{2}{x}$  
## Solution 1.
### Answer 1.:
- limit for 1 does exist, and it is equal to 
### Proof 1.:
Since polynomials are [[Continuity|continuous]] everywhere (according to slide 88), our function that is a division of two polynomials is [[Continuity|continuous]] everywhere, except $x^2-M=0$ ([[Arithmetic operations with Continuity|according to slide 84]])
Therefore 
$$\lim_{x\to M}\frac{x^2-(1+\sqrt M)x+\sqrt M)}{x^2-M}=\frac{M^2-(1+\sqrt M)M+\sqrt M)}{M^2-M}$$
$$=\frac{M^2-M-M\sqrt M+\sqrt M}{M^2-M}=\frac{M(M-1)-\sqrt M(M-1)}{M(M-1)}=$$$$=\frac{35(35-1)-\sqrt {35}(35-1)}{35(35-1)}=\frac{35-\sqrt {35}}{35}=1-\frac{1}{\sqrt{35}}$$