---
tags:
  - e_e_214
created: 2024-10-23
---

In truth table form:

| PS3 | PS2 | PS1 | PS0 | NS3 | NS2 | NS1 | NS0 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| 0   | 0   | 0   | 0   | 0   | 0   | 0   | 1   |
| 0   | 0   | 0   | 1   | 0   | 0   | 1   | 0   |
| 0   | 0   | 1   | 0   | 0   | 0   | 1   | 1   |
| ... |     |     |     |     |     |     |     |
| 1   | 1   | 1   | 1   | 0   | 0   | 0   | 0   |

Then we feed the output of the register back into itself.

Another design:

![[Binary Counter 2024-10-23 09.31.28.excalidraw]]

**Asynchronous counter**: Not connected to "Autobahn" clock network; fast but skewed.