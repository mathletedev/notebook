---
tags:
  - e_e_214
created: 2024-11-18
see also:
  - "[[State Machine]]"
---

Mechanical switches will "bounce" when pressed, not ensuring constant contact.

1. Use a clock rate on the magnitude of the debounce rate
2. Ensure $IN$ / $\overline{IN}$ is asserted for at least 2 clock cycles before transitioning state