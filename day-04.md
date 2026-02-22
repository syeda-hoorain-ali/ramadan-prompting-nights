# Day 04 - 22 Feb 2026

## Challenge

### TypeScript Profile Label
**Scenario:**

Scenario (TypeScript mindset): Write `typedProfileSummary` to return `"<name> (<role>)"`. If role is missing, use `Student`.

**Example Output:**
```js
typedProfileSummary({name:"Aisha",role:"Mentor"}) -> "Aisha (Mentor)"
```

---

## My Prompt

**Goal:** Create a Profile Label Generator
**Constraints:** You MUST use the input object. Avoid white-spaces and write a single-line arrow function.
**Edge Cases:** Handle missing role. If not provided, use Student
**Output Format:** It should return `{name} ({role})`

## Generated Code

```js
const typedProfileSummary = ({name, role = "Student"}) => `${name} (${role})`
```

---

Prompt tokens: 60    
Code tokens: 19  
Efficiency total: 79 

Attempts: 1     
Your best: 100 points on first attempt 
Submitted at 11:10 pm  
#1 on Leaderboard with 393 points  
