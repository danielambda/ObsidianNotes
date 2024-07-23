## Task
Using variable substitution find $\int f(x)dx$ for the following $f(x):$
1. $\frac{M}{M+\sqrt x}$
2. $\frac{M}{1+Me^x}$
## Solution 1.
$$\int\frac{35}{35+\sqrt x}dx$$
$t=\sqrt x, dt=\frac{dx}{2\sqrt x}\implies dx=2\sqrt x dt=2tdt$
$$\int\frac{35}{35+t}2tdt=70\int\frac{35+t-35}{35+t}dt=70\left(\int dt-\int\frac{35}{t+35}dt\right)=$$
$$70\left(t-\int\frac{1}{\frac t{35}+1}dt\right)=70\left(t-35\int\frac{d(\frac{t}{35})}{\frac{t}{35}+1}\right)=$$
$$=70t-2450\ln\left|1+\frac{t}{35}\right|+C=70\sqrt x-2450\ln\left|1+\frac{\sqrt x}{35}\right|\Large+C$$
$$70(\sqrt x-35\ln\left|35+\sqrt x\right|)+C$$
## Solution 2.
$$\int\frac{35}{1+35e^x}dx$$
$t=35e^x, dt=35e^xdx, dx=\frac{dt}{t}$
$$35\int\frac{dt}{t(1+t)}$$
$$\forall t:\frac{1}{t(1+t)}=\frac{A}{t}+\frac{B}{t+1}\implies A=-B$$
$$1=A(t+1)-At\implies A=1\implies B=-1$$
$$35\int\left(\frac{1}{t}-\frac{1}{t+1}\right)dt=35\left(\int\frac{dt}{t}-\int\frac{dt}{t+1}\right)=35(\ln|t|-\ln|t+1|)+C=$$
$$=35(\ln(35e^x)-\ln(35e^x+1))+C=35(\ln35+x-\ln(35e^x+1))+C$$