---
tags:
  - CompArch
  - Programming
  - Verilog
  - Java
---
## Blocking
``` Verilog
always @ (*)
begin
	q = (i1 & ~s) | (i2 & s);
	q1 = (i1 & ~s) & (i2 & s);
end
```
q =.., q1 =... are "Blocking" assignment statements:
- First, line 6 is executed;
- After completing q =.., q1 =.. is executed
## Non-Blocking
```
always @ (*)
begin
	q <= (i1 & ~s) | (i2 & s);
	q1 <= (i1 & ~s) & (i2 & s);
end
```
q <=.., q1 <=... are "Non-Blocking" assignment statements:
	they execute concurrently