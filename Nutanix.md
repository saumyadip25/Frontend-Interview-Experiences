# Nutanix Interview Experience

## Role Information

- **Position:** MTS-2 (Frontend)
- **Application Date:** June 2024
- **Application Method:** Applied through Career Site
- **Total Rounds:** 3 (Completed 1)

---

## Round 1: Frontend Fundamentals

**Duration:** 60 minutes

**1. Hoisting in JavaScript**

Explain what hoisting is in JavaScript with examples. Also explain the concept of Temporal Dead Zone (TDZ).

**2. Event Delegation**

What do you mean by Event delegation? Explain how it works with event bubbling and its benefits.

**3. Closures in JavaScript**

Explain what closures are in JavaScript with examples.

**4. Output Prediction - setTimeout with var**

What will be the output of below code and explain why:

```javascript
for (var i = 0; i < 5; i++) {
  setTimeout(() => {
    console.log(i);
  }, i * 1000);
}
```

The output will be `5` printed five times. This happens because `var` is function-scoped, and all setTimeout callbacks reference the same `i` variable which becomes 5 after the loop completes.

**5. Event Loop in JavaScript**

Explain the JavaScript Event Loop, including microtask queue and macrotask queue. Discuss how promises and setTimeout are handled differently.

**6. Output Prediction - Event Loop**

Predict the output of below code and explain why:

```javascript
console.log(1);

setTimeout(() => console.log(2));

Promise.resolve().then(() => console.log(3));

Promise.resolve().then(() => setTimeout(() => console.log(4)));

Promise.resolve().then(() => console.log(5));

setTimeout(() => console.log(6));

console.log(7);
```

**7. React - forwardRef and Suspense**

Explain the use of `forwardRef` and `Suspense` in React:

- **forwardRef:** Used to pass refs through components to child elements
- **Suspense:** Used for handling loading states while lazy loading components or fetching data

**8. Progress Bar Implementation**

Implement a progress bar in React on CodeSandbox with these requirements:

- Progress should complete to 100% in 5000ms
- Display completion percentage
- Should be scalable and reusable

---

## Overall Experience

**Result:** Rejected after Round 1

This was my first frontend interview experience, and it did not go well. I gave the interview without proper preparation and struggled with articulating my answers clearly. Even though I understood the concepts, I couldn't find the right words to explain my thinking process.
This rejection taught me the importance of preparation and communication skills. After this experience, I focused on studying JavaScript fundamentals in depth and practiced explaining concepts clearly, which significantly improved my performance in subsequent interviews.
