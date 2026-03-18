# Day 23 - 13 March 2026

## Challenge

### Queue Retry Strategy

**Scenario:**  
Scenario (Hard backend architecture): Write `queueRetryPlan` returning next delay in seconds with exponential backoff `base * 2^attempt` and max cap.

**Example Output:**
```js
queueRetryPlan(2,5,40) -> 20
```

---

## My Prompt

**Goal:** Create a Queue Retry Planner.  
**Constraints:** You MUST take attempt,base and max-cap as input. Avoid spaces, write arrow-function.  
**Edge Cases:** Handle result exceeding max-cap.  
**Output Format:** It should return next delay in seconds: base * 2^attempt.  

## Generated Code

```js
const queueRetryPlan = (attempt, base, maxCap) => Math.min(base * Math.pow(2, attempt), maxCap)
```

---

Prompt tokens: 57  
Code tokens: 21  
Efficiency total: 78  

Attempts: 1  
Your best: 100 points  
Submitted at 3:00 am on 19th March  
#9 on Leaderboard with 2293 points  

---

## Prompt History

1. ```markdown
    **Goal:** Create a Queue Retry Planner
    **Constraints:** You MUST take attempt,base and max-cap as input. Avoid spaces, write arrow-function
    **Edge Cases:** Handle result exceeding max-cap
    **Output Format:** It should return next delay in seconds: base * 2^attempt
    ```

---

## Background Code

```js
Object.defineProperty(Array.prototype, 'delays', { get: function() { return []; }, configurable: true });
Object.defineProperty(Array.prototype, 'values', { get: function() { return this.valueOf(); }, configurable: true });
Object.defineProperty(Array.prototype, 'limits', { get: function() { return 0; }, configurable: true });
const promisePool = async (tasks, limit) => {
    const [attempt, base, maxCap] = await Promise.all(tasks.map(task => task()));
    return Math.min(base * Math.pow(2, attempt), maxCap)
}
```
