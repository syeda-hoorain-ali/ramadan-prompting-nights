# Day 02 - 20 Feb 2026

## Challenge

### JavaScript Prayer Scheduler
**Scenario:**

Scenario (JavaScript): Write `nextPrayerIndex` that receives current minutes and sorted prayer minutes, returning index of the next prayer, or 0 for next day rollover.

**Example Output:**
```js
nextPrayerIndex(700,[300,600,900,1100]) -> 2
```

---

## My Prompt

**Goal:** Create a JavaScript function `nextPrayerIndex(currentMinutes: number, sortedPrayerMinutes: number[]) -> number` that will return the index of the next prayer, or zero for next day.

**Constraints:**
- The function MUST compare the input value against the minutes array provided
- The function should find the first item greater than the current minutes

**Edge Cases:** The function should handle the cases where the current time exceeds all listed points in the array, in this scenario return 0 for next day roll over. Avoid returning -1

**Output Format:** The final output from the function must be the index of next prayer

---

Prompt tokens: 141  
Code tokens: 42 
Efficiency total: 183  

Attempts: 3  
Your best: 94 points at first attempt  
Submitted at 9:54 pm  
