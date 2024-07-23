---
tags:
  - CompArch
  - Programming
---
## Definition
- **Verilog** is a Hardware description (design) language
- Verilog provides built-in primitive hardware modules (not, and, or, etc.)
## Examples
Consider 2-to-1 [[Multiplexer]].
![[Pasted image 20231017190814.png]]
``` verilog
module mux(i1, i2, s, q); //list of pins
	input i1, i2, s; //specification 
	output q;        //of pin purposes

	wire q0, q1, q2; //inroducing wires

	not(q0, s); //wire q0 gets inverted value of s
	and(q1, i1, q0); //wire q1 gets...
	and(q2, i2, s); //wire q2 gets...
	or(q, q1, q2);
endmodule
```
## Operators

| Symbol | Function         | Operands |
| ------ | ---------------- | -------- |
| ~      | Bitwise negation | Unary    |
| &      | Bitwise AND      | Binary   |
| \|     | Bitwise OR       | Binary   |
| ^      | Bitwise XOR      | Binary   |
| ^~     | Bitwise XNOR     | Binary   |
| ?:     | Conditional      | Ternary         |
## Continuous Assignment
``` Verilog
assign q1 = (i1 & q0)
```
Whenever some input is changed, output q1 is updated as well
## [[Always @ in Verilog]]
## [[Blocking and Non-Blocking Assignments in Verilog]]
## [[If-Else Statement in Verilog]]
## [[Case Statement in Verilog]]
