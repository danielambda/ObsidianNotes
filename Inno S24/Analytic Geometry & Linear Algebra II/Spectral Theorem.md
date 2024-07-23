---
tags:
  - Math
  - AGLA
  - ComplexAnalysis
---
## Theorem
- For given [[Matrix]] $A$: $$A=A^H\implies$$$$1.\;\forall \lambda\in\text{eighenvalues}(A): \lambda\in\mathbb R$$
$$2. \forall\lambda_i,\lambda_j\in\text{eighenvalues}(A):\lambda_i\not=\lambda_j\implies v_i\perp v_j$$
## Proof
$$1.\;Av=\lambda x\implies \overline A\overline x=\overline \lambda\overline x\implies \left(\overline A\overline v\right)^\intercal=\left(\overline \lambda\overline v\right)^\intercal\implies x^H A^H=\overline \lambda x^H\implies$$
$$\implies v^H A v=\overline\lambda v^Hv\implies\lambda v^Hv=\overline\lambda v^Hv\implies\lambda=\overline\lambda\implies$$
$$\implies \Large\lambda\in\mathbb R$$
$$2.\; Ax_1=\lambda_1 x_1, Ax_2=\lambda_2 x_2\;\square$$
$$\text{Consider } \lambda_1 x_1^Hx_2=(\lambda_1x_1)^H x_2=(Ax_1)^Hx_2=x_1^HA^Hx_2=x_1^HAx_2=x_1^H\lambda_2x_2\implies$$
$$\implies \lambda_1x_1^Hx_2=\lambda_2x_1^Hx_2$$
$$\text{Since } \lambda_1\not=\lambda_2\implies x_1^Hx_2=0\implies x_1\perp x_2\;\square\blacksquare$$