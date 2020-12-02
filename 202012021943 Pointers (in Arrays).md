---
title: Pointers (in Arrays)
date: 2020-12-02 19:43
---

| Operation | Time Complexity |
| --------- | --------------- |
| lookup    | `O(1)`          |

[[202012021931 Arrays|Arrays]] are great, but the necessity of having each element be a fixed size makes things... annoying.

As a workaround, we can instead store these variable-length bits of data somewhere in memory, and instead fill our array with _pointers_ - little tidbits that _point to_ the address of where this data is.

Note that this approach isn't cache-friendly, as there's no guarantee that any item co-exists closely in memory, like there is with a regular array. It's also slower because of this (but that slowness isn't reflected in [[202012021151 Big O Expressions|Big O]] - it's still considered `O(1)`)

Pointers aren't just limited to arrays, but they're useful there.

---

#datastructure #computers
