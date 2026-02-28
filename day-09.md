# Day 09 - 27 Feb 2026

## Challenge

### Node.js File Stats

**Scenario:**  
Scenario (Node.js): Write `nodeFileStats` that returns `{lines,words}` for a text block.

**Example Output:**
```js
nodeFileStats('a b\nc d e') -> {lines:2,words:5}
```

---

## My Prompt

**Goal:** Create a Node.js File Stats tool.  
**Constraints:** You MUST use the input. Avoid white-spaces in code, write single-line arrow function.  
**Edge Cases:** Handle missing input and white-spaces.  
**Output Format:** It should return object with lines and words properties. 

## Generated Code

```js
const nodeFileStats=(t="")=>t.trim()?{lines:t.split("\n").length,words:t.trim().split(/\s+/).filter(w=>w).length}:{lines:0,words:0}
```

---

Prompt tokens: 59  
Code tokens: 16  
Efficiency total: 75  

Attempts: 1  
Your best: 100 points on first attempt  
Submitted at 7:55 am  
#7 on Leaderboard with 893 points  
