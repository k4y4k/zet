---
title: quadratic time
date: 2020-12-09 13:36
---

[[202012021151 Big O Expressions|Big O Notation]]: `O(n²)`.

This appears when loops get nested, like such:

```javascript
const logAllPairs = boxes => {
  boxes.forEach(box1 => {
    boxes.forEach(box2 => {
      console.log(box1, box2)
    })
  })
}
```

---

#bigO #algorithm
