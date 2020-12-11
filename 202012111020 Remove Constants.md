---
title: Remove Constants
date: 2020-12-11 10:20
---

This is step 2 of [[202012091203 Simplify Big O Expressions]]

Consider this function:

```javascript
function printFirstItemThenFirstHalfThenSayHi100Times(items) {
  console.log(items[0]) // O(1)

  var middleIndex = Math.floor(items.length / 2)
  var index = 0

  while (index < middleIndex) {
    // O(n/2)
    console.log(items[index])
    index++
  }

  for (var i = 0; i < 100; i++) {
    // O(100)
    console.log('hi')
  }
}
```

At first glance, this might seem to have a Big O time complexity of `O(1 + n/2 + 100)`. But this is not totally correct, because we drop the constants, like `+1`, `/2` or `+100`. As `n` grows, these constants become less and less significant, so we don't consider them an element in regards to the scalability of an algorithm (which, after all, is what Big O was invented to analyse).

| Step               | Description                                        |
| ------------------ | -------------------------------------------------- |
| `O(1 + n/2 + 100)` | start                                              |
| `O(n/2 + 101)`     | collect the terms being added                      |
| `O(n/2 + 1)`       | simplify the addition to `1`                       |
| `O(n + 1)`         | remove the constant division and constant addition |
| `O(n)`             | result                                             |

([#neagoie-35BigRule2020])

---

[#neagoie-35BigRule2020]: Neagoie, A. (2020, December). 35. Big O Rule 2. Udemy. Retrieved from https://www.udemy.com/course/master-the-coding-interview-data-structures-algorithms/learn/lecture/12145938#overview

---

#bigO #algorithm
