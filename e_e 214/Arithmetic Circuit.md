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

## Full Adder

![Full Adder](https://www.elprocus.com/wp-content/uploads/Full-Adder-Logical-Diagram.png)

## Subtraction

We use **two's complement** to represent negative numbers:
`00000000` = 0
`00000001` = 1
`11111111` = -1
`11111110` = -2
etc.

To obtain the negative of a number, we can invert the bits and add 1:
3 -> `00000011` -> `11111100` -> `11111101` -> -3

## Comparator

### Equality

`XNOR` each pair of bits, then `AND` the results.

### Greater Than / Less Than

![[Arithmetic Circuit 2024-11-04 09.33.00.excalidraw]]