# Day 12 - 2 March 2026

## Challenge

### Dashboard Widget Mapper

**Scenario:**  
Scenario (React/Next.js): Write `dashboardCardLayout` to map metric values into standardized card objects `{label,value,trend}`.

**Example Output:**
```js
dashboardCardLayout({users:20,active:16}) -> [{label:'users',value:20,trend:'up'},{label:'active',value:16,trend:'up'}]
```

---

## My Prompt

**Goal:** Create a Dashboard Widget Mapper.  
**Constraints:** You MUST take object as input. Avoid white-spaces, write single-line arrow function.  
**Edge Cases:** Handle missing input, use default parameter.  
**Output Format:** It should return list of object in this order: {label:key,trend:'up/flat/down',value}.  

## Generated Code

```js
const dashboardCardLayout=(o={})=>Object.entries(o).map(([k,v])=>({label:k,trend:v>0?'up':v<0?'down':'flat',value:v}))
```

---

Prompt tokens: 62  
Code tokens: 15  
Efficiency total: 77  

Attempts: 12  
Your best: 100 points  
Submitted at 7:37 am  
#2 on Leaderboard with 1193 points  

---

## Prompt History

1. ```markdown
    **Goal:** Create a Dashboard Widget Mapper
    **Constraints:** You MUST take object as input. Avoid white-spaces, write single-line arrow function
    **Edge Cases:** Handle missing values
    **Output Format:** It should return list of object: {label:key,value,trend:'up/flat/down'}
    ```

2. ```markdown
    **Goal:** Create a Dashboard Widget Mapper
    **Constraints:** You MUST take object as input. Avoid white-spaces, write single-line arrow function
    **Edge Cases:** Handle missing values
    **Output Format:** It should return list of object: {label:key,trend:'up/flat/down',value}
    ```

3. ```markdown
    **Goal:** Create a Dashboard Widget Mapper
    **Constraints:** You MUST take object as input. Avoid white-spaces, write single-line arrow function
    **Edge Cases:** Handle missing values
    **Output Format:** It should return list of object in same order: {label:key,trend:'up/flat/down',value}
    ```

4. ```markdown
    **Goal:** Create a Dashboard Widget Mapper
    **Constraints:** You MUST take object as input. Avoid white-spaces, write single-line arrow function
    **Edge Cases:** Handle missing/empty object
    **Output Format:** It should return list of object in same order: {label:key,trend:'up/flat/down',value}
    ```

5. ```markdown
    **Goal:** Create a Dashboard Widget Mapper
    **Constraints:** You MUST take object as input. Avoid white-spaces, write single-line arrow function
    **Edge Cases:** Handle missing input, use default parameter
    **Output Format:** It should return list of object in same order: {label:key,trend:'up/flat/down',value}
    ```

6. ```markdown
    **Goal:** Create a Dashboard Widget Mapper
    **Constraints:** You MUST take object as input. Avoid white-spaces, write single-line arrow function
    **Edge Cases:** Handle missing input, use default parameter
    **Output Format:** It should return list of object in this order: {label:key,trend:'up/flat/down',value}
    ```
