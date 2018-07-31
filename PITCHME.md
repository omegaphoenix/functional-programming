# Why Functional Programming Rocks

Baby J

---

### Higher Order Functions

```javascript
// 1 + 2 + 3
let sum = 0;
const nums = [1, 2, 3];
for (let i = 0; i < nums.length; i++) {
  sum = sum + nums[i];
}

// Another loop - "abc"
let res = '';
const strs = ['a', 'b', 'c'];
for (let i = 0; i < strs.length; i++) {
  res = res + strs[i];
}
```

```javascript
const sum = [1, 2, 3].reduce((a, b) => (a + b), 0) // > 6
const res = ["a", "b", "c"].reduce((a, b) => a + b, "") // > "abc"
```

---

### Immutability

- Mutation Mistakes
- Concurrent Code

---

### Pure Functions

- Always Same Output For a Given Input
- Easier Testing and Debugging

---

### Lazy Evaluation

- Efficient
- Infinite Lists

```
quickSort [] = []
quickSort (x:xs) = quickSort (filter (< x) xs) ++ [x] ++ quickSort (filter (>= x) xs)

minimum ls = head (quickSort ls)
```

---

### Why FP?

- Easier Reasoning
- Easier Testing and Debugging
- Easier Parallel Programming

---

### References

![Benefits of Functional Programming](https://alvinalexander.com/scala/fp-book/benefits-of-functional-programming)
![Why Functional Programming Matters](https://www.cs.kent.ac.uk/people/staff/dat/miranda/whyfp90.pdf)
![Why Functional Programming From A Developer Productivity Perspective](https://medium.com/@xiaoyunyang/why-functional-programming-from-a-developer-productivity-perspective-69c4b8100776)
