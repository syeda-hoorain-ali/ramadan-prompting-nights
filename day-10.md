# Day 10 - 28 Feb 2026

## Challenge

### FastAPI Route Manifest

**Scenario:**  
Scenario (Python/FastAPI): Write `fastapiRouteMap` that returns an array of route objects from names list using GET method.

**Example Output:**
```js
fastapiRouteMap(['health','users']) -> [{path:'/health',method:'GET'},{path:'/users',method:'GET'}]
```

---

## My Prompt

**Goal:** Create a FastAPI Route Manifest Builder.  
**Constraints:** You MUST take list of pathnames as input. Avoid white-spaces, write single-line arrow function.  
**Edge Cases:** Handle empty and missing list, use default parameter.  
**Output Format:** It should return list of object: `{path:'/{name}',method:'GET'}` .  

## Generated Code

```js
const fastapiRouteMap=(names=[])=>names.map(name=>({path:`/${name}`,method:'GET'}))
```

---

Prompt tokens: 66  
Code tokens: 11  
Efficiency total: 77  

Attempts: 1  
Your best: 100 points on first attempt  
Submitted at 8:40 am  
#4 on Leaderboard with 993 points  
