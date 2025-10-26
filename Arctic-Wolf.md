# Arctic Wolf Interview Experience

## Role Information

- **Position:** Senior Developer (UI)
- **Application Date:** September 2025
- **Application Method:** Referral
- **Total Rounds:** 5

---

## Round 1: JavaScript Fundamentals

**Duration:** 60 minutes

### Questions Asked:

1. **Closures**

   - Explain what closures are
   - Provide code examples

2. **Debounce and Throttle**

   - Implement debounce and throttle in vanilla JavaScript

3. **Promises**

   - Explain what promises are
   - Write a polyfill for `Promise.all()`

4. **Promise Chain Output**

   ```javascript
   Promise.resolve(1)
     .then((val) => {
       console.log(val);
       return val + 1;
     })
     .then((val) => {
       console.log(val);
     })
     .then((val) => {
       console.log(val);
       return Promise.resolve(3).then((val) => {
         console.log(val);
       });
     })
     .then((val) => {
       console.log(val);
       return Promise.reject(4);
     })
     .catch((val) => {
       console.log(val);
     })
     .finally((val) => {
       console.log(val);
       return 10;
     })
     .then((val) => {
       console.log(val);
     });
   ```

5. **'this' Keyword Behavior**

   ```javascript
   const obj = {
     dev: "bfe",
     a: function () {
       return this.dev;
     },
     b() {
       return this.dev;
     },
     c: () => {
       return this.dev;
     },
     d: function () {
       return (() => {
         return this.dev;
       })();
     },
     e: function () {
       return this.b();
     },
     f: function () {
       return this.b;
     },
     g: function () {
       return this.c();
     },
     h: function () {
       return this.c;
     },
     i: function () {
       return () => {
         return this.dev;
       };
     },
   };

   console.log(obj.a());
   console.log(obj.b());
   console.log(obj.c());
   console.log(obj.d());
   console.log(obj.e());
   console.log(obj.f()());
   console.log(obj.g());
   console.log(obj.h()());
   console.log(obj.i()());
   ```

6. **Event Loop and Microtasks**

   ```javascript
   console.log(1);
   const promise = new Promise((resolve) => {
     console.log(2);
     resolve();
     console.log(3);
   });

   console.log(4);

   promise
     .then(() => {
       console.log(5);
     })
     .then(() => {
       console.log(6);
     });

   console.log(7);

   setTimeout(() => {
     console.log(8);
   }, 10);

   setTimeout(() => {
     console.log(9);
   }, 0);
   ```

7. **var vs let in Loops**

   ```javascript
   for (var i = 0; i < 5; i++) {
     setTimeout(() => console.log(i), 0);
   }

   for (let i = 0; i < 5; i++) {
     setTimeout(() => console.log(i), 0);
   }
   ```

8. **Hoisting and Variable Scope**

   ```javascript
   var a = 1;

   function func() {
     a = 2;
     console.log(a);
     var a;
   }

   func();

   console.log(a);

   if (!("b" in window)) {
     var b = 1;
   }

   console.log(b);
   ```

9. **Array.prototype.reduce Polyfill**
   - Write a polyfill for the `reduce` method

---

## Round 2: Machine Coding

**Duration:** 60 minutes

### Main Task:

Build a **To-Do List Application** with the following requirements:

- Three filter tabs: Completed, In Progress, and Deleted
- Display tasks based on the selected filter
- Handle keyboard interactions (e.g., add new task on Enter key press)

### Additional Question (after early completion):

```javascript
Promise.resolve(1)
  .then(() => 2)
  .then(3)
  .then((value) => value * 3)
  .then(Promise.resolve(4))
  .then(console.log);
```

---

## Round 3: System Design

**Duration:** 60 minutes  
**Interviewer:** Lead Engineer

### Topics Covered:

1. **Project Discussion**

   - Detailed discussion about past projects

2. **Optimization Techniques**

   - Virtualization
   - Lazy loading
   - Write pseudo-code to implement virtualization with vanilla JavaScript using Intersection Observer

3. **React Performance**

   - React Profiler and its usage for performance optimization

4. **Architecture**
   - Micro-frontend architecture (theory knowledge)

---

## Round 4: Hiring Manager

**Duration:** 60 minutes  
**Interviewer:** Engineering Manager

### Topics Covered:

1. **Career Discussion**

   - Career journey and background

2. **System Design**

   - Message queues (despite UI-focused profile)
   - Role-based authentication application implementation
   - How to show pages based on user roles

3. **Behavioral Assessment**
   - Situational questions
   - Cultural fit questions

---

## Round 5: Final Tech Round

**Duration:** 60 minutes

> **Note:** Before this round, the recruiter informed that all rounds were cleared with positive feedback. Offer letter rollout was expected by Monday. However, on Monday, they scheduled one more round on design and coding.

### Topics Covered:

1. **Introduction and Project Discussion**

   - Explained migration from Gatsby to React at Fairmatic
   - Follow-up questions on design choices
   - Collaboration with Manager, Junior Developers, and Product Managers

2. **React Coding Challenge**
   - Question based on async behavior
   - Misunderstood the question and coded a complex solution (which was working)
   - Interviewer asked for a simpler solution, which I could not implement during the interviewer

### Outcome:

- **Feedback:** "Do Not Proceed"
- **Result:** Rejected

---

## Overall Experience

The overall experience after 4 rounds were okayish. But 5th round was not good as per feedback. I got "Do Not Proceed" feedback in 5th round due to which I got rejected. The 5th round interviewer gave a very bad feedback actually which I was very surprised because I gave a complex solution for a simple solution. This made me sad and I was frustrated because I was told that Hiring Manager liked me and they will roll out offer letter soon and then in 5th round which was not excellent I was rejected.

