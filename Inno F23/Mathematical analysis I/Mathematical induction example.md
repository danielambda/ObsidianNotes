___
Tags:
#Math  ^k13yiQOP
___
## Theorem:
For all $n \in \mathbb{N}, n(n + 1)(n + 5)$ is divisible by 3 
## Proof:
Inducting by $n \in \mathbb{N}$
## Induction base:
Let $n = 0$: 
$0(0 + 1)(0 + 5) = 0$ is divisible by 3 - OK
## Induction hypothesis: 
Assume that $\forall k \in \mathbb{N}$ $k(k +1)(k + 5)$ is divisible by 3

## Induction step:
Prove that $(k + 1)((k + 1) + 1)((k + 1) + 5)$ is divisible by 3:$$(k + 1)((k + 1) + 1)((k + 1) + 5) = (k + 1)(k + 2)(k + 6) = $$ $$ = k^3 + 9k^2 + 20k + 12 = k(k^2 + 9k + 20) + 12 = k(k + 4)(k + 5) + 12 =$$ $$ = k(k + 1 + 3)(k + 4) + 12 = 3(k(k + 4)) + k(k + 1)(k + 5) + 12 =$$$$ = 3(k(k + 4) + 4) + k(k + 1)(k + 4)$$
Which is divisible by 3. Q.E.D. $\blacksquare$
