# Day 06 - 24 Feb 2026

## Challenge

### Next.js Health Payload
**Scenario:**

Scenario (Next.js API): Write `apiHealthPayload` that returns `{status:'ok',service,version}`.

**Example Output:**
```js
apiHealthPayload('ramadan-api','1.0.0') -> {status:'ok',service:'ramadan-api',version:'1.0.0'}
```

---

## My Prompt

**Goal:** Create a Health API Payload Generator  
**Constraints:** You MUST take service and version as input. Avoid white-spaces and write single-line arrow function.  
**Edge Cases:** Handle missing version. If not provided, use '1.0.0'  
**Output Format:** It should return object containing status, service and version  

## Generated Code

```js
const apiHealthPayload=(service,version)=>({status:'ok',service,version:version||'1.0.0'})
```

---

Prompt tokens: 67  
Code tokens: 10  
Efficiency total: 77  

Attempts: 1  
Your best: 100 points on first attempt  
Submitted at 10:20 pm  
#4 on Leaderboard with 593 points  
