# Kotak Bank Interview Experience

## Role Information

- **Position:** SDE-2 (Frontend)
- **Application Date:** August 2024
- **Application Method:** Applied through LinkedIn
- **Total Rounds:** 3

---

## Round 1: Frontend Fundamentals (Conducted by Bar Raiser [Third Party])

**Duration:** 60 minutes

**1. JavaScript Closures**

Explain what closures are in JavaScript, how they work, and provide practical use cases. Discussed lexical scoping, function scope, and how closures enable data privacy.

**2. CSS Position: Fixed vs Sticky**

Explain the difference between CSS `position: fixed` and `position: sticky`:

- Fixed: Element is removed from document flow and positioned relative to viewport
- Sticky: Element toggles between relative and fixed positioning based on scroll position

**3. Count Occurrences in Sorted Array**

Given a sorted array, find the count of a specific number using an optimized approach.

**Problem:**

```javascript
// Input: [2, 3, 4, 4, 4, 5, 10]
// Find count of 4
// Output: 3
```

**Approach:** Use binary search to find the first and last occurrence of the target number, then calculate count. Time complexity: O(log n).

**4. Polyfill for Promise.all()**

Implement a polyfill for the `Promise.all()` method that takes an array of promises and returns a single promise that resolves when all input promises have resolved.

**5. Custom useDebounce Hook in React**

Asked to implement a custom React hook for debouncing. Similar to this problem: [useDebounce on GreatFrontEnd](https://www.greatfrontend.com/questions/javascript/use-debounce)

**6. Core Web Vitals**

Explain what Core Web Vitals are and their importance:

- **LCP (Largest Contentful Paint):** Loading performance
- **FID (First Input Delay):** Interactivity
- **CLS (Cumulative Layout Shift):** Visual stability

Discussed how these metrics impact user experience and SEO rankings.

**7. Flexbox UI Implementation**

Given a reference UI design, recreate it using HTML and CSS on CodeSandbox. The layout was based on Flexbox properties. This was a straightforward implementation task testing practical CSS skills.

---

## Round 2: System Design + Frontend Fundamentals (Bar Raiser Round)

**Duration:** 60 minutes

**1. System Design: JIRA Clone (30 minutes)**

Asked to design a task management system similar to JIRA (Atlassian product).

**Design Requirements:**

- Component architecture and reusable components
- API design for CRUD operations
- State management approach

**API Design:**

- `POST /api/tasks` - Create new task
- `PUT /api/tasks/:id` - Update task
- `DELETE /api/tasks/:id` - Delete task
- `PATCH /api/tasks/:id/status` - Update task status
- `GET /api/tasks` - Fetch all tasks

**Component Structure:**

- TaskBoard (container)
- TaskColumn (for different status columns)
- TaskCard (individual task)
- TaskForm (create/edit task)
- TaskDetails (modal/drawer for task details)

Discussed state management, drag-and-drop functionality, real-time updates, and data flow between components.

**2. Polyfill for bind() Method**

Implement a polyfill for JavaScript's `bind()` method that creates a new function with a specific `this` context and optional preset arguments.

**3. Curry Function Implementation**

Asked to implement function currying in JavaScript. Similar to this problem: [Curry on GreatFrontEnd](https://www.greatfrontend.com/questions/javascript/curry)

**Example:**

```javascript
const add = (a, b, c) => a + b + c;
const curriedAdd = curry(add);

curriedAdd(1)(2)(3); // 6
curriedAdd(1, 2)(3); // 6
curriedAdd(1)(2, 3); // 6
```

---

## Round 3: Machine Coding and JavaScript Deep Dive (Senior Engineer Round)

**Duration:** 60 minutes

**1. File Explorer UI Implementation (30 minutes)**

Build a file/folder structure similar to VS Code's file explorer on CodeSandbox.

**Requirements:**

- Create nested folder structure
- Add files inside folders
- Files cannot contain other files/folders (leaf nodes)
- Implement delete functionality for both files and folders
- Recursive component structure

**2. Custom useThrottle Hook**

Implement a custom React hook for throttling function calls. Similar to debounce but ensures the function is called at most once in a specified time period.

**3. Event Loop and Async JavaScript**

Provide a detailed explanation of:

- JavaScript Event Loop mechanism
- Call Stack, Task Queue, and Microtask Queue

**4. Behavioral Questions**

- How do you handle conflicts in a team?
- How do you manage situations with high work pressure and tight deadlines?

---

## Overall Experience

**Result:** Cleared all technical rounds

After completing all three rounds, I received a call from the recruiter informing me that I had successfully cleared the technical rounds. She mentioned that she would reach out for salary negotiation discussions.
However, the recruiter never followed up for the salary discussion. By that time, I had already received an offer from another company and was not particularly interested in pursuing this opportunity further because Kotak had bad WLB and 90 days Notice period.
