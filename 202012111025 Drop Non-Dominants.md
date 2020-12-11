---
title: Drop Non-Dominants
date: 2020-12-11 10:25
---

This is step 4, the final step of [[202012091203 Simplify Big O Expressions]].

```javascript
const printAllNumbersThenAllPairSums = numbers => {
  console.log('These are the numbers:')
  numbers.forEach(number => console.log(number))

  console.log('...and these are their sums:')
  numbers.forEach(firstNumber => {
    numbers.forEach(secondNumber => console.log(firstNumber + secondNumber))
  })
}
```

([#neagoie-38BigRule2020])

The Big O time complexity of this is `O(n + n²)`, right?

Nah. We only care about the most important term, so it's actually `O(n²)`.

---

[#neagoie-38BigRule2020]: Neagoie, A. (2020, Dev). 38. Big O Rule 4. Udemy. Retrieved from https://www.udemy.com/course/master-the-coding-interview-data-structures-algorithms/learn/lecture/12145946#overview

---

#bigO #algorithm
