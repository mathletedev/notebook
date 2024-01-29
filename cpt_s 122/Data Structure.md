---
tags:
  - cpt_s_122
code:
  - https://github.com/mathletedev/cpt_s/blob/main/122/lectures/movies
---

> An organisation of information, usually in memory, for better *algorithm efficiency*, such as **queue**, **stack**, **linked list**, **heap**, **dictionary**, and **tree**, or conceptual unity, such as the name and address of a person. It may include redundant information, such as length of the **list** or number of **nodes** in a **sub-tree**.

## Selecting a data structure

Consider two linear data structures:

1. Array `[ 3 | 2 | 7 | 5 ]`
	- Indexing, searching, insertion, deletion
	- $O(1)$ time complexity
	- Can't resize
1. Linked list `[ 3 ] -> [ 2 ] -> [ 7 ] -> [ 5 ]`
	- Indexing, searching, insertion, deletion
	- $O(n)$ time complexity
	- Dynamic memory (can resize)

### Steps

1. Analyse problem, consider constraints and resource requirements
2. Determine basic operations that must be supported
3. Select best data structure that fits these conditions