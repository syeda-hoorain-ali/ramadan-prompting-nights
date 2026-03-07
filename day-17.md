# Day 17 - 7 March 2026

## Challenge

### Full-Stack Notes Transformer

**Scenario:**  
Scenario (Next.js full stack): Write `notesApiTransform` converting note strings to objects `{id,text}` with incremental ids starting at 1.

**Example Output:**
```js
notesApiTransform(['a','b']) -> [{id:1,text:'a'},{id:2,text:'b'}]
```

---

## My Prompt

**Goal:** Create a Notes Transformer.  
**Constraints:** You MUST take array of string as input. **Avoid spaces in code**, write single-line arrow function.  
**Edge Cases:** Handle missing input, use default parameter.  
**Output Format:** It should return list of object with these fields: {id:1,text}.  

## Generated Code

```js
const notesApiTransform=(notes=[])=>notes.map((text,index)=>({id:index+1,text}))
```

---

Prompt tokens: 65  
Code tokens: 10  
Efficiency total: 75  

Attempts: 8 
Your best: 100 points  
Submitted at 10:55 pm  
#5 on Leaderboard with 1693 points  

---

## Prompt History

1. ```markdown
    **Goal:** Create a Notes Transformer
    **Constraints:** You MUST take array of string as input. Avoid white-spaces, write single-line arrow function
    **Edge Cases:** Handle missing input, use default parameter
    **Output Format:** It should return list of object with these fields: {id:1,text}
    ```

2. ```markdown
    **Goal:** Create a Notes Transformer
    **Constraints:** You MUST take array of string as input. **Avoid white-spaces**, write single-line arrow function
    **Edge Cases:** Handle missing input, use default parameter
    **Output Format:** It should return list of object with these fields: {id:1,text}
    ```

3. ```markdown
    **Goal:** Create a Notes Transformer
    **Constraints:** You MUST take array of string as input. **MUST Avoid white-spaces**, write single-line arrow function
    **Edge Cases:** Handle missing input, use default parameter
    **Output Format:** It should return list of object with these fields: {id:1,text}
    ```

4. ```markdown
    **Goal:** Create a Notes Transformer
    **Constraints:** You MUST take array of string as input. **Avoid white-spaces in code**, write single-line arrow function
    **Edge Cases:** Handle missing input, use default parameter
    **Output Format:** It should return list of object with these fields: {id:1,text}
    ```

5. ```markdown
    **Goal:** Create a Notes Transformer
    **Constraints:** You MUST take array of string as input. **Avoid spaces in code**, write single-line arrow function
    **Edge Cases:** Handle missing input, use default parameter
    **Output Format:** It should return list of object with these fields: {id:1,text}
    ```
