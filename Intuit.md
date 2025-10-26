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

- What are closures?
- What are the applications of closures? (e.g., data encapsulation, currying, module pattern, etc.)

### 7. Web Security

- What do you mean by web security?
- Explain CORS, XSS, CSRF, Man in the Middle attacks
- Explain how to fix these web vulnerabilities

### 8. React - Performance Optimization Hooks

Difference between `useMemo`, `useCallback`, and `memo`

### 9. React - State Management

- What are Context APIs?
- Difference between Context and Redux
- How Redux gives better performance

### 10. AI Tools for Coding

- What AI tools do you use for coding?
- Follow-up: Write a prompt for a given component (accordion component)

### 11. Web Accessibility

- What are web accessibility standards?
- How to improve web accessibility?
