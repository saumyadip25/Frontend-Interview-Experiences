# Interview Experience

# Role - Senior Software Engineer Frontend

## Round 1 - TPI

**Duration:** 75 minutes

### 1. Project Discussion

Can you explain about the most challenging project you have worked upon? What were the challenges you faced and how did you resolve them?

### 2. DSA Question - Balanced Brackets

You are given a string with characters and brackets. Tell whether the string is balanced or not.

**Examples:**

- `((abd))` - Balanced
- `)(())abc` - Not balanced
- `{{[abcfGHTY]()UUffU}}` - Balanced

### 3. DSA Question - Connected Graph

How would you check if a graph is connected or not? Meaning if all vertices can be visited from a particular vertex. It's based on connected components or union find (graph component).

### 4. JavaScript - Hoisting

Output based question on hoisting:

```javascript
const func1 = () => console.log(1);
func1();
func2();
function func2() {
  console.log(2);
}
func3();
var func3 = function func4() {
  console.log(3);
};
```

### 5. JavaScript - Promises

Output based question on promises:

```javascript
console.log(1);
const promise = new Promise((resolve) => {
  console.log(2);
  resolve();
  console.log(3);
});
console.log(4);
```

### 6. JavaScript - Closures

What are closures? What are the applications of it? (data encapsulation, currying, module pattern, etc.)

### 7. Web Security

What do you mean by web security? Explain CORS, XSS, CSRF, Man in the Middle attacks. Explain how to fix these web vulnerabilities.

### 8. React - Performance Optimization Hooks

Difference between `useMemo`, `useCallback`, and `memo`

### 9. React - State Management

What are Context APIs? Difference between Context and Redux. How Redux gives better performance.

### 10. AI Tools for Coding

What AI tools do you use for coding? Follow-up: Write a prompt for a given component (accordion component).

### 11. Web Accessibility

What are web accessibility standards? How to improve web accessibility?

## Round 2 - With 2 SSE, 1 Staff Engineer, 1 EM

**Duration:** 90 minutes

### Preparation

I was given a GitHub codebase one day prior to this round: https://github.com/Intuit-A4A/frontend-page-prism?tab=readme-ov-file. Required to go through the codebase, follow the readme.md file, and complete the setup.

**1. Nested Comment Component**

- Implement a nested comment component in the above codebase. Follow same patterns.
- Store state data in IndexedDB.
- The codebase had utility methods to insert and update IndexedDB data.
- Test skills to understand and work with a new codebase.

**2. Typeahead Component**

- Implement a simple typeahead component in same codebase.
- Successfully coded the component quickly.
- Follow-up: Write unit tests using Jest/React Testing Library (Could not complete the unit tests due to lack of proper practice).

## Round 3 - With 2 SSE

**Duration:** 60 minutes

### 1. JavaScript - Promise Retry Function

Implement a retry function that takes a promise-returning function and retries it a specified number of times with a delay between retries if it fails.

I coded this:

```javascript
function retry(fn, retries = 3, delay = 1000) {
  return new Promise((resolve, reject) => {
    function attempt(attemptsLeft) {
      fn()
        .then(resolve)
        .catch((error) => {
          if (attemptsLeft === 0) {
            reject(error);
          } else {
            console.log(`Attempt failed. Retries left: ${attemptsLeft}`);
            setTimeout(() => {
              attempt(attemptsLeft - 1);
            }, delay);
          }
        });
    }

    attempt(retries);
  });
}
```

### 2. Web Security

I was asked lot of questions on web security based on the code I had done in Round 2. Topics covered:

- XSS (Cross-Site Scripting)
- CSRF tokens
- How to fix these vulnerabilities

### 3. JavaScript - Promise Methods

Difference between `Promise.race()` and `Promise.any()`. Also code the polyfill for `Promise.race()`.

### 4. Redux - State Management

Few questions about state management in Redux:

- Actions
- Reducers
- Initial State

## Round 4 - With Staff Engineer

**Duration:** 45 minutes

### 1. DOM Tree Comparison

Implement a function `identicalDOMTrees` that checks if two DOM trees are identical or not. The function takes two DOM nodes as the root nodes of two DOM trees and returns a boolean result.

```javascript
function compareAttributes(nodeA, nodeB) {
  const attrA = nodeA.attributes;
  const attrB = nodeB.attributes;

  if (attrA.length !== attrB.length) {
    return false;
  }

  for (let i = 0; i < attrA.length; i++) {
    const key = attrA[i].name;
    const value = attrA[i].value;
    if (nodeB.getAttribute(key) !== value) {
      return false;
    }
  }
  return true;
}

export default function identicalDOMTrees(nodeA, nodeB) {
  if (nodeA.nodeType !== nodeB.nodeType) {
    return false;
  }
  if (nodeA.nodeType === Node.TEXT_NODE) {
    if (nodeA.textContent === nodeB.textContent) {
      return true;
    }
    return false;
  }
  if (nodeA.tagName != nodeB.tagName) {
    return false;
  }

  if (!compareAttributes(nodeA, nodeB)) {
    return false;
  }

  const childrenA = nodeA.childNodes;
  const childrenB = nodeB.childNodes;

  if (childrenA.length !== childrenB.length) {
    return false;
  }

  for (let i = 0; i < childrenA.length; i++) {
    if (!identicalDOMTrees(childrenA[i], childrenB[i])) {
      return false;
    }
  }
  return true;
}
```

### 2. User Story - LLM Integration (Implement on Round 2 codebase)

As a user, I want to generate a text description that represents my inspiration/project and then displays it on the project details page.

**Scope:**

- Leverage provided LLM to query and generate a text description that represents an inspiration/project
- Handle any errors or unexpected outputs
- Add unit test: handle different cases of LLM output

**Experience:**
The interviewer expected to use Server-Sent Events (SSE) for communication protocol but I implemented it using native JavaScript. I got stuck and took help from online resources, which extended the interview to 55 minutes. I felt the interviewer did not like the native approach as it was very lengthy and complex to implement.

## Round 5 - With Engineering Manager

**Duration:** 30 minutes

### 1. Project Discussion

General discussion on the projects I had done. He gave me some feedback on Round 2 where he was also present.

### 2. Microfrontends

Asked about microfrontends and discussed it for 10 minutes.

- Pros and Cons of microfrontends
- How to implement it

### 3. Web Performance

He asked me lot of questions about:

- Web vitals
- Web optimization techniques
- What all things I have done in the past to optimize the performance of my app

### 4. Web Workers and Service Workers

Asked when to use web workers and service workers.

### 5. Product Demo

Then showed me the Intuit QuickBooks product which his team works on.

# Overall Experience

- The interview experience was very good. I really liked the interviewers as they were calm, polite and collaborative.
- The final verdict was YES but I was offered a SWE-2 role (one level demotion).
- I was very tired because Round 2 to Round 5 happened on same day with a gap of 10 minutes.
- I think it was SWE-2 because:
  - I could not write the tests properly as I lost the practice after joining Fairmatic
  - In Round 4, I made a mistake which looked bad
  - I did not use Server-Sent Events (SSE) for the LLM based question
  - Based on the projects discussion, the EM thought I have not worked on scale and decided to offer me SWE-2 role so that I can grow there as an SSE
