## Task
Study whether 
1. $e^M>M^e$
2. $e^{1/M}>(1/M)^e$
3. $(1/e)^M>M^{1/e}$
Your solutions should be self-explanatory and proof-carrying!
## Solution
1. $e^{35}>35^e$ is true:
We know that $e^x=1+x+\frac{x^2}{2!}+\frac{x^3}{3!}+...$ (do we?)
$x^{1/e}$ is a monotonously growing function because $1/e>0$, so
$(e^{35})^{1/e}>(35^e)^{1/e}\implies e^{35}>35^e$
$(35^e)^{1/e}=35$
$(e^{35})^{1/e}=e^{35/e}=1+\frac{35}{e}+\frac{1225}{2e^2}+...>1+\frac{35}{e}+\frac{1225}{2e^2}$
$e<3.5\implies 1+\frac{35}{e}+\frac{1225}{2e^2}>1+10+50=61$
$(e^{35})^{1/e}>61>35=(35^e)^{1/e}\implies e^{35}>35^{e}, Q.E.D.\square$

2. $e^{1/35}>(1/35)^e$ is true:
$1/35>0\implies e^{1/35}>1$
${1/35}<1\;\&\; e>1\implies (1/35)^e<1$
$\implies e^{1/35}>1>(1/35)^e. Q.E.D. \square$

3. $(1/e)^{35}>35^{1/e}$ is false: 
$(1/e)^{35}=1/e^{35}<1$
$1/e > 0\;\&\;35>1\implies 35^{1/e}>1$
$\implies (1/e)^{35}<1<35^{1/e}, Q.E.D.\square$
$\blacksquare$ 