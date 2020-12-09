---
title: Linear Complexity
date: 2020-12-09 11:19
---

Notation: `O(n)`

Algorithms with linear time complexity will run longer and longer the bigger the input, relative to the size of the input.

An example:

```javascript
const compressBoxes = boxes => {
  for (let i = 0; i < boxes.length; i++) {
    console.log(boxes[i])
  }
}
```

This function will run one operation (the log) per loop - and it loops over every element in the array. Therefore, it has a _linear runtime_.

---

#bigO #algorithm
