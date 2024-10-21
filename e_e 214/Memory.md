---
tags:
  - e_e_214
created: 2024-10-16
---

![[Memory 2024-10-16 09.20.07.excalidraw]]

Problem with capacitors: We need to constantly refresh, or the charge is lost.

Flip-flops are driven by the *rising edge* of the clock.

**Skew**: The time it takes for a clock signal to travel between registers.

**PIPO**: Parallel in, parallel out - N bits in, N bits out.
**SIPO**: Serial in, parallel out - 1 bit in, N bits out (by shifting a 1 on each clock pulse).
**SISO**: Serial in, serial out - 1 bit in, 1 bit out.
**PISO**: Parallel in, serial out - N bits in, 1 bit out.

Universal register:

![[Memory 2024-10-21 09.36.50.excalidraw]]

## Metastability

**Metastable**: When an output is "balanced" on an energy barrier.

Every flip-flop can enter a metastable state - the chance is very low, but not 0.

To reduce the risk, we can just chain multiple flip-flops together.