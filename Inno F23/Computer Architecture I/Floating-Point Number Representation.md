---
tags:
  - CompArch
---
- Representation of floating point number is not unique:
	- $55.66 = 55.66 \times10^0 = 5.566\times10^1=0.5566\times10^2 = ...$
## Example Base 10
- Using numerals with 5 digits of the kind ± .XXX ±EE 
- Mantissa = ± .XXX three signed digits 0.001 ≤ m < 1 
- Exponent = ±EE two signed digits -99 ≤ e ≤ 99 Represented numbers are:
![[Pasted image 20231004151729.png]]
## Standard IEEE 754 (1985)
- Standard definition (i.e., architecture independent)
- Single precision (uses 32 bits to represent sign, exponent and mantissa![[Pasted image 20231004151847.png]]
- Double precision (uses 64 bits)
![[Pasted image 20231004151908.png]]

