---
tags:
  - CompArch
  - Programming
  - Verilog
---
## Example
```Verilog
output reg q
always @ (i1 or o2 or s)
begin
	q = (i1 & ~s) | (i2 & s);
end
```
Update q whenever i1, i2, or s changes
	q **has to be** reg 
	because only "regs" can be modified withing an "always" code block
## Sensitivity List
the thing in parentheses is the sensitivity list of "always" block 
Execute the body of the code block whenever one of the inputs in sensitivity list changes
### wildcard operator (*)
Forces to automatically determine the
dependencies of q, and to update q
whenever some of those input
dependencies changes
``` Verilog
always @ (*)
begin
...
end
```
 	