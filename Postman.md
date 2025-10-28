## Postman Interview Experience

### Role Information

- **Position:** Senior Frontend Engineer
- **Application Date:** September 2024
- **Application Method:** Applied through Career Site
- **Total Rounds:** 4

---

## Round 1: Engineering Manager Round

**Duration:** 60 minutes

**Questions Asked:**

1. **Introduction and Background**

   - Current projects and work experience
   - Tech stack worked on in the past

2. **Promise Implementation from Scratch**

   - Implement a custom Promise constructor
   - Chaining was not required, but explain how it would be implemented
   - Implementation should support basic `.then()` and `.catch()` functionality

   **My Implementation:**

   ```javascript
   function MyPromise(executor) {
     let onResolve; // callback for resolve
     let onReject; // callback for reject
     let isFulfilled = false; // whether the promise has been resolved
     let isRejected = false; // whether the promise has been rejected
     let isCalled = false; // to prevent calling handlers multiple times
     let value; // store resolved value
     let error; // store rejected error

     // Called when executor calls resolve()
     function resolve(val) {
       isFulfilled = true;
       value = val;
       // If a .then handler is already attached, call it
       if (typeof onResolve === "function" && !isCalled) {
         onResolve(val);
         isCalled = true;
       }
     }

     // Called when executor calls reject()
     function reject(err) {
       isRejected = true;
       error = err;
       // If a .catch handler is already attached, call it
       if (typeof onReject === "function" && !isCalled) {
         onReject(err);
         isCalled = true;
       }
     }

     // Register a handler for success
     this.then = function (thenHandler) {
       onResolve = thenHandler;
       // If already resolved earlier, call handler immediately
       if (!isCalled && isFulfilled) {
         onResolve(value);
         isCalled = true;
       }
       return this; // allow chaining
     };

     // Register a handler for error
     this.catch = function (catchHandler) {
       onReject = catchHandler;
       // If already rejected earlier, call handler immediately
       if (!isCalled && isRejected) {
         onReject(error);
         isCalled = true;
       }
       return this; // allow chaining
     };

     // Immediately execute the executor with resolve and reject
     executor(resolve, reject);
   }

   // Test cases
   const newPromise = new MyPromise((resolve, reject) => {
     setTimeout(() => {
       resolve("Saumyadip");
     }, 1000);
   });

   const newPromise2 = new MyPromise((resolve, reject) => {
     resolve("Saumyadip");
   });

   newPromise.then((val) => {
     console.log(val);
   });

   newPromise2.then((val) => {
     console.log(val);
   });
   ```

3. **React Timer Implementation**
   - Implement a timer functionality in CodeSandbox using React
   - Three buttons: START, PAUSE, RESET
   - Display timer in HH:MM:SS format

---

## Round 2: Frontend Technical Round

**Duration:** 60 minutes

**Questions Asked:**

1. **Web Security Concepts**

   - Cross-Site Scripting (XSS)
   - Content Security Policy (CSP)
   - Cross-Origin Resource Sharing (CORS)

2. **Polyfill Implementation**

   - Implement polyfill for `getElementsByClassName`
   - Problem link: https://www.greatfrontend.com/questions/javascript/get-elements-by-class-name
   - **Status:** Could not solve it even after hints

3. **Browser APIs**

   - What are Mutation Observers?
   - Use cases and implementation (Could not answer properly)

4. **Data Structures & Algorithms**

   - Solve the "Number of Islands" problem
   - Problem link: https://leetcode.com/problems/number-of-islands/description/

5. **Asynchronous Programming**

   - Question similar to implementing `mapAsync`
   - Reference: https://www.greatfrontend.com/questions/javascript/map-async
   - **Note:** Interviewer had slightly modified the original question

6. **Performance Optimization**
   - How do you manage performance when rendering 1000+ items?
   - Expected discussion on virtualization, pagination, lazy loading, etc.

---

## Round 3: System Design

**Duration:** 60 minutes

**Interviewer:** Senior Engineer from UK

**Problem:** Design a chat application like Slack

**Topics Covered:**

1. **Communication Protocols**

   - Which protocols to use (WebSockets, HTTP, etc.)
   - Real-time communication strategy

2. **State Management**

   - How to manage application state
   - Message synchronization across clients

3. **Component Design**

   - Component architecture
   - Reusable component patterns

4. **Accessibility**

   - ARIA labels and keyboard navigation
   - Screen reader compatibility

5. **Performance**
   - Message rendering optimization
   - Lazy loading and virtualization
   - Caching strategies

## Overall Experience

**Result:** Rejected after Round 3

The interview process was challenging and covered a comprehensive range of topics. Round 1 went well with successful implementation of Promise from scratch and the timer functionality. However, Round 2 had some difficulties:

- Could not solve the `getElementsByClassName` polyfill even with hints
- Struggled with one other question

Round 3 (System Design) did not go as well as expected. The accent barrier created some initial communication challenges, and the overall discussion could have been more thorough. Given the performance in Rounds 2 and 3, the rejection was expected.
