---
tags:
  - science_olympiad
  - quantum_quandaries
---

> A set containing linearly independent vectors that spans a given space

## Vectors

A [[vector]] can be represented with a matrix: $
\begin{bmatrix}
	a\\
	b
\end{bmatrix}
$

## Linearly independent basis

These is a linearly independent basis:
$$
\left\{
\begin{bmatrix}
	0\\
	1
\end{bmatrix}
,
\begin{bmatrix}
	1\\
	2
\end{bmatrix}
\right\}
$$

With a linearly independent basis, we can reach any point in a space by multiplying by [[scalar|scalars]].

- $R^1$: 1-dimensional space (1 vector required)
- $R^2$: 2-dimensional space (2 vectors required)
- $R^3$: 3-dimensional space (3 vectors required)
- $R^n$: $n$-dimensional space ($n$ vectors required)

### Solving

Assuming $
A = \begin{bmatrix}
	3 & 1 & 4\\
	6 & 7 & 1\\
	1 & 2 & 3
\end{bmatrix}
$ If there is a non-trivial solution to $Ax = 0$, then $A$ is linearly independent.

We can perform row operations on $A$ to turn it into reduced row echelon form.

**Reduced row echelon form**: $
\begin{bmatrix}
	1 & 0 & 0\\
	0 & 1 & 0\\
	0 & 0 & 1
\end{bmatrix}
$
If we can get a matrix to reduced row echelon form, then it is linearly independent.