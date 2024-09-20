---
tags:
  - e_e_214
created: 2024-09-18
updated: 2024-09-20
---

| AB\CD | 00  | 01  | 11  | 10  |
| ----- | --- | --- | --- | --- |
| 00    | 1   | 1   | 0   | 0   |
| 01    | 0   | 0   | 0   | 0   |
| 11    | 1   | 0   | 1   | 1   |
| 10    | 0   | 0   | 1   | 1   |

Find the largest groups with size $2^n$. For every group, you reduce the number of variables needed by $n$.
Groups must be rectangles of size:
- 1x1 ($2^0$)
- 2x1 ($2^1$)
- 2x2 ($2^2$)
- 4x1 ($2^2$)
- 4x2 ($2^3$)

*You only need to loop each value once.*

> *Example*
> Find a [[Logic Equation#Minterms and Maxterms|minterm]] equation for the following K-map:

| A\BC | 00  | 01  | 11  | 10  |
| ---- | --- | --- | --- | --- |
| 0    | 0   | 1   | 0   | 1   |
| 1    | 0   | 1   | 1   | 0   |

$Y \Leftarrow \overline A B \overline C + A C + \overline B C$

---

You can also loop zeros to find a maxterm POS equation:

> *Example*
> Find a maxterm POS equation for the following K-map:

| A\BC | 00  | 01  | 11  | 10  |
| ---- | --- | --- | --- | --- |
| 0    | 0   | 1   | 0   | 0   |
| 1    | 0   | 0   | 1   | 1   |

$Y \Leftarrow (A + \overline B) (\overline A + B) (B C)$

---

## Finding a Minimal Circuit

For both the SOP and POS equations:

1. Count the number of gates
2. Count the number of inputs

## Supermaps

![[Karnaugh Map 2024-09-18 09.21.25.excalidraw]]

Values in the same relative positions can be grouped together.

## Optimising Gates

![[Karnaugh Map 2024-09-18 09.37.14.excalidraw]]

Implementing a sub-optimal solution for one output to optimise the entire system by re-using gates.

To do this, you can look at values in the same relative positions across multiple K-maps of outputs.

## Don't Cares

If a combination of inputs is physically impossible, it can be treated as a **don't care** ($\phi$ or X). For instance, radio buttons.

You can loop a don't care as either a `0` or a `1`, whichever makes the logic simpler.

| A\BC | 00  | 01  | 11  | 10  |
| ---- | --- | --- | --- | --- |
| 0    | 0   | 1   | X   | 1   |
| 1    | 0   | X   | X   | 0   |

> *Example*
> $$ Y \Leftarrow \sum m(0, 1, 6, 7, 9, 12, 14) + \phi (3, 4, 11, 13) $$

$Y_{SOP} = \overline B D + B \overline D + \overline A B C + \overline A \overline B \overline C$

$Y_{POS} = (\overline A + B + D) (B + \overline C) (\overline A + \overline B + \overline D) (\overline B + C + \overline D)$