---
tags:
  - e_e_214
created: 2024-09-04
updated: 2024-09-06
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