---
tags:
  - cpt_s_223
  - data_structures
created: 2025-02-03
---

**Efficiency**: $O(H)$ where $H$ is the height of the tree.

Different implementations of a self-balancing tree:
1. AVL Trees
2. Splay Trees
3. Red-Black Trees

## Binary Search Trees

- Each node has at most two children
- All nodes in the left subtree are lesser than any node in the right subtree.

## AVL Trees

New property: For every node, the *height difference* between its left and right subtrees is at most one.

Four cases:
- `LL` case: Perform a right rotation
- `RR` case: Perform a left rotation
- `LR` case: Perform a left rotation on the left subtree, then a right rotation
- `LR` case: Perform a right rotation on the right subtree, then a left rotation