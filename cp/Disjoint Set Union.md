---
tags:
  - cp
---

```cpp
struct DSU {
  std::vector<int> e;

  DSU(int N) { e.assign(N, -1); }

  int find(int x) { return e[x] < 0 ? x : e[x] = find(e[x]); }
  bool same_set(int x, int y) { return find(x) == find(y); }
  int size(int x) { return -e[find(x)]; }
  bool unite(int x, int y) {
    x = find(x), y = find(y);
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