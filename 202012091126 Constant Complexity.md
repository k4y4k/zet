---
title: Constant Complexity
date: 2020-12-09 11:26
---

Notation: `O(1)`

An algorithm with constant complexity will perform a set number of operations _no matter the size of the input._

```javascript
const logFirstItem = items => console.log(items[0])
```

```javascript
const logFirstFiveItems = items => {
  console.log(items[0])
  console.log(items[1])
  console.log(items[2])
  console.log(items[3])
  console.log(items[4])
}
```

This would be `O(5)`, right? Wrong. We simplify it down to 1. Anything like `O(7)`, `O(194)`, or `O(100000000)` are all simplified down to be `O(1)`.

---

#bigO #algorithm
