---
tags:
  - cs_143
created: 2025-01-09
---

> Consider the language:
> $$ \set{(^i )^i \mid i \geq 0} $$

This is a language with a *nesting structure*.

## Pipeline

| *Phase* | *Input*              | *Output*         |
| ------- | -------------------- | ---------------- |
| Lexer   | String of characters | String of tokens |
| Parser  | String of tokens     | Parse tree       |

Note: Sometimes the parser performs the role of the lexer as well.

## Parsing

> **Input**: Sequence of tokens from the lexer
> **Output**: Parse tree of the program

## Context-Free Grammars (CFGs)

We need:
- A language for describing valid strings of tokens
- A method for distinguishing valid from invalid strings of tokens

Note: Programming languages have a natural recursive structure.
- E.g. `if EXPR then EXPR else EXPR fi`

Context-free grammars are a natural notation for this recursive structure

A CFG consists of:
- A set of **terminals** $T$
- A set of **non-terminals** $N$
- A **start symbol** $S$ where $S \in N$
- A set of **productions** $X \rightarrow Y_1, \dots, Y_n$ where $X \in N, \quad Y_i \in N \cup T \cup \set{\epsilon}$

Productions can be read as rules.
E.g. $S \rightarrow (s)$

Steps:
1. Begin with a string with only the start symbol $S$.
2. Replace any non-terminal $X$ in the string by the right-hand side of some production $X \rightarrow Y_1, \dots, Y_n$.
3. Repeat (2) until there are no non-terminals.

E.g. $X_1, \dots, X_i, X, X_{i + 1}, \dots, X_n \rightarrow X_1, \dots, X_i, Y_1, \dots, Y_k, X_{i + 1}, \dots, X_n$

Note on notation:
$\alpha_0 \overset{*}\rightarrow \alpha_n$ is equivalent to $\alpha_0 \rightarrow \alpha_1 \rightarrow \alpha_2 \rightarrow \cdots \rightarrow \alpha_n$
$\overset{*}\rightarrow$ means "rewrites in 0 or more steps".

> Let $G$ be a context-free grammar with start symbol $S$.
> Then the language $L(G)$ of $G$ is:
> $$ \set{a_1, \dots, a_n \mid \forall i \quad a_i \in T \quad S \overset{*}\rightarrow \alpha_1, \dots, \alpha_n} $$

- Terminals are so-called because there are no rules for replacing them.
- Once generated, terminals are permanent.
- Terminals out to be the *tokens* of the language.

For a CFG:
- Membership in a language is "yes" or "no"; also need a parse tree of the input
- Must handle errors gracefully
- Need an implementation of CFGs (e.g. a bison)

Left off: 19:40