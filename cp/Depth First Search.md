---
tags:
  - cp
---

```cpp
void dfs(int node) {
  if (visited[node])
    return;
  visited[node] = 1;

  for (int u : adj[node])
    dfs(u);
}
```