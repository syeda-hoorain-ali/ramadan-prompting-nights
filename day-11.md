# Day 11 - 1 March 2026

## Challenge

### Signup Validation Engine

**Scenario:**  
Scenario (Frontend + TypeScript): Write `validateSignup` returning error array for missing name, invalid email, or password length < 8.

**Example Output:**
```js
validateSignup({name:'',email:'a',password:'123'}) -> ['name required','invalid email','password too short']
```

---

## My Prompt

**Goal:** Create a Javascript Signup Validation Engine.  
**Constraints:** You MUST take 'user' object as input. Avoid white-spaces, write single-line arrow function.  
**Edge Cases:** Handle missing values.  
**Output Format:** It should return: ['name required','invalid email','password too short']  

## Generated Code

```js
const validateSignup=(user)=>[!user?.name?'name required':'',!/@/.test(user?.email||'')?'invalid email':'',user?.password?.length>=8?'':'password too short'].filter(Boolean)
```

---

Prompt tokens: 58  
Code tokens: 21  
Efficiency total: 79  

Attempts: 1  
Your best: 100 points on first attempt  
Submitted at 7:06 am on 3rd March  
#7 on Leaderboard with 1093 points  

---

## Prompt History

1. ```markdown
    **Goal:** Create a Signup Validation Engine
    **Constraints:** You MUST take object as input. Avoid white-spaces, write single-line arrow function.
    **Edge Cases:** Handle missing values
    **Output Format:** It should return: ['name required','invalid email','password too short']
    ```

2. ```markdown
    **Goal:** Create a Signup Validation Engine
    **Constraints:** You MUST take user object as input. Avoid white-spaces, write single-line arrow function
    **Edge Cases:** Handle missing values
    **Output Format:** It should return: ['name required','invalid email','password too short']
    ```

3. ```markdown
    **Goal:** Create a Signup Validation Engine
    **Constraints:** You MUST take user object as input. Avoid white-spaces, write single-line arrow function
    **Edge Cases:** Handle missing values. Use regex
    **Output Format:** It should return: ['name required','invalid email','password too short']
    ```

4. ```markdown
    **Goal:** Create a Signup Validation Engine
    **Constraints:** You MUST take 'user' object as input. Avoid white-spaces, write single-line arrow function
    **Edge Cases:** Handle missing values
    **Output Format:** It should return: ['name required','invalid email','password too short']
    ```

5. ```markdown
    **Goal:** Create a Signup Validation Engine (Javascript)
    **Constraints:** You MUST take 'user' object as input. Avoid white-spaces, write single-line arrow function
    **Edge Cases:** Handle missing values
    **Output Format:** It should return: ['name required','invalid email','password too short']
    ```

6. ```markdown
    **Goal:** Create a Javascript Signup Validation Engine
    **Constraints:** You MUST take 'user' object as input. Avoid white-spaces, write single-line arrow function
    **Edge Cases:** Handle missing values
    **Output Format:** It should return: ['name required','invalid email','password too short']
    ```
