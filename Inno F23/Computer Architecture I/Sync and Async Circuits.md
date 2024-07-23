---
tags:
  - CompArch
slide: "9.34"
---
| Characteristic                                    | Asynchronous      (like [[Set Reset Latch]])                   | Synchronous       (like [[Flip-Flop]])                             |
| ------------------------------------------------- | -------------------------------------------------- | ----------------------------------------------------- |
| Output Update Trigger                             | Any change of one of the inputs                    | A [[Clock]] signal, together with other input signals |
| [[Clock]] Presence                                | No [[Clock]] present                               | Clock governs the entire circuit activity             |
| Reliability (for result correctness)              | Less reliable                                      | Reliable                                              |
| [[Memory]] Element Presence                       | Might be used or not (it can be [[Memory]] itself) | Used                                                  |
| Operation Speed                                   | Faster                                             | Slower                                                |
| Power Consumption                                 | Less consuming                                     | More consuming                                        |
| Logical Complexity, Size (the number of elements) | Simpler and Smaller                                | More Complex and Larger                                                      |
