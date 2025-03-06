---
tags:
  - cpt_s_223
  - data_structures
created: 2025-03-05
---

**Min heap**: Parent key >= children's keys
**Max heap**: Parent key <= children's keys

Note: A binary heap can be represented in an array.

**Null path length (NPL)**: Shortest path from a node to a `null`.
- $NPL(A) = \min(NPL(B), NPL(C)) + 1$

## Leftist Tree

New property: NPL of left node >= NPL of right subtree

### Merging a Leftist Tree

1. Compare roots
2. `R = merge(right subtree of smaller root, other tree)`
3. Add $R$ as the new right subtree (of the tree with smaller root)
4. If merging breaks the leftist property, swap the left and right nodes