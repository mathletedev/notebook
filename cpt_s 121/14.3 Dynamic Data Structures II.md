---
tags:
  - cpt_s_121
---

-> [Lecture code](https://github.com/mathletedev/cpt_s/blob/main/121/lectures/2023-12-01)

```c
int insert_front(Node **head, int data) {
	Node *node = create_node(data);

	if (node == NULL)
		return 0;

	if (*head == NULL)
		*head = node;
	else {
		node->next = *head;
		*head = node;
	}

	return 1;
}
```

- Note: use a pointer to a pointer `Node **` to change the **pointer** to the `Node`