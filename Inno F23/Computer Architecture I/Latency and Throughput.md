---
tags:
  - CompArch
---
## Definitions
- Latency - Response time or Delay
	- A time delay between the cause and the start of the effect
	- But not “[[Execution time]]”, which includes “latency” together with additional timing overheads
		- Example:
			- You request a web page of 1000 bytes (e.g. via HTTP protocol). The first byte arrives in 18 ms, and the last byte - in 713 ms; Latency in this case is 18 ms, but Execution time (to retrieve the entire web page) is 713 ms
	- A precise definition depends on the context
- Throughput - Amount of jobs machine can run at once
## Differences 
![[Pasted image 20231002234949.png]]
## !! 
- Latency and throughput are related . . . sometimes
	- Replacing a processor with a faster one improves both latency and throughput (e.g. due to hyper-threading)
	- Adding a second processor, improves the throughput but NOT the response time
