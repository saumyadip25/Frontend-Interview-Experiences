# MakeMyTrip Interview Experience

## Role Information

- **Position:** Senior Software Engineer-1 (Frontend)
- **Application Date:** July 2024
- **Application Method:** Recruiter Reached out through LinkedIn
- **Total Rounds:** 3

---

## Round 1: Frontend Fundamentals

**Duration:** 60 minutes

**1. Deep Object Equality**

Write a function to check if two objects are deep equal, handling nested objects and arrays.

**2. React Design Patterns**

Explain different React patterns you know and implement:

- Higher-Order Component (HOC) pattern with example
- Render Props pattern with example

**3. Core Web Vitals**

Explain what Core Web Vitals are and their importance (LCP, FID, CLS).

**4. Web Performance Optimization**

List different ways of improving the performance of a web application, including code splitting, lazy loading, caching, image optimization, etc.

**5. memo vs useMemo**

Explain the difference between `React.memo` and `useMemo` hook and when to use each.

**6. useTransition and useLayoutEffect**

Explain what `useTransition` and `useLayoutEffect` hooks do. (Could not answer this question)

---

## Round 2: Machine Coding + Frontend Fundamentals

**Duration:** 60 minutes

**1. Counter App Implementation (20 minutes)**

Create a counter application with three buttons:

- **Start:** Begins counting every second
- **Stop:** Pauses the count
- **Reset:** Sets counter to zero

**2. Hydration in SSR**

Explain what hydration means in Server-Side Rendering and how it works.

**3. ARIA Labels**

Explain what ARIA labels are used for and their importance in web accessibility.

**4. Breadcrumb Trail Construction**

Given a flat list of objects with `id`, `parentId`, and `title`, construct the breadcrumb trail from root to target.

**Input:**

```javascript
const breadCrum = [
  { id: 3, parentId: 12, title: "Headphones" },
  { id: 19, parentId: 28, title: "True wireless" },
  { id: 28, parentId: 3, title: "Wired" },
  { id: 12, parentId: null, title: "Audio" },
  { id: null, parentId: 19, title: "Bluetooth" },
];
```

**Expected Output:** `"Audio >> Headphones >> Wired >> True wireless >> Bluetooth"`

**5. Event Loop - Output Prediction**

Predict the order of output and explain why:

```javascript
console.log("start");

const promise1 = Promise.resolve().then(() => {
  console.log("promise1");
  setTimeout(() => console.log("timer1"), 0);
});

setTimeout(() => {
  console.log("timer2");
  Promise.resolve().then(() => console.log("promise2"));
}, 0);

console.log("end");
```

**Output:** `start, end, promise1, timer2, promise2, timer1`

**6. Array.sort() Behavior**

Explain the sorting behavior of `Array.sort()` with edge cases like `[1, null, 5, 2, undefined]`. Discuss how JavaScript handles null, undefined, and number comparisons in default sorting.

---

## Round 3: Engineering Manager Round

**Duration:** 60 minutes

**1. Background and Journey**

Discussed my work experience at Zendrive and my journey in frontend development.

**2. React Portals**

Explain what React Portals are and when to use them (rendering children outside parent DOM hierarchy).

**3. System Design - E-Commerce Website**

Design a scalable, performant e-commerce platform with the following features:

**Core Features:**

- Product listing and detail pages
- Shopping cart functionality
- Checkout flow
- Order tracking system
- User authentication (login/signup, sessions)
- Admin dashboards

**Design Considerations:**

- Scalability and performance
- State management approach
- API design
- Caching strategies
- Database schema
- Microservices vs monolithic architecture

**4. Cultural Fit Questions**

- Why do you want to join MakeMyTrip?
- Team collaboration and conflict resolution
- Handling pressure and deadlines

---

## Overall Experience

The overall experience was decent, and I felt the interviews went reasonably well. I was confident about my performance and expected a positive outcome. However, to my surprise, I received a rejection email after 2 days.
I reached out to the HR for feedback to understand what went wrong, but unfortunately received no response.
