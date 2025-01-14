---
tags:
  - cpt_s_223
created: 2025-01-13
---

> *Definition: Function*
> A **function** maps each element of a set $A$ (domain) to exactly one element of a set $B$ (codomain).

Representation: $f: A \to B$, where $f(x) = y, x \in A, y \in B$.

> *Interpretation: Set-Theoretic*
> A function is a relation that uniquely associates elements in one set (domain) with elements in another set (codomain).

> *Interpretation: Algebraic*
> Functions can be represented as algebraic formulas:
> - E.g. $f(x) = x^2$
> - E.g. $g(x) = 2x + 1$
>
> Composition: $(f \circ g)(x) = f(g(x))$.
> Inverse: $f^{-1}(f(x)) = x$.
> Especially useful for infinite sets.

> *Interpretation: Geometric*
> Points on a Cartesian plane: $(x, f(x))$.

## Growth of Functions

How functions behave as $x \to \infty$.

Comparing growth rates:
$$ \log x < x < x^k < x! $$

> *Definition: Asymptotic Notation*
> **Asymptotic notation** describes the behaviour of functions as inputs grow large.

Purpose: Provides an *upper bound*, *lower bound*, or *tight bound* of a function's growth.

Independent of algorithms or computer science - applicable to any function.

Key ideas:
- Dominant terms

## Big-O Notation

$f(x) \in O(g(x))$ if there exists constants $c > 0$ and $x_0 > 0$ such that:
$$ f(x) \leq c \cdot g(x), \forall x \geq x_0 $$

The "switch-over point" s called $N_0$ or $x_0$.

- Provides an upper bound for the growth of a function.
- Upper bounds provide worst-case estimates

## Big-Omega Notation

$f(x) \in \Omega(g(x))$ if there exists constants $c > 0$ and $x_0 > 0$ such that:
$$ f(x) \geq c \cdot g(x), \forall x \geq x_0 $$

## Big-Theta Notation

$f(x) \in \Theta(g(x))$ if there exists constants $c_1, c_2 > 0$ and $x_0 > 0$ such that:
$$ c_1 \cdot g(x) \leq f(x) \leq c_2 \cdot g(x), \forall x \geq x_0 $$

## Algorithm Analysis

- **Time complexity**: How execution time grows with input size.
- **Space complexity**: How memory usage grows with input size.

Note: The y-axis is usually the # of operations instead of time. This is because time depends on hardware specs.