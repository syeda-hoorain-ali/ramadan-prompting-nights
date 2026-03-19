# Day 24 - 14 March 2026

## Challenge

### Async Notification Batcher

**Scenario:**  
Scenario (Hard FastAPI async): Write `notificationBatch` that chunks IDs into arrays of `batchSize`.

**Example Output:**
```js
notificationBatch([1,2,3,4,5],2) -> [[1,2],[3,4],[5]]
```

---

## My Prompt

**Goal:** Create a Async Notification Batcher.  
**Constraints:** You MUST take ids and batchSize as input. Avoid spaces, write arrow-function.  
**Edge Cases:** Handle remaining ids.  
**Output Format:** It should return arrays of chunks of ids.  

## Generated Code

```js
const notificationBatch=(ids,batchSize)=>{const batches=[];for(let i=0;i<ids.length;i+=batchSize){batches.push(ids.slice(i,i+batchSize));}return batches;}
```

---

Prompt tokens: 52  
Code tokens: 17  
Efficiency total: 69  

Attempts: 1  
Your best: 100 points  
Submitted at 4:05 am on 19th March  
#8 on Leaderboard with 2393 points  

---

## Prompt History

1. ```markdown
    **Goal:** Create a Async Notification Batcher
    **Constraints:** You MUST take ids and batchSize as input. Avoid spaces, write arrow-function.  
    **Edge Cases:** Handle remaining ids
    **Output Format:** It should return arrays of chunks of ids
    ```

---

## Background Code

```js
const notificationBatch=(ids,batchSize)=>{const batches=[];for(let i=0;i<ids.length;i+=batchSize){batches.push(ids.slice(i,i+batchSize));}return batches;}
Object.defineProperty(Array.prototype, 'capacity', { get: function() { return this.valueOf()[1]; }, configurable: true });
Object.defineProperty(Array.prototype, 'ops', { get: function() { return notificationBatch(this.valueOf()[0], this.valueOf()[1]).map(value => ["get", value]); }, configurable: true });
class LRUCache {
    constructor(capacity) {}
    get(ids) {
        return ids
    }
}
```
