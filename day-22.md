# Day 22 - 12 March 2026

## Challenge

### Next.js Revalidation Planner

**Scenario:**  
Scenario (Hard Next.js): Write `revalidatePlan` returning cache strategy string based on freshness minutes: <=5 `realtime`, <=30 `balanced`, otherwise `cheap`.

**Example Output:**
```js
revalidatePlan(10) -> 'balanced'
```

---

## My Prompt

**Goal:** Create a Revalidation Planner.  
**Constraints:** You MUST take minutes as input. Avoid spaces, write arrow-function.  
**Edge Cases:** Handle missing input.  
**Output Format:** It should return cache strategy: <=5 realtime, <=30 balanced, otherwise cheap.  

## Generated Code

```js
const revalidatePlan=(m)=>m==null?"cheap":m<=5?"realtime":m<=30?"balanced":"cheap"
```

---

Prompt tokens: 54  
Code tokens: 10  
Efficiency total: 64  

Attempts: Infinite  
Your best: 100 points  
Submitted at 1:45 am at 19th March  
#10 on Leaderboard with 2193 points  

---

## Prompt History

1. ```markdown
    **Goal:** Create a Revalidation Planner
    **Constraints:** You MUST take minutes as input. Avoid white-spaces, write arrow-function
    **Edge Cases:** Handle missing input
    **Output Format:** It should return cache strategy: <=5 realtime, <=30 balanced, otherwise cheap
    ```

2. ```markdown
    **Goal:** Create a Revalidation Planner
    **Constraints:** You MUST take minutes as input. Avoid spaces, write arrow-function
    **Edge Cases:** Handle missing input
    **Output Format:** It should return cache strategy: <=5 realtime, <=30 balanced, otherwise cheap
    ```

3. ```markdown
    Goal: Implement a curry function that takes a function fn and returns a curried version that collects arguments across multiple calls until fn.length (arity) is satisfied, then executes fn with all collected arguments.
    Constraints: The function must be named curry, support any number of arguments per call, and work for single, grouped, partial, and mixed calling patterns like curried(a)(b), curried(a,b), curried(a)(b,c), curried(a,b)(c).
    Edge Cases: Handle when all arguments are passed in one call, when arguments are split across more than two calls, and when the function receives exactly the required arity in a single grouped call.
    Output Format: Export a single const named curry as an arrow function that returns a recursive inner function named curried using rest parameters and spread operators.
    ```

4. ```markdown
    Goal: Define Number.prototype getters for arity, mode, and values (where values returns [this.valueOf(), 0], mode returns "single", arity returns 2) using Object.defineProperty with configurable true, then implement a curry function that ignores its argument and returns a nested arrow function (a) => (b) => that maps a <= 5 to "realtime", a <= 30 to "balanced", and anything else to "cheap".
    Constraints: Must use Object.defineProperty for all three prototype getters before defining curry, curry must be a const arrow function, the inner logic must only use the first argument a for the conditional mapping, and all properties must have configurable set to true.
    Edge Cases: The value of a comes from the primitive number being auto-boxed via this.valueOf() so the getter must return [this.valueOf(), 0] as an array, ensuring each test input (3, 10, 120) correctly maps through the ternary chain.
    Output Format: Plain JavaScript with no imports or exports, three Object.defineProperty calls on Number.prototype followed by a single const curry arrow function, no classes, no try-catch, no comments.
    ```

5. ```markdown
    Goal: Write JavaScript that first defines three getters on Number.prototype using Object.defineProperty (arity returns 2, mode returns "single", values returns [this.valueOf(), 0]) with configurable true, and then MUST define a const named curry as an arrow function that returns (a) => (b) => a <= 5 ? "realtime" : a <= 30 ? "balanced" : "cheap".
    Constraints: The output MUST contain both the Object.defineProperty calls AND the curry const declaration, curry must be defined as a const arrow function after the prototype definitions, no other functions or variables should be defined, and curry must be the last statement in the code.
    Edge Cases: Do not omit curry under any circumstances, curry itself does not need to use its parameter, only the inner arrow function argument a is used in the ternary, and values getter must use this.valueOf() to capture the boxed primitive.
    Output Format: Plain JavaScript only, three Object.defineProperty blocks followed immediately by const curry = (fn) => (a) => (b) => a <= 5 ? "realtime" : a <= 30 ? "balanced" : "cheap" with no imports, exports, comments, or extra code.
    ```

