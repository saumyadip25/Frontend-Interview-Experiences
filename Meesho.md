# Meesho Interview Experience

## Role Information

- **Position:** SDE-3 (Frontend)
- **Application Date:** September 2025
- **Application Method:** Referral
- **Total Rounds:** 3 (Rejected after 2 rounds)

---

## Round 1: Tech Round (HTML+CSS+JS+React)

**Duration:** 90 minutes

### Questions Asked:

1. **Semantic HTML**

   - What is the use of semantic HTML?

2. **HTML Coding Challenge**

   - Shown a UI and had to code it using semantic HTML
   - Used tags: `header`, `nav`, `li`, `aside`, `main`, `button`, `footer`, `article`, etc.
   - Focus on good HTML knowledge (important for E-Commerce platform sites)

3. **CSS Display Properties**

   - Difference between block and inline-block elements

4. **Critical Rendering Path**

   - What is critical rendering path?
   - Why is CSS called render blocking?

5. **CSS Animations**

   - Difference between transition and animation (keyframes)?
   - Write a basic animation in JS Fiddle

6. **CSS Performance**

   - Different techniques to improve CSS performance
   - _(Reference: https://web.dev/ and w3schools)_

7. **FPS and GPU Acceleration**

   - What is FPS?
   - Why should we use `transform` instead of animating `width` and `height`?
   - _(Read about FPS and how transform is GPU accelerated)_

8. **Project Discussion**

   - Explain most challenging project

9. **Memoization Function**

   - Write a function that memoizes another function

   ```javascript
   function memoize(fn) {
     const cache = new Map();

     return function (...args) {
       const key = JSON.stringify(args);
       if (cache.has(key)) {
         return cache.get(key);
       }

       const result = fn.apply(this, args);
       cache.set(key, result);
       return result;
     };
   }
   ```

10. **Polyfills**

    - Write polyfill for `throttle`
    - Write polyfill for `filter`

11. **Event Loop Output**

    ```javascript
    console.log(4);

    promise
      .then(() => {
        console.log(5);
      })
      .then(() => {
        console.log(6);
      });

    console.log(7);
    ```

12. **Async/Await**

    - Question on async JavaScript
    - Rewrite using async/await
    - _(Question forgotten but was little complicated was able to solve with a hint)_

13. **Typeahead Component (15 minutes)**
    - Implement a typeahead component
    - Made a simple mistake that couldn't be debugged due to time constraints
    - Interview went over 90 minutes
    - Interviewer gave the answer, and implementation was completed
    - Very basic mistake that was frustrating to miss

---

## Round 2: Hiring Manager

**Duration:** 45 minutes

### Topics Covered:

1. **Introduction**

   - EM gave introduction
   - Asked about myself

2. **Project Discussion**

   - Explained past projects and work experiences
   - Discussed most challenging projects

3. **Micro-frontends**

   - Many questions about micro-frontends
   - What is Webpack Module Federation?
   - What happens if there's a React version mismatch between remote app and host app?

4. **System Design**
   - Design a config-driven UI
   - Backend config should determine UI layout (e.g., Swiggy uses config-driven UI)

### Outcome:

- **Result:** Not moving forward after Hiring Manager round

---

## Overall Experience

After Hiring Manager round I was told they are not going ahead with my profile.

I think because of following reasons:

1. In 1st round, I made a very simple mistake and could not debug it during the time.
2. I have not worked on scale. Like I have worked on B2B applications only. So this was a negative to the EM.
3. Also I have not worked on microfrontends, I was able to answer the questions but since I have not worked on them, it was a bad impression to the EM.
