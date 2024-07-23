## Task
Let $I=\lambda x,y\in\mathbb R.\int^y_xe^{t^M}dt.$ Find $\frac{dI}{dx}, \frac{dI}{dy}$
## Solution
Let $F(t)$ be [[Antiderivative]] of $e^{t^{35}}$
Then
$$I=\int^y_xe^{t^{35}}dt=F(y)-F(x)$$
$$\frac{dI}{dx}=\frac{d(F(y)-F(x))}{dx}=\frac{d(F(y))}{dx}-\frac{d(F(x))}{dx}=0-e^{x^{35}}=-e^{x^{35}}$$
$$\frac{dI}{dy}=\frac{d(F(y)-F(x))}{dy}=\frac{d(F(y)}{dy}-\frac{d(F(x))}{dx}=e^{y^{35}}-0=e^{y^{35}}$$