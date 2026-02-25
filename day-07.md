# Day 07 - 25 Feb 2026

## Challenge

### Tailwind Class Join

**Scenario:**  
Scenario (Tailwind CSS): Write `tailwindClassMerger` that joins only truthy class names with a single space.

**Example Output:**
```js
tailwindClassMerger(['p-4','','bg-black',null,'text-white']) -> "p-4 bg-black text-white"
```

---

## My Prompt

**Goal:** Create a Tailwind Class Joiner.  
**Constraints:** You MUST take array as input. Avoid white-spaces, write single-line arrow function.  
**Edge Cases:** Handle falsy values in array, remove them.  
**Output Format:** It should return joined string with truthy values.  

## Generated Code

```js
const tailwindClassMerger = (classes) => classes.filter(Boolean).join(' ');
```

---

Prompt tokens: 58  
Code tokens: 14  
Efficiency total: 72  

Attempts: 1  
Your best: 100 points on first attempt  
Submitted at 11:05 pm  
#4 on Leaderboard with 693 points  
