---
title: Different Terms for Inputs
date: 2020-12-11 10:24
---

This is step 3 of [[202012091203 Simplify Big O Expressions]].

```javascript
const chat = (input1, input2) => {
  input1.forEach(input => console.log(input))
  input2.forEach(input => console.log(input))
}
```

([#neagoie-36BigRule2020])

This function is NOT `O(n)`. Both loops won't have the same time / space complexity, because they _aren't the same input._ Therefore, we describe the runtime with different terms for the two different inputs: `O(a + b)`.

---

[#neagoie-36BigRule2020]: Neagoie, A. (2020, December). 36. Big O Rule 3. Udemy. Retrieved from https://www.udemy.com/course/master-the-coding-interview-data-structures-algorithms/learn/lecture/12145940#overview

---

#bigO #algorithm
