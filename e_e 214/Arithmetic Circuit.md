---
tags:
  - e_e_214
created: 2024-10-28
---

Use **divide and conquer** strategy: Instead of dealing with `N` bits all at once, do individual calculations on pairs of bits (as well as a carry-in bit).

![[Arithmetic Circuit 2024-10-28 09.53.47.excalidraw]]

After truth tables and [[Karnaugh Map|K-maps]]:

$S \Leftarrow A \oplus B \oplus Cin$
$Cout \Leftarrow A \oplus B \oplus Cin$

**Ripple-Carry Adder (RCA)**: The above circuit, requires lots of time for calculations.
**Carry-Propagate-Generate Network (CGPN)**: Allows for minimal delay between carrying bits.