# Day 21 - 11 March 2026

## Challenge

### RBAC Permission Guard

**Scenario:**  
Scenario (Hard backend): Write `rbacCanAccess` returning true when role has permission using map `{role:[permissions...]}`.

**Example Output:**
```js
rbacCanAccess('admin','delete',map) -> true
```

---

## My Prompt

**Goal:** Create a RBAC Permission Guard.  
**Constraints:** You MUST take role,action,map as input. Avoid white-spaces, write arrow-function.  
**Edge Cases:** Handle empty map.  
**Output Format:** It should return true if role has permission to do action.  

## Generated Code

```js
const rbacCanAccess=(role,action,map)=>map[role]?.includes(action)??false
```

---

Prompt tokens: 54  
Code tokens: 7  
Efficiency total: 61  

Attempts: 1  
Your best: 100 points  
Submitted at 11:00 pm at 13th March  
#5 on Leaderboard with 2093 points  

---

## Prompt History

1. ```markdown
    **Goal:** Create a RBAC Permission Guard
    **Constraints:** You MUST take role,action,map as input. Avoid white-spaces, write arrow-function
    **Edge Cases:** Handle empty map,
    **Output Format:** It should return true if role has permission to do action
    ```
