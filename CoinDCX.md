# CoinDCX Interview Experience

## Role Information

- **Position:** Senior Software Engineer (Frontend)
- **Application Date:** July 2024
- **Application Method:** Applied through Career Site
- **Total Rounds:** 4 (Completed 2)

---

## Round 1: JavaScript, CSS and React Fundamentals

**Duration:** 60 minutes

**1. Flatten a Nested Array**

Write a function to flatten a nested array structure.

**Problem:**

```javascript
// Input: [0, 1, [2, [3, 4]], 5]
// Output: [0, 1, 2, 3, 4, 5]
```

**2. CSS Specificity**

Explain what specificity means in CSS and how it determines which styles are applied when multiple rules target the same element. Discussed the specificity hierarchy (inline styles, IDs, classes, elements) and how browsers calculate specificity scores.

**3. CSS Render Blocking**

Explain why CSS is render-blocking and its impact on page performance. Discussed:

- How browsers construct the CSSOM (CSS Object Model)
- Why the browser waits for CSS to load before rendering
- Strategies to optimize CSS delivery and reduce render-blocking time

**4. Memoize a Function**

Implement a higher-order function that memoizes another function to cache its results based on input arguments.

**Solution:**

```javascript
function memoize(fn) {
  const cache = new Map();
  return function (...args) {
    const key = JSON.stringify(args);
    if (cache.has(key)) return cache.get(key);
    const result = fn.apply(this, args);
    cache.set(key, result);
    return result;
  };
}

function add(a, b) {
  return a + b;
}

const memoizedAdd = memoize(add);

console.log(memoizedAdd(2, 3)); // Computes and caches result
console.log(memoizedAdd(2, 3)); // Returns cached result
```

**5. Memoize an Async Function (Follow-up)**

After solving the basic memoization, the interviewer increased the complexity by asking me to memoize an async function that makes API calls.

**Problem:**

```javascript
// Async function to fetch user data with a query and search key.
// Uses a callback to return data after the fetch is complete.
async function getUserData(query, searchKey, callback) {
  fetch(`localhost:3000/get/users?query=${query}&key=${searchKey}`).then(
    (result) => {
      // Parse the JSON response
      return result.json().then((data) => {
        // Pass the result to the callback function
        callback(data);
      });
    }
  );
}

// Wrapping the async function with a memoization function
// This prevents duplicate API calls for same inputs
let memoFun = memoizeUserData(getUserData);

// Calling the memoized version — this will only make one API call for the same input
memoFun("test", 100, callback); // First call → API request happens
memoFun("test", 100, callback); // Second call → Result returned from cache (no API request)
```

The challenge here was to handle async operations, promises, and callbacks while maintaining a cache to prevent redundant API calls.

**6. JavaScript 'this' Context**

Predict the output of the following code:

```javascript
const obj = {
  a: 1,
  b() {
    return this.a;
  },
};
console.log(obj.b());
```

This tested understanding of JavaScript's `this` binding and how it works in different contexts (object method calls, arrow functions, etc.).

---

## Round 2: Machine Coding

**Duration:** 60 minutes

**Problem: Nested Comments System**

I was asked to implement a nested comment feature similar to what we see on Facebook or Reddit. The interviewer showed me a visual reference and provided the requirements. I had to implement the functionality of adding new comments, deleting comments and editing comments.

**Requirements:**

- Display comments in a hierarchical structure
- Support unlimited nesting levels (replies to replies)
- Implement adding new comments/replies
- Handle the UI rendering of nested structure

**My Approach:**

I understood that this problem required a recursive approach to render nested components, where each comment could have child comments that would be rendered using the same component recursively. However, I struggled to implement the complete solution during the interview time frame.

**Challenges Faced:**

- Time pressure made it difficult to think through the recursion logic clearly
- Handling state management for deeply nested comments
- Managing the UI structure for variable nesting depths

---

## Overall Experience

**Result:** Rejected after Round 2

I received a rejection email following the machine coding round. At that time, I wasn't adequately prepared for machine coding interviews, especially implementing complex UI components under time constraints.
