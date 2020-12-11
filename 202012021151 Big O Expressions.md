---
title: Big O Expressions
date: 2020-12-02 11:51
---

Big O expresses an algorithm's runtime in terms of how quickly the runtime or [[202012021203 Space Complexity in Big O|space complexity]] grows as the input to an algorithm gets bigger and bigger up to an indefinite, arbitrary point. The input of an algorithm is called [[202012021155 n]].

Those expressions look like this:

| Rating | Expression | Name | What It Means |
| --- | --- | --- | --- |
| Excellent | `O(1)` | [[202012091126 Constant Complexity]] | runtime stays the same relative to the size of the input |
| Excellent | `O(lg n)` |  |  |
| Fair | `O(n)` | [[202012091119 Linear Complexity]] | runtime increases linearly relative to input size |
| Horrible | `O(n²)` | [[202012091336 Quadratic Time]] | runtime increases by a power of 2 relative to input size |
| Horrible | `O(2ⁿ)` |  |  |
| Horrible | `O(n!)` | [[202012111314 Factorial Time]] | for every input, a nested loop is executed. Complexity grows by factors of itself |

And, compared, look like this:

![A chart showing how good / bad several Big O complexity notations are](./img/big-o-graph.png) [#rowell-KnowThyComplexities]

An algorithm can be described by several expressions, depending on [[202012021213 Case]].

There is a process to [[202012091203 Simplify Big O Expressions|simplifying these]].

---

[#rowell-KnowThyComplexities]: Rowell, E. (n.d.). Know Thy Complexities. Retrieved 9 December 2020, from Big-O Algorithm Complexity Cheat Sheet (Know Thy Complexities!) @ericdrowell website: https://www.bigocheatsheet.com/

---

#bigO
