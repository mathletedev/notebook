---
tags:
  - cp
---

## Minimising

```cpp
int low = 0, high = N;
while (low < high) {
  int mid = (low + high) / 2;

  if (is_possible(mid))
    high = mid;
  else
    low = mid + 1;
}
```

## Maximising

```cpp
int low = 0, high = N;
while (low < high) {
  int mid = (low + high) / 2 + (low + high) % 2;

  if (is_possible(mid))
    low = mid;
  else
    high = mid - 1;
}
```