# Day 18 - 8 March 2026

## Challenge

### Theme Preference Resolver

**Scenario:**  
Scenario (Frontend Tailwind): Write `themePreference` that chooses user preference if valid (`light`/`dark`), otherwise fallback to system preference.

**Example Output:**
```js
themePreference('dark','light') -> 'dark'
```

---

## My Prompt

**Goal:** Create a Theme Preference Resolver.  
**Constraints:** You MUST take userTheme and systemTheme as input. Avoid white-spaces, write single-line arrow function.  
**Edge Cases:** Handle invalid userTheme, use systemTheme.  
**Output Format:** It should return "light" or "dark" theme.  

## Generated Code

```js
const themePreference=(userTheme,systemTheme)=>(userTheme==="light"||userTheme==="dark")?userTheme:systemTheme
```

---

Prompt tokens: 57  
Code tokens: 9    
Efficiency total: 66  

Attempts: 1 
Your best: 100 points  
Submitted at 10:10 pm on 10th March  
#5 on Leaderboard with 1793 points  

---

## Prompt History

1. ```markdown
    **Goal:** Create a Theme Preference Resolver
    **Constraints:** You MUST take userTheme and systemTheme as input. Avoid white-spaces, write single-line arrow function
    **Edge Cases:** Handle invalid userTheme, use systemTheme
    **Output Format:** It should return "light" or "dark" theme
    ```
