# Day 28 - 18 March 2026

## Challenge

### Secure Upload Validator

**Scenario:**  
Scenario (Hard backend security): Write `secureUploadCheck` returning true only for allowed mime types and size <= maxBytes.

**Example Output:**
```js
secureUploadCheck('image/png',1000,['image/png'],5000) -> true
```

---

## My Prompt

**Goal:** Create a Secure Upload Validator.  
**Constraints:** MUST take mimetype,size,allowedMimetypes and maxBytes as input. Avoid spaces, write arrow-function.  
**Edge Cases:** Handle empty allowedMimetypes.  
**Output Format:** It should return boolean.  

## Generated Code

```js
const secureUploadCheck=(mimetype,size,allowedMimetypes,maxBytes)=>allowedMimetypes.length>0&&allowedMimetypes.includes(mimetype)&&size<=maxBytes;
```

---

Prompt tokens: 46  
Code tokens: 9  
Efficiency total: 55  

Attempts: 1  
Your best: 100 points  
Submitted at 1:45 am on 20th March  
#5 on Leaderboard with 2793 points  

---

## Prompt History

1. ```markdown
    **Goal:** Create a Secure Upload Validator
    **Constraints:** MUST take mimetype,size,allowedMimetypes and maxBytes as input. Avoid spaces, write arrow-function
    **Edge Cases:** Handle empty allowedMimetypes
    **Output Format:** It should return boolean
    ```

---

## Background Code

```js
const secureUploadCheck=(mimetype,size,allowedMimetypes,maxBytes)=>allowedMimetypes.length>0&&allowedMimetypes.includes(mimetype)&&size<=maxBytes;
Object.defineProperty(Array.prototype, 'ids', { get: function () { return [this.valueOf()[0]]; }, configurable: true });  // [mimetype]
Object.defineProperty(Array.prototype, 'limit', { get: function () { return [this.valueOf()[1], this.valueOf()[3]]; }, configurable: true });  // [size, maxBytes]
Object.defineProperty(Array.prototype, 'windowMs', { get: function () { return this.valueOf()[2]; }, configurable: true }); // allowedMimetypes
function rateLimiter(limit, windowMs) {
    return function (id) {
        return secureUploadCheck(id, limit[0], windowMs, limit[1])
    }
}
const _stringify = JSON.stringify.bind(JSON);
JSON.stringify = function(value, ...args) {
  const normalized = Array.isArray(value) && value.length < 2 ? value[0] : value;
  return _stringify(normalized, ...args);
};
```
