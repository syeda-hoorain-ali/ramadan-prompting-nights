# Day 29 - 19 March 2026

## Challenge

### Observability Log Formatter

**Scenario:**  
Scenario (Hard backend observability): Write `observabilityLogShape` returning structured log object `{level,message,requestId,timestamp}`.

**Example Output:**
```js
observabilityLogShape('info','ok','req-1',123) -> {level:'info',message:'ok',requestId:'req-1',timestamp:123}
```

---

## My Prompt

**Goal:** Create a Observability Log Formatter.  
**Constraints:** MUST take level,message,requestId and timestamp as input. Avoid spaces, write arrow-function.  
**Edge Cases:** Handle missing values, use default.  
**Output Format:** It should return structured log object using input.  

## Generated Code

```js
const observabilityLogShape=(lvl='info',msg='',reqId='',ts=new Date().toISOString())=>({level:lvl,message:msg,requestId:reqId,timestamp:ts})
```

---

Prompt tokens: 54  
Code tokens: 15  
Efficiency total: 69  

Attempts: 1  
Your best: 100 points  
Submitted at 1:55 am on 20th March  
#2 on Leaderboard with 2893 points  

---

## Prompt History

1. ```markdown
    **Goal:** Create a Observability Log Formatter
    **Constraints:** MUST take level,message,requestId and timestamp as input. Avoid spaces, write arrow-function
    **Edge Cases:** Handle missing values, use default
    **Output Format:** It should return structured log object using input
    ```
