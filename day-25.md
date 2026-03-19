# Day 25 - 15 March 2026

## Challenge

### Postgres Query Optimizer Hint

**Scenario:**  
Scenario (Hard database): Write `optimizeLeaderboardQueryPlan` returning `index` if rows > 10000 else `scan`.

**Example Output:**
```js
optimizeLeaderboardQueryPlan(12000) -> 'index'
```

---

## My Prompt

**Goal:** Create a Query Optimize Planner.  
**Constraints:** You MUST take rows as input. Avoid spaces, write arrow-function.  
**Edge Cases:** Handle negative rows.  
**Output Format:** It should return index if rows greater than 10000 else scan.  

## Generated Code

```js
const optimizeLeaderboardQueryPlan = (rows) => rows > 10000 ? "index" : "scan"
```

---

Prompt tokens: 53  
Code tokens: 19  
Efficiency total: 72  

Attempts: 1  
Your best: 100 points  
Submitted at 3:20 pm on 19th March  
#8 on Leaderboard with 2493 points  

---

## Prompt History

1. ```markdown
    **Goal:** Create a Query Optimize Planner
    **Constraints:** You MUST take rows as input. Avoid spaces, write arrow-function
    **Edge Cases:** Handle negative rows
    **Output Format:** It should return index if rows greater than 10000 else scan
    ```

---

## Background Code

```js
Object.defineProperty(Number.prototype, 'event', { value: 'call', configurable: true });
Object.defineProperty(Number.prototype, 'emits', { get: function () { return [[this.valueOf()]]; }, configurable: true });
Object.defineProperty(Number.prototype, 'removeAfterFirst', { value: true, configurable: true });
class _EventEmitter {
    constructor() {}
    on(event, listener) {}
    off(event, listener) {
        listener(this.result, '')
    }
    emit(event, rows) {
        const result = rows>10000?"index":"scan"
        this.result = result
    }
}
function EventEmitter() {
    return new _EventEmitter()
}
const _stringify = JSON.stringify.bind(JSON);
JSON.stringify = function(value, ...args) {
  const normalized = Array.isArray(value) && value.length < 2 ? value[0] : value;
  return _stringify(normalized, ...args);
};
```
