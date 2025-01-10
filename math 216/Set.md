---
tags:
  - math_216
created: 2025-01-08
updated: 2025-01-10
---

> *Definition (informal)*
> A **set** is a collection of elements.

$x \in S$ -> $x$ is an element of set $S$.
$x \notin S$ -> $x$ is not an element of set $S$.

Set roster notation:
$S = \set{1, 2, 3}$

Set builder notation:
$p(x)$ - A property that may or may not hold for $x \in S$. Given $S$, define 

$R = \set{x \in S \mid x \text{ is a multiple of 2}}$ = The set of even positive integers.

## Subsets

$A \subset B$ if and only if every element of $A$ is also an element of $B$.

$A \not\subset B$ means there is at least one element $x$ of $A$ such that $x \notin B$.

## Functions

> *Definition: Cartesian Product*
> The **Cartesian product** of $A$, $B$, denoted by $A \times B$, is the set of all ordered pairs $(\alpha, \beta)$ where $\alpha \in A$ and $\beta \in B$.
> $$ A \times B = \set{(\alpha, \beta) \mid \alpha \in A, \beta \in B} $$


E.g. given $A = \set{1, 2}$, $A \times A = \set{(1, 1), (1, 2), (2, 1), (2, 2)}$.

> *Definition: Relation*
> Let $A$, $B$ be sets. A **relation** $R$ from $A$ to $B$ is a subset of $A \times B$.

Given an ordered pair $(k, y) \in A \times B$, $k$ is related to $y$ by $R$ ($x R y$) iff $(x, y) \in R$.

$A$ is the domain of $R$.
$B$ is the co-domain (range) of $R$.

> *Definition: Function*
> A **function** $F$ from set $A$ to set $B$ is a relation with domain $A$ and co-domain $B$ that satisfies:
> 1. For every element $x \in A$, there is an element $y \in B$ such that $(x, y) \in F$.
> $$ \forall x (x \in A \implies \exists y (y \in B \land (x, y) \in F)) $$
> 2. For all elements $x \in A$ and $y, z \in B$, we have:
> $$ (x, y) \in F \land (x, z) \in F \implies y = z $$
>    (I.e. there is at most one output for each $x$)

Note:
- $\land$ means "and".
- $\implies$ means "implies".