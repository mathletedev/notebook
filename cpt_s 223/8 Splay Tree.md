---
tags:
  - cpt_s_223
  - data_structures
created: 2025-02-03
---

> *Definition*
> A **splay tree** guarantees that any $M$ consecutive operations, starting from an empty tree, take at most $O(M \log N)$ time.

- Single operations might take $O(N)$ but the *amortised cost* per operation is $O(\log n)$.
- Over a long sequence, some operations may take more time, others less.

**Restructuring benefits**:
- Accessing deep nodes brings related deep nodes closer to the root
- Balances the tree (to some extent) during restructuring

**Logic**:
- Frequently accessed nodes are likely to be accessed again (*temporal locality*)
- Reduces average access times over multiple operations

## Cases

**Zig-zag**: Used for `LR` case
**Zig-zig**: Used for `LL` case