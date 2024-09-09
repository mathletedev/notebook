---
tags:
  - e_e_214
created: 2024-09-04
updated: 2024-09-09
---

**AND**: $Y \Leftarrow A . B$ (Think multiplication)
**OR**: $Y \Leftarrow A + B$ (Think addition)
**NOT**: $Y \Leftarrow \overline A$

**NAND**: $Y \Leftarrow \overline{A . B}$

---

**Sum of Products (SOP)**: $Y \Leftarrow \overline A . B + A . C$
**Product of Sums (POS)**: $Y \Leftarrow (\overline A + B) . (A + C)$

For POS, take each zero-row of the truth table and negate each input in that row.

Two ways of thinking:
- SOP: ONE OF `|` the 1 cases is true
- POS: ALL OF `&` the NEGATED `~` 0 cases are false

---

## Minterms and Maxterms

Using the following table:

| A   | B   | C   | Y   | m   |
| --- | --- | --- | --- | --- |
| 0   | 0   | 0   | 1   | 0   |
| 0   | 0   | 1   | 1   | 1   |
| 0   | 1   | 0   | 0   | 2   |
| 0   | 1   | 1   | 0   | 3   |
| 1   | 0   | 0   | 1   | 4   |
| 1   | 0   | 1   | 0   | 5   |
| 1   | 1   | 0   | 1   | 6   |
| 1   | 1   | 1   | 0   | 7   |

**minterm equation**: $Y \Leftarrow \sum m(0, 1, 4, 6)$
This is equivalent to $\overline A . \overline B . \overline C + \overline A . \overline B . C + A . \overline B . \overline C + A . B . \overline C$

A minterm contains all the variables.

**maxterm equation**: $Y \Leftarrow \prod M (2, 3, 5, 7)$
This is equivalent to $(A + \overline B + C) . (A + \overline B + \overline C) . (\overline A + B + \overline C) . (\overline A + \overline B + \overline C)$