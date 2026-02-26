# Day 08 - 26 Feb 2026

## Challenge

### PostgreSQL Insert Query Builder

**Scenario:**  
Scenario (PostgreSQL): Write `buildStudentsInsertSQL` that returns SQL insert string for one student row.

**Example Output:**
```js
buildStudentsInsertSQL(1,'Sara','sara@giaic.com') -> "insert into students (id,name,email) values (1,'Sara','sara@giaic.com');"
```

---

## My Prompt

**Goal:** Create a PostgreSQL Query Builder.  
**Constraints:** You MUST use input. Avoid white-spaces, write single-line arrow-function.  
**Edge Cases:** Handle missing values, use default parameters.  
**Output Format:** It should return: "insert into students (id,name,email) values (1,'Sara','sara@giaic.com');".  

## Generated Code

```js
const buildStudentsInsertSQL=(id=1,name='Unknown',email='unknown@default.com')=>`insert into students (id,name,email) values (${id},'${name}','${email}');`;
```

---

Prompt tokens: 59  
Code tokens: 21  
Efficiency total: 80  

Attempts: 1  
Your best: 100 points on first attempt  
Submitted at 10:45 pm  
#5 on Leaderboard with 793 points  
