# Day 20 - 10 March 2026

## Challenge

### JWT Payload Builder

**Scenario:**  
Scenario (Backend auth): Write `buildJwtPayload` returning `{sub,role,iat}` where iat is provided timestamp integer.

**Example Output:**
```js
buildJwtPayload('u1','student',1700000000) -> {sub:'u1',role:'student',iat:1700000000}
```

---

## My Prompt

**Goal:** Create a JWT Payload Builder.  
**Constraints:** You MUST take sub,role,iat as input. Avoid white-spaces, write arrow-function.  
**Edge Cases:** Handle missing vaules, use default.  
**Output Format:** It should return object in this order: {iat,sub,role}.  

## Generated Code

```js
const buildJwtPayload=(sub,role,iat)=>({iat:iat??Math.floor(Date.now()/1000),sub:sub??'',role:role??'user'})
```

---

Prompt tokens: 54  
Code tokens: 11  
Efficiency total: 65  

Attempts: 5  
Your best: 100 points  
Submitted at 11:10 pm  
#5 on Leaderboard with 1993 points  

---

## Prompt History

1. ```markdown
    **Goal:** Create a JWT Payload Builder
    **Constraints:** You MUST take sub,role,student as input. Avoid white-spaces, write arrow-function
    **Edge Cases:** Handle missing vaules, use default
    **Output Format:** It should return object of given input
    ```

2. ```markdown
    **Goal:** Create a JWT Payload Builder
    **Constraints:** You MUST take sub,role,iat as input. Avoid white-spaces, write arrow-function
    **Edge Cases:** Handle missing vaules, use default
    **Output Format:** It should return object of given input
    ```

3. ```markdown
    **Goal:** Create a JWT Payload Builder
    **Constraints:** You MUST take sub,role,iat as input. Avoid white-spaces, write arrow-function
    **Edge Cases:** Handle missing vaules, use default
    **Output Format:** It should return object in this order: {iat,role,sub}
    ```

4. ```markdown
    **Goal:** Create a JWT Payload Builder
    **Constraints:** You MUST take sub,role,iat as input. Avoid white-spaces, write arrow-function
    **Edge Cases:** Handle missing vaules, use default
    **Output Format:** It should return object in this order: {iat,sub,role}
    ```
