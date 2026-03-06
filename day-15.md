# Day 15 - 5 March 2026

## Challenge

### FastAPI Task Payload Normalizer

**Scenario:**  
Scenario (Python/FastAPI): Write `taskCrudPayload` to normalize task input to `{title,done}` with default `done:false`.

**Example Output:**
```js
taskCrudPayload({title:'Review PR'}) -> {title:'Review PR',done:false}
```

---

## My Prompt

**Goal:** Create a Task Payload Normalizer.  
**Constraints:** You MUST take object as input. Avoid white-spaces, write single-line arrow function. 
**Edge Cases:** Handle missing done fields, returrn false.  
**Output Format:** It should return object in this order: {done,title}.  

## Generated Code

```js
const taskCrudPayload=o=>({done:o.done===undefined?false:o.done,title:o.title})
```

---

Prompt tokens: 57  
Code tokens: 8  
Efficiency total: 65  

Attempts: 1  
Your best: 100 points  
Submitted at 7:50 am  
#3 on Leaderboard with 1493 points  

---

## Prompt History

1. ```markdown
    **Goal:** Create a Task Payload Normalizer
    **Constraints:** You MUST take object as input. Avoid white-spaces, write single-line arrow function
    **Edge Cases:** Handle missing done fields, returrn false
    **Output Format:** It should return object in this order: {done,title}
    ```
