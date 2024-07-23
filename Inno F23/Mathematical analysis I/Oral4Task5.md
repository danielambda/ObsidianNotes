## Task 
Using any integration technique find $\int f(x)dx$ for the following $f(x):$
1. $(\sin x)(\cos x)^M$
2. $(\sin(Mx))^2(\cos(Mx))^3$
3. $\frac{1}{(\cos(Mx))^4}$
## Solution 1.
$$\int(\sin x)(\cos x)^{35}dx$$
$t=\cos x,dt=-\sin {x}dx$
$$\int-t^{35}dt=-\frac{t^{36}}{36}+C=\frac{-(\cos x)^{36}}{36}+C$$
## Solution 2.
$$\int(\sin(35x))^2(\cos(35x))^3dx=\int(\sin(35x))^2(\cos(35x))(1-(\sin(35x))^2)dx$$
$t=\sin(35x),dt=35\cos(35x)dx$
$$\frac{1}{35}\int t^2(1-t^2)dt=\frac{1}{35}\left(\int t^2dt-\int t^4dt\right)=$$
$$=\frac{1}{35}\left(\frac{t^3}{3}-\frac{t^5}{5}\right)+C=\frac{5(\sin(35x))^3-3(\sin(35x))^5}{525}+C$$
## Solution 3.
$$\int\frac{dx}{(\cos(35x))^4}=\frac{1}{35}\int\frac{d(35 x)}{(\cos(35x))^4}=$$$$=\frac{1}{35}\int\frac{(\cos(35x))^2+(\sin(35x))^2}{(\cos(35x))^4}d(35x)=\frac1{35}\left(\int\frac{(\cos(35x))^2}{(\cos(35x))^4}d(35x)+\int\frac{(\sin(35x))^2}{(\cos(35x))^4}d(35x)\right)=$$
$$=\frac{1}{35}\left(\int\frac{d(35x)}{(\cos(35x))^2}+\int(\tan(35x))^2\frac{d(35x)}{(\cos(35x))^2}\right)$$
$t=\tan(35x),dt=\frac{d(35x)}{(\cos(35x))^2}$
$$\frac{1}{35}\left(\tan(35x)+\int t^2dt\right)=\frac{1}{35}\left(\tan(35x)+\frac{t^3}{3}\right)+C=\frac{3\tan(35x)+(\tan(35x))^3}{105}$$