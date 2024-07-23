---
tags:
  - CompArch
  - Programming
  - Verilog
---
## Example
``` Verilog
module mux (i1, i2, s, q);
	input i1, i2, s;
	output reg q;
	always @ (*)
	begin
		if (s == 0)	begin 
			q <= i1; 
		end
		else if (s == 1) begin 
			q <= i2;
		end
	end
endmodule
```
also can be written as
``` Verilog
module mux (i1, i2, s, q);
	input i1, i2, s;
	output reg q;
	always @ (*)
	begin
		if (s == 0)	q <= i1; 
		else if (s == 1) q <= i2;
	end
endmodule
```