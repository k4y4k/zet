---
title: Hashing Function
date: 2020-12-03 09:19
---

A hashing function converts an input into a hash. The same input always resolves to the same hash.

They're what gives [[202012030840 Hash Tables]] their name.

In hash tables, they're used to transform an arbitrary key (e.g. a string) into an array-friendly index.

A simple hashing algorithm for strings might look like this:

1. Create a key under which to store a value
2. Convert each character in the key into a numerical character code
3. Sum the character codes to get a total
4. Total % array length = hash

For example, to hash the key `kayak`, using UTF-8, into an array of length 30:

```
k = u+006b = 107
a = u+0061 = 97
y = u+0079 = 121

107 + 97 + 121 + 97 + 107 = 529

529 % 30 = 19
```

Therefore, we can put whatever value we want assigned to key `kayak` into index `19` of our hash table.

If two distinct values have the same hash, that's known as a [[202012030911 Hash Collision]].

---

#algorithm #datastructure
