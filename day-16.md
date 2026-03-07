# Day 16 - 6 March 2026

## Challenge

### Docker Compose Service Summary

**Scenario:**  
Scenario (Docker): Write `composeServicesSummary` returning sorted service names from a compose-like object.

**Example Output:**
```js
composeServicesSummary({services:{api:{},web:{},db:{}}}) -> ['api','db','web']
```

---

## My Prompt

**Goal:** Create a Docker Compose Service Summary Generator.  
**Constraints:** You MUST take object as input with services field. Avoid white-spaces, write single-line arrow function.  
**Edge Cases:** Handle missing values, use default.  
**Output Format:** It should return list of services names.  

## Generated Code

```js
const composeServicesSummary=(c)=>(c?.services?Object.keys(c.services).sort():[])
```

---

Prompt tokens: 60  
Code tokens: 8  
Efficiency total: 68  

Attempts: 2  
Your best: 100 points  
Submitted at 10:55 pm  
#3 on Leaderboard with 1593 points  

---

## Prompt History

1. ```markdown
    **Goal:** Create a Docker Compose Service Summary Generator
    **Constraints:** You MUST take object as input with services field. Avoid white-spaces, write single-line arrow function
    **Edge Cases:** Handle missing vaules, use default
    **Output Format:** It should return list of services names
    ```
