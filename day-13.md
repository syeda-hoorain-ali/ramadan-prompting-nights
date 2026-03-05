# Day 13 - 3 March 2026

## Challenge

### Node Rate Limit Counter

**Scenario:**  
Scenario (Backend Node.js): Write `applyRateLimit` that returns whether a request is allowed for `count <= limit`.

**Example Output:**
```js
applyRateLimit(3,5) -> true
```

---

## My Prompt

**Goal:** Create a Rate Limit Counter, that checks whether a request is allowed.  
**Constraints:** You MUST take count and limit as input. Avoid white-spaces, write single-line arrow function.  
**Edge Cases:** Handle case where count exceed limit.  
**Output Format:** It should return boolean.  

## Generated Code

```js
const applyRateLimit = (count, limit) => count <= limit;
```

---

Prompt tokens: 63  
Code tokens: 15  
Efficiency total: 78  

Attempts: 1  
Your best: 100 points  
Submitted at 8:40 pm on 5th March  
#5 on Leaderboard with 1293 points  

---

## Prompt History

1. ```markdown
    **Goal:** Create a Rate Limit Counter, that checks whether a request is allowed
    **Constraints:** You MUST take count and limit as input. Avoid white-spaces, write single-line arrow function
    **Edge Cases:** Handle case where count exceed limit
    **Output Format:** It should return boolean
    ```
