## Task
Evaluate the following improper integrals:
1. $\int^{+\infty}_0 e^{-Mx}dx$
2. $\int^{\sqrt M}_0\frac{dx}{\sqrt{M-x^2}}$
3. $\int^{+\infty}_0\frac{dx}{x^2+Mx+1}$
## Solution 1.
$$\int^{+\infty}_0e^{-35x}dx=\lim_{t\to+\infty}\left(\int^t_0e^{-35x}dx\right)=\frac{-1}{35}\lim_{t\to+\infty}\left(\int^t_0-35e^{-35x}dx\right)=^-$$

---
$$\int -35e^{-35x}dx=\int e^{-35x}d(-35x)=e^{-35x}\LARGE +C$$

---
$$^-=\frac{-1}{35}\lim_{t\to+\infty}\left(e^{-35x}\bigg|_0^t\right)=\frac{-1}{35}\lim_{t-\to+\infty}\left(e^{-35t}-e^{-35\times0}\right)=\frac{-1}{35}\left(0-1\right)=\large\frac{1}{35}$$
## Solution 2.
$$\int_0^{\sqrt {35}}\frac{dx}{\sqrt{35-x^2}}=\lim_{t\to\sqrt{35}}\left(\int^t_0\frac{dx}{\sqrt{35}\sqrt{1-\frac{x^2}{35}}}\right)=^-$$

---
$$\int\frac{dx}{\sqrt{35}\sqrt{1-\frac{x^2}{35}}}=\int\frac{d\left(\frac{x}{\sqrt{35}}\right)}{\sqrt{1-\left(\frac{x}{\sqrt35}\right)^2}}=\sin^{-1}\left(\frac{x}{\sqrt{35}}\right)\LARGE+C$$

---
$$^-=\lim_{t\to\sqrt{35}}\left(\sin^{-1}\left(\frac{x}{\sqrt{35}}\right)\bigg|_0^t\right)=\lim_{t\to\sqrt{35}}\left(\sin^{-1}\left(\frac{t}{\sqrt{35}}\right)-\sin^{-1}\left(\frac{0}{\sqrt{35}}\right)\right)=\sin^{-1}1=\large\frac{\pi}{2}$$
## Solution 3.
$$\int^{+\infty}_0\frac{dx}{x^2+35x+1}=\lim_{t\to+\infty}\left(\int_0^t\frac{dx}{x^2+35x+1}\right)=\lim_{t\to+\infty}\left(\int_0^t\frac{dx}{\left(x+\frac{35}2\right)^2-\frac{1221}{4}}\right)=^-$$

---
$$\int\frac{dx}{(x+\frac{35}{2})^2-\frac{1221}{4}}=\frac{4}{1221}\int\frac{d(x+\frac{35}2)}{\left(\frac{x+\frac{35}{2}}{\sqrt{\frac{1221}{4}}}\right)^2-1}=\sqrt\frac{4}{1221}\int\frac{d\left(\frac{x+\frac{35}{2}}{\sqrt{\frac{1221}{4}}}\right)}{\left(\frac{x+\frac{35}{2}}{\sqrt\frac{1221}{4}}\right)^2-1}=$$
$$=\sqrt\frac{4}{1221}\int\frac{d\left(\frac{x+\frac{35}{2}}{\sqrt{\frac{1221}{4}}}\right)}{\left(\frac{x+\frac{35}{2}}{\sqrt\frac{1221}{4}}-1\right)\left(\frac{x+\frac{35}{2}}{\sqrt\frac{1221}{4}}+1\right)}=$$$$=\sqrt\frac{4}{1221}\int\left(\frac{\frac12}{\left(\frac{x+\frac{35}{2}}{\sqrt\frac{1221}{4}}-1\right)}-\frac{\frac12}{\left(\frac{x+\frac{35}{2}}{\sqrt\frac{1221}{4}}+1\right)}\right)d\left(\frac{x+\frac{35}{2}}{\sqrt{\frac{1221}{4}}}\right)=$$
$$\large=\sqrt\frac{1}{1221}\left(\ln\left|\frac{\frac{x+\frac{35}{2}}{\sqrt\frac{1221}{4}}-1}{\frac{x+\frac{35}{2}}{\sqrt\frac{1221}{4}}+1}\right|\right)+C=\sqrt\frac{1}{1221}\ln\left|\frac{2x+35-\sqrt{1221}}{2x+{35}+\sqrt{1221}}\right|+C$$
---
$$^-=\sqrt{\frac{1}{1221}}\lim_{t\to+\infty}\left(\ln\left|\frac{2x+35-\sqrt{1221}}{2x+35+\sqrt{1221}}\right|\bigg|_0^t\right)=$$$$=\sqrt\frac{1}{1221}\lim_{t\to+\infty}\left(\ln\left|\frac{2t+35-\sqrt{1221}}{2t+35+\sqrt{1221}}\right|-\ln\left|\frac{0+35-\sqrt{1221}}{0+35+\sqrt{1221}}\right|\right)=$$
$$=\sqrt\frac{1}{1221}\left(\lim_{t\to+\infty}\left(\ln\left|1+\frac{-2\sqrt{1221}}{2t+35+\sqrt{1221}}\right|\right)-\lim_{t\to+\infty}\left(\ln\left|\frac{35-\sqrt{1221}}{35+\sqrt{1221}}\right|\right)\right)=$$
$$\large=\sqrt\frac{1}{1221}\left(\ln\left|1\right|-\ln\left|\frac{35-\sqrt{1221}}{35+\sqrt{1221}}\right|\right)=-\sqrt\frac{1}{1221}\ln\left|\frac{35-\sqrt{1221}}{35+\sqrt{1221}}\right|=$$
$$\LARGE=\frac{\ln\left|\frac{35+\sqrt{1221}}{35-\sqrt{1221}}\right|}{\sqrt{1221}}$$