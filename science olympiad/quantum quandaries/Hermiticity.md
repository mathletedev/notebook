---
tags:
  - science_olympiad
  - quantum_quandaries
---

## Complex conjugation

Starting with $A$:
$$
A = \begin{bmatrix}
	1 & -2 - i & 5\\
	1 + i & i & 4 - 2i
\end{bmatrix}
$$

We first transpose $A$:
$$
A^T = \begin{bmatrix}
	1 & 1 + i\\
	-2 - i & i\\
	5 & 4 - 2i
\end{bmatrix}
$$

Then conjugate each of the elements of $A$:
$$
A^H = \begin{bmatrix}
	1 & 1 - i\\
	-2 + i & -i\\
	5 & 4 + 2i
\end{bmatrix}
$$

$A$ is **Hermitian** if $A = A^H$.

For instance, $
\begin{bmatrix}
	0 & i\\
	-i & 0
\end{bmatrix}
$ is a Hermitian matrix.