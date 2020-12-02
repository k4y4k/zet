---
title: Hash Collision
date: 2020-12-03 09:11
---

| Operation          | Time Complexity |
| ------------------ | --------------- |
| lookup (collision) | `O(n)`          |

When two (or more) keys [[202012030919 Hashing Function|hash]] to the same value, that's a hash collision.

One way to solve it:

1. Make the value of the colliding index into a linked list
2. Populate the linked list with the colliding values

In the 'real' world, collisions are considered to be pretty rare.

---

#datastructure
