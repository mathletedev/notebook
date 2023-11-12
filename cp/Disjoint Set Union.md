---
tags:
  - cp
---

```cpp
struct DSU {
  std::vector<int> e;

  DSU(int n) { e.assign(n, -1); }

  int comp(int x) { return e[x] < 0 ? x : e[x] = comp(e[x]); }
  bool same_set(int x, int y) { return comp(x) == comp(y); }
  int size(int x) { return -e[comp(x)]; }
  bool unite(int x, int y) {
    x = comp(x), y = comp(y);
    if (x == y)
      return 0;
    if (e[x] > e[y])
      std::swap(x, y);
    e[x] += e[y];
    e[y] = x;
    return 1;
  }
};
```