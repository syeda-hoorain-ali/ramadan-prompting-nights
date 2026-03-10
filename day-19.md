# Day 19 - 9 March 2026

## Challenge

### CSV Row to JSON Mapper

**Scenario:**  
Scenario (Python data API): Write `csvRowsToJson` mapping row arrays to objects by headers.

**Example Output:**
```js
csvRowsToJson(['name','age'],[['Ali','20']]) -> [{name:'Ali',age:'20'}]
```

---

## My Prompt

**Goal:** Create a CSV Row to JSON Mapper.  
**Constraints:** You MUST take header and rows array as input. Avoid white-spaces, write arrow-function.  
**Edge Cases:** Handle empty rows.  
**Output Format:** It should return array of objects, sorted alphabetically.  

## Generated Code

```js
const csvRowsToJson=(headers,rows)=>rows.filter(r=>r.length>0).map(row=>Object.fromEntries(headers.map((h,i)=>[h,row[i]??null]).sort((a,b)=>a[0].localeCompare(b[0]))))
```

---

Prompt tokens: 51  
Code tokens: 18    
Efficiency total: 69  

Attempts: 16 
Your best: 100 points  
Submitted at 10:45 pm on 10th March  
#5 on Leaderboard with 1893 points  

---

## Prompt History

1. ```markdown
    **Goal:** Create a CSV Row to JSON Mapper
    **Constraints:** You MUST take header and rows array as input. Avoid white-spaces, write single-line arrow function
    **Edge Cases:** Handle empty rows
    **Output Format:** It should return array of object
    ```

2. ```markdown
    **Goal:** Create a CSV Row to JSON Mapper
    **Constraints:** You MUST take header and rows array as input, sort headers alphabatically. Avoid white-spaces, write single-line arrow function
    **Edge Cases:** Handle empty rows
    **Output Format:** It should return array of object
    ```

3. ```markdown
    **Goal:** Create a CSV Row to JSON Mapper
    **Constraints:** You MUST take header and rows array as input, sort headers alphabatically. Avoid white-spaces, write single-line arrow function
    **Edge Cases:** Handle empty rows
    **Output Format:** It should return array of objects
    ```

4. ```markdown
    **Goal:** Create a CSV Row to JSON Mapper
    **Constraints:** You MUST take header and rows array as input. Avoid white-spaces, write arrow-function
    **Edge Cases:** Handle empty rows
    **Output Format:** It should return array of objects, sorted alphabetically
    ```

5. ```markdown
    Goal: Create a CSV Row to JSON Mapper
    Constraints: You MUST take header and rows array as input. Avoid white-spaces, write arrow-function
    Edge Cases: Handle empty rows
    Output Format: It should return array of objects, sorted alphabetically
    ```