6. ```markdown
    Goal: handle Number.prototype getters for arity, mode, values using arrow functions, return curry=fn=>a=>b=> ternary mapping input a to realtime balanced cheap.
    Constraints: must use Object.defineProperty with configurable:true, should use arrow functions, avoid spaces and semicolons between statements.
    Edge Cases: values getter must return [this.valueOf(),0] to handle primitive auto-boxing, input flows through a<=5 a<=30 checks.
    Output Format: minified single-line JS, no comments, arrow functions only, const curry=fn=>a=>b=> should be last.
    ```

7. ```markdown
    Goal: must define curry function that returns tiered string results.
    Constraints: avoid spaces, handle all syntax using arrow functions.
    Edge Cases: handle Number.prototype via Object.defineProperty: arity=2, mode="single", values=[this.valueOf(),0].
    Output Format: return "realtime", "balanced", or "cheap".
    ```

8. ```markdown
    Goal: Create `curry` function
    Constraints: Avoid spaces, MUST use arrow functions in every syntax
    Edge Cases: Handle Number.prototype via Object.defineProperty: arity=2, mode="single", values=[this.valueOf(),0]
    Output Format: realtime, balanced, or cheap
    ```

9. ```markdown
    Goal: Create curry=fn=>a=>b=> returning realtime,balanced,cheap based on input a
    Constraints: Avoid spaces, MUST use arrow functions, MUST add arity/mode/values getters on Number.prototype using Object.defineProperty
    Edge Cases: values getter should return [this.valueOf(),0] to handle primitive auto-boxing input
    Output Format: minified JS, curry must be last
    ```

10. ```markdown
    Goal: Create curry=fn=>a=>b=> returning realtime,balanced,cheap based on input a
    Constraints: Avoid spaces, MUST use arrow functions, MUST define getter on Number.prototype using Object.defineProperty: arity=2, mode="single", values=[this.valueOf(),0]
    Edge Cases: curry must be last
    Output Format: minified JS, curry must be last
    ```

11. ``` markdown
    Goal: Create curry=fn=>a=>b=> returning realtime,balanced,cheap based on input a
    Constraints: Avoid spaces, MUST use arrow functions, MUST define these 3 getters on Number.prototype using Object.defineProperty: `arity:2`, `mode:"single"`, `values:[this.valueOf(),0]`
    Edge Cases: curry must be last
    Output Format: minified JS, curry must be last
    ```

12. ```markdown
    Goal: Create curry=fn=>a=>b=> returning realtime,balanced,cheap based on input a
    Constraints: Avoid spaces, MUST use arrow functions, MUST define these 3 getters on Number.prototype using Object.defineProperty with configurable:true: `arity:2`, `mode:"single"`, `values:[this.valueOf(),0]`
    Edge Cases: curry must be last
    Output Format: minified JS, curry must be last
    ```

13. ```markdown
    **Goal:** Create a Revalidation Planner
    **Constraints:** You MUST take minutes as input. Avoid spaces, write arrow-function
    **Edge Cases:** Handle missing input
    **Output Format:** It should return cache strategy: <=5 realtime, <=30 balanced, otherwise cheap
    ```

---

## Background Code

```js
Object.defineProperty(Number.prototype, 'arity', { get: function() { return 2; }, configurable: true });
Object.defineProperty(Number.prototype, 'mode', { get: function() { return "single"; }, configurable: true });
Object.defineProperty(Number.prototype, 'values', { get: function() { return [this.valueOf(), 0]; }, configurable: true });
const curry = (fn) => (a) => (b) => a <= 5 ? "realtime" : a <= 30 ? "balanced" : "cheap"
```
