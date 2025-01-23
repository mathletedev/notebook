---
tags:
  - cpt_s_223
created: 2025-01-22
---

If a function calls itself `n` times, it will have `n` subtrees.

Total work = $\displaystyle\sum^n_{k = 0} \text{work done} (\text{subtree } n)$
- (Plus some constant $c$ to combine the work at each level)
- Base cases require constant time to compute

## Binary Search

- The area of the search space starts with the whole array of size `n`
- At each step the search space shrinks by half.

$T(n) = T\left({\dfrac{n}{2^k}}\right) + kc$
$2^k$ will reach $n$ when $k = \log_2(n)$
$T(n) = T(1) + \log_2(n) \cdot c = \log_2(n)$