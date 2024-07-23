---
tags:
  - Programming
---
``` C
enum TrafficLight { red, yellow, green };

TrafficLight trafficLight;

trafficLight = 2; //OK
trafficLight = green; //OK

trafficLight = 436 //NOT an error. this is ok... C, wtf? 
```
