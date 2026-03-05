# Day 14 - 4 March 2026

## Challenge

### Leaderboard Rank Builder

**Scenario:**  
Scenario (PostgreSQL backend logic): Write `leaderboardRanks` that returns sorted entries with rank by ascending score.

**Example Output:**
```js
leaderboardRanks([{name:'A',score:40},{name:'B',score:20}]) -> [{name:'B',score:20,rank:1},{name:'A',score:40,rank:2}]
```

---

## My Prompt

**Goal:** Create a Leaderboard Rank Builder.  
**Constraints:** You MUST take the list of object as input. Avoid white-spaces, write single-line arrow function.  
**Edge Cases:** Handle missing input, use default parameter.  
**Output Format:** It should return list of object in this order: {name,rank,score}.  

## Generated Code

```js
const leaderboardRanks=(arr=[])=>[...arr].sort((a,b)=>a.score-b.score).map((e,i)=>({name:e.name,rank:i+1,score:e.score}))
```

---

Prompt tokens: 64  
Code tokens: 16  
Efficiency total: 80  

Attempts: 3  
Your best: 100 points  
Submitted at 9:05 pm  
#3 on Leaderboard with 1393 points  

---

## Prompt History

1. ```markdown
    **Goal:** Create a Leaderboard Rank Builder
    **Constraints:** You MUST take the list of object as input. Avoid white-spaces, write single-line arrow function
    **Edge Cases:** Handle missing input, use default parameter
    **Output Format:** It should return list of object in this order: {name,score,rank}
    ```

2. ```markdown
    **Goal:** Create a Leaderboard Rank Builder
    **Constraints:** You MUST take the list of object as input. Avoid white-spaces, write single-line arrow function
    **Edge Cases:** Handle missing input, use default parameter
    **Output Format:** It should return list of object in this order: {name,rank,score}
    ```
