# Day 30 - 20 March 2026

## Challenge

### Capstone Delivery Checklist

**Scenario:**  
Scenario (Hard full stack capstone): Write `capstoneChecklist` returning completion percentage (0-100) from boolean checklist values.

**Example Output:**
```js
capstoneChecklist({frontend:true,backend:true,db:false}) -> 67
```

---

## My Prompt

**Goal:** Create Capstone Delivery Checklist Creator.  
**Constraints:** MUST take object as input. Avoid spaces, write arrow-function.  
**Edge Cases:** Handle any number of properties in object.  
**Output Format:** It should return percentage from boolean checklist values.  

## Generated Code

```js
const capstoneChecklist=(obj)=>{const values=Object.values(obj);if(values.length===0)return 0;const trueCount=values.filter(v=>v===true).length;return Math.round((trueCount/values.length)*100);}
```

---

Prompt tokens: 53  
Code tokens: 20  
Efficiency total: 73  

Attempts: 1  
Your best: 100 points  
Submitted at 2:05 am on 21st March  
#4 on Leaderboard with 2993 points  

---

## Prompt History

1. ```markdown
    **Goal:** Create Capstone Delivery Checklist Creator
    **Constraints:** MUST take object as input. Avoid spaces, write arrow-function
    **Edge Cases:** Handle any number of properties in object
    **Output Format:** It should return percentage from boolean checklist values
    ```
