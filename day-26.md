# Day 26 - 16 March 2026

## Challenge

### Docker Stage Selector

**Scenario:**  
Scenario (Hard Docker): Write `dockerStagePlan` returning `production` if optimize flag true else `development`.

**Example Output:**
```js
dockerStagePlan(true) -> 'production'
```

---

## My Prompt

**Goal:** Create a Docker Stage Selector.  
**Constraints:** You MUST take optimize flag as input. Avoid spaces, write arrow-function.  
**Edge Cases:** Handle missing input, use default.  
**Output Format:** It should return production if optimize flag is true else development.  

## Generated Code

```js
const dockerStagePlan=(optimize=false)=>optimize?"production":"development"
```

---

Prompt tokens: 57  
Code tokens: 6  
Efficiency total: 63  

Attempts: 1  
Your best: 100 points  
Submitted at 3:25 pm on 19th March  
#8 on Leaderboard with 2593 points  

---

## Prompt History

1. ```markdown
    **Goal:** Create a Docker Stage Selector
    **Constraints:** You MUST take optimize flag as input. Avoid spaces, write arrow-function
    **Edge Cases:** Handle missing input, use default
    **Output Format:** It should return production if optimize flag is true else development
    ```
