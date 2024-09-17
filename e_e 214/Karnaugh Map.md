---
tags:
  - e_e_214
created: 2024-09-16
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