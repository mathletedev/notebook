---
tags:
  - e_e_214
created: 2024-08-30
updated: 2024-10-09
---

## NAND Relationship

![[Logic Gate 2024-08-30 09.25.19.excalidraw]]

```tikz
\usepackage{circuitikz}
\begin{document}
\begin{circuitikz}[american, voltage shift=0.5]

\draw (0, 0) node[rground]{}
node[nfet](Q1){FET}

\end{circuitikz}
\end{document}
```

| A   | B   | Q1  | Q2  | Q3  | Q4  | Y   |
| --- | --- | --- | --- | --- | --- | --- |
| 0   | 0   | on  | on  | off | off | 1   |
| 0   | 1   | on  | off | off | on  | 1   |
| 1   | 0   | off | on  | on  | off | 1   |
| 1   | 1   | off | off | on  | on  | 0   | 

Note: We can denote this as $Y_{AND}$.

## NOT Relationship

![[Logic Gate 2024-08-30 09.45.22.excalidraw]]

This is called an **inverter**.

| A   | Q1  | Q2  | Y   |
| --- | --- | --- | --- |
| 0   | on  | off | 1   | 
| 1   | off | on  | 0   |

## NOR Relationship

![[Logic Gate 2024-08-30 09.49.25.excalidraw]]

| A   | B   | Y   |
| --- | --- | --- |
| 0   | 0   | 1   |
| 0   | 1   | 0   |
| 1   | 0   | 0   |
| 1   | 1   | 0   |

---

pFETs and nFETs are *always* complementary. pFETs will always source from `Vdd`, and nFETs will always source from `GND`. The output will always be between the pFETs and nFETs.

**Metal oxide semiconductor (MOS)**: The type of semiconductor we use
**MOSFET**: MOS FET
**CMOS**: Complementary MOS

---

## Symbols

![[Logic Gate 2024-09-04 09.20.34.excalidraw]]

Buffers can be used to represent an inverter.

### Conjugates

![[Logic Gate 2024-09-04 09.28.47.excalidraw]]

To make a conjugate:
- Change the gate shape
- Where there are bubbles, remove bubbles
- Where there are no bubbles, add bubbles

---

## Compound Logic Gates

![[Logic Gate 2024-09-06 09.45.08.excalidraw]]

$Y \Leftarrow \overline A . \overline B . C + \overline A . B . C + A . B . C$

## XOR Gate

![[Logic Gate 2024-10-09 09.40.05.excalidraw]]

Total: 16 transistors

In general,
- XOR is `1` when an **odd** number of inputs are `1`
- XNOR is `1` when an **even** number of inputs are `1`