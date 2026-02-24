# Day 05 - 23 Feb 2026

## Challenge

### React Card Prop Merger
**Scenario:**

Scenario (React): Write `mergeCardProps` to merge default and custom props. Custom values override defaults.

**Example Output:**
```js
mergeCardProps({title:'Day 1',badge:'Easy'},{badge:'Done'}) -> {title:'Day 1',badge:'Done'}
```

---

## My Prompt

**Goal:** Create a React Card-Props Merger  
**Constraints:** You should merge the input, custom values MUST take priority. Avoid white-spaces, write single-line arrow function.  
**Edge Cases:** Handle empty objects. If no custom props, return default  
**Output Format:** The final output is the merged object.  

## Generated Code

```js
const mergeCardProps=(defaults={},custom={})=>({...defaults,...custom})
```

---

Prompt tokens: 65  
Code tokens: 10  
Efficiency total: 75  

Attempts: 1  
Your best: 100 points on first attempt  
Submitted at 8:15 am  
#4 on Leaderboard with 493 points  
