---
title: Dynamic Arrays
date: 2020-12-02 19:53
---

| Operation                            | Time Complexity |
| ------------------------------------ | --------------- |
| append (best / average case)         | `O(1)`          |
| append (worst case; doubling append) | `O(n)`          |
| prepend                              | `O(n)`          |

[[202012021931 Arrays]] are kind of stuck when they're full. Enter dynamic arrays.

These work by transparently augmenting an _underlying_ array. When the underlying array is filled, it's then duplicated into a new, bigger array (which is usually twice the size).

The used space in a dynamic array is its `size`, and the total size it has to play with is called its `capacity`. `size` is kept track of by the structure.

On an append that would cause its `size` to exceed its `capacity`, the following happens:

1. A new, bigger array (`new`) is created somewhere in memory
2. Every element from the current array (`old`) is copied in sequence into `new`
3. `old` is disposed of, as it's not needed anymore
4. The element that couldn't fit into `old` is appended into `new`

Appends that trigger this process are known as _doubling appends_. They're `O(n)` time, because they have to loop through `n` items in `old` to add them to `new`.

However, because this happens exponentially less often as a dynamic array grows, an average-case append to a dynamic array is still considered to be `O(1)`. All the regular appends are 'paying for' the doubling append, should it happen.

This is the tradeoff - the size of the array doesn't need to be known ahead of time, but appends can be expensive.

Prepending an element to a dynamic array takes `O(n)` time, as every existing element needs to be "shuffled down" one slot to make room.

JavaScript uses dynamic arrays by default.

---

#datastructure #computers
