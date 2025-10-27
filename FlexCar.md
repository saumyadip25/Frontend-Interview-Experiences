# FlexCar Interview Experience

## Role Information

- **Position:** Senior Frontend Developer
- **Application Date:** September 2025
- **Application Method:** Applied through Career Site
- **Total Rounds:** 4

---

## Round 1: JavaScript and React Knowledge

**Duration:** 60 minutes

**1. Introduction and Project Discussion**

The interview began with a standard introduction followed by a detailed discussion about my previous projects and work experience.

**2. Custom Sort Implementation**

I was asked to implement a custom sorting function for an array of objects with specific sorting criteria.

**Problem:** Given an array of objects, sort them based on a primary key, and if values are equal, apply secondary sorting in descending order.

```javascript
let obj = [
  { a: 2, b: 2 },
  { a: 1, b: 1 },
  { a: 1, b: -1 },
];
// Sort by 'b' in ascending order
// If 'b' values are equal, sort by 'a' in descending order
```

**3. React useReducer Hook**

- What does the `useReducer` hook do?
- When should we use `useReducer` over `useState`?
- Discussion on state management patterns in React

**4. Redux vs React Context Performance**

Explained scenarios where Redux provides better performance compared to React Context API. Topics covered included:

- Re-rendering optimization
- Selector functions and memoization
- Context value splitting strategies
- Large-scale application state management

**5. Flatten a Nested Object**

Asked to write a function to flatten a deeply nested JavaScript object into a single-level object.

**Example:**

```javascript
let user = {
  name: "John",
  address: {
    country: "India",
    state: "India",
    education: {
      school: "APS",
      year: 2021,
    },
  },
};

// Expected output:
// {
//   name: 'John',
//   'address.country': 'India',
//   'address.state': 'India',
//   'address.education.school': 'APS',
//   'address.education.year': 2021
// }
```

---

## Round 2: Take Home Assignment

**Duration:** 2-3 days (assigned over weekend)

I was provided with a take-home coding assignment to be completed over the weekend. The assignment document contained detailed requirements for building a frontend application or component.

**Assignment Link:** [Google Docs Assignment](https://docs.google.com/document/d/1Ejg18tvUh31kCSQN2hdnsEC51kvMo8OXuQv9AT7Dux4/edit?tab=t.0)

I completed and submitted the assignment as per the requirements mentioned in the document, implementing all the requested features and functionalities.

---

## Overall Experience

**Result:** Rejected after Round 2

I received a rejection email following the submission of my take-home assignment. This was unexpected as I was informed that my Round 1 feedback was very positive.
I suspect the rejection might be related to AI tool usage during the assignment. I utilized AI assistance to complete the assignment efficiently, implementing exactly what was requested in the requirements. However, it's possible that:
