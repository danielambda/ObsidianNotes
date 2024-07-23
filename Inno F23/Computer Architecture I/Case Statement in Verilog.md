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
		case (s) 
			0: q <= i1; 
			1: q <= i2;
		endcase 
	end
endmodule
```