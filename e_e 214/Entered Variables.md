---
tags:
  - e_e_214
created: 2024-09-20
see also: "[[Karnaugh Map]]"
---

| A   | B   | C   | Y   |
| --- | --- | --- | --- |
| 0   | 0   | 0   | 0   |
| 0   | 0   | 1   | 1   |
| 0   | 1   | 0   | 1   |
| 0   | 1   | 1   | 0   |
| 1   | 0   | 0   | 0   |
| 1   | 0   | 1   | 0   |
| 1   | 1   | 0   | 1   |
| 1   | 1   | 1   | 1   |

Can be transformed into:

| A   | B   | Y             |
| --- | --- | ------------- |
| 0   | 0   | $C$           |
| 0   | 1   | $\overline C$ |
| 1   | 0   | 0             |
| 1   | 1   | 1             |

Or:

| A   | Y                               |
| --- | ------------------------------- |
| 0   | $\overline B C + B \overline C$ |
| 1   | $B$                             |

## Techniques for Simplifying

### Using [[Karnaugh Map|K-maps]]

1. Draw out the full K-map using all variables
2. Expand terms of the outer variables to the inner cells

### Using [[Karnaugh Map#Supermaps|Supermaps]]

1. Replace every cell with a submap
2. Loop according to supermap rules
3. If you loop a `1` with an entered variable, you must loop the other half as well