# 🌙 Ramadan Prompting Nights

My personal submission journal for [Sir Asharib Ali's](https://github.com/asharibali) [**Ramadan Prompting Nights**](https://github.com/AsharibAli/ramadan-prompting-nights/) challenge — 30 nights, 30 real-world coding scenarios, completed 30/30.

<div align="center">

### 🏆 4th Place &nbsp;|&nbsp; 2993 / 3000 Points &nbsp;|&nbsp; 30 / 30 Completed

**[🎓 Verify Certificate → RPN-5SRH-JGJJ](https://prompting.asharib.xyz/verify?id=RPN-5SRH-JGJJ)**

*Certificate issued by Asharib Ali (Creator of RPN) · March 22, 2026*

</div>

---

## 🧩 What Is This Challenge?

Every night at **10 PM PKT** throughout Ramadan 2026, a new coding scenario unlocked on the platform. The goal was **not** to write code directly — but to write a structured AI prompt precise enough that an LLM would generate a correct and efficient JavaScript function that passed hidden test cases.

**30 nights. 30 challenges. One prompt per night.**

---

## 📊 My Results

| Stat | Value |
|---|---|
| 🏅 Final Rank | **#4 on Leaderboard** |
| 💯 Total Score | **2993 / 3000** |
| ✅ Completion | **30 / 30 days** |
| 🌙 Difficulty | Easy (Days 1–10) · Medium (11–20) · Hard (21–30) |
| 🔥 Streak | Perfect 100/100 from Day 3 onwards |

---

## 🧠 Scoring System

Each submission was scored out of **100 points** across three components:

| Component | Points | Criteria |
|---|---|---|
| **Prompt Quality** | 60 | All 4 required sections present (15 pts each) |
| **Prompt Depth** | +20 | Linear ramp, maxes out at ≥200 characters |
| **Specificity** | +20 | Keyword hits: `must` `should` `avoid` `handle` `return` `input` `output` |
| **Correctness** | 20 | Generated code passes all hidden test cases |
| **Efficiency** | 20 | Fewer tokens in generated code = higher score |

### Required Prompt Structure

```markdown
**Goal:** what the function should do
**Constraints:** rules the code must follow
**Edge Cases:** special inputs to handle
**Output Format:** exact return format expected
```

---

## 🔥 The Hard Days (21–30)

The final 10 days had a hidden layer of complexity — several challenges had a **mismatch between the API spec and the test runner**. The platform's test runner expected a completely different function signature than what the challenge description showed:

| Day | API Says | Runner Actually Tests |
|---|---|---|
| 22 | `revalidatePlan` | `curry` |
| 23 | `queueRetryPlan` | `promisePool` |
| 24 | `notificationBatch` | `LRUCache` class |
| 25 | `optimizeLeaderboardQueryPlan` | `EventEmitter` factory |
| 27 | `realtimeMergeState` | `buildTrie` + `search` |
| 28 | `secureUploadCheck` | `rateLimiter` closure |

Most students (including me at first) dropped off at Day 22 after repeatedly hitting `curry is not defined` errors. Cracking each of these required reading the actual test runner source code, understanding how the background code interacted with user submissions, and reverse-engineering what the runner truly expected — then crafting a prompt that generated exactly that.

---

## 📁 Structure

Each `day-XX.md` file contains:

- **Challenge** — the original scenario and problem statement
- **My Prompt** — the structured prompt I submitted
- **Generated Code** — the JavaScript function AI produced
- **Score Breakdown** — tokens, attempts, final score, leaderboard position at that point
- **Prompt History** — all attempts made that night
- **Background Code** — the hidden test harness (reverse-engineered)

---

## 📜 Certificate

```
CERTIFICATE OF COMPLETION
Issued to:   Syeda Hoorain Ali
Score:       2993 / 3000
Rank:        #4
Completed:   30 / 30
Date:        March 22, 2026
Issued by:   Asharib Ali (Creator of RPN)
ID:          RPN-5SRH-JGJJ
```

🔗 **[prompting.asharib.xyz/verify?id=RPN-5SRH-JGJJ](https://prompting.asharib.xyz/verify?id=RPN-5SRH-JGJJ)**

---
 
If you're a student who gave up on Day 22 — go back. The hard days aren't broken, they're just harder. Read the source code, understand the runner, and try again. Every day in this challenge is solvable.
 
*— Syeda Hoorain Ali · Ramadan 2026*
