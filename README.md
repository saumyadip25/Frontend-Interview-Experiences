# Frontend Interview Preparation Guide

## HTML

Your fundamentals in HTML should be strong, especially understanding how and why to use semantic HTML. Be familiar with the different semantic tags such as `<header>`, `<aside>`, and `<footer>`. You may be asked to design a page layout using only native HTML, ensuring that it follows proper semantic structure and accessibility principles.

### Key Topics

- Difference between HTML elements such as `<div>`, `<span>`, and `<a>` (anchor tag)
- Understand the purpose and semantic differences between commonly used HTML elements
- When to use a `<div>` vs. a `<span>`
- The role of the `<a>` (anchor) tag for navigation and linking

### Resources

- https://www.w3schools.com/html/ (Go through important tags only)
- https://www.codewithharry.com/tutorial/html-home

---

## CSS

Your CSS fundamentals should be very strong. Many companies place significant emphasis on it. In my experience, I've been asked numerous CSS-related questions during interviews with companies like Meesho, Eightfold, ServiceNow, and Postman.

### Key Topics

- Selectors
- Positioning
- Units
- Display types
- Animations and transitions
- Modern layout techniques: Flexbox and CSS Grid
- CSS performance optimization techniques (CSS is render blocking)

**Note:** Companies prefer candidates who have a strong understanding of core CSS concepts rather than relying solely on frameworks or preprocessors like SASS or Tailwind CSS.

### Resources

- https://www.w3schools.com/css/
- https://www.w3schools.com/css/css_performance.asp
- CodeWithHarry CSS videos
- MDN CSS

---

## JavaScript

A strong grasp of JavaScript fundamentals is crucial and consistently evaluated in interviews across companies. It forms the core foundation for working with any framework or library, so mastering the basics is essential before diving into advanced concepts.

### Important JavaScript Topics

- Hoisting
- Asynchronous JavaScript (Promises, Async/Await, Event Loop)
- `this` keyword and its behavior
- Functions and Closures
- Currying
- Objects and their manipulation
- `call`, `apply`, and `bind` methods
- Event Propagation (capturing and bubbling)
- Debouncing and Throttling
- Prototypes and Inheritance
- Classes and Constructors
- Interview Patterns

### Interview Patterns

In many places you are asked output-based questions on JavaScript, so concepts should be very clear.

### Resources

- https://bigfrontend.dev/quiz (Solve output-based questions from start. Cover the important ones)
- Roadside Coder - https://learn.roadsidecoder.com/new-courses/1/content?activeTab=Content (JavaScript) [Paid course]
- Akshay Saini - Namaste Javascript Series [Free on YouTube]
- GreatFrontEnd's JavaScript questions: https://www.greatfrontend.com/questions/javascript-interview-questions
  - Start with Easy to build momentum
  - Progress to Medium to deepen understanding
  - Tackle a few Hard problems if time permits
- Cover important topics like polyfills for promise, promise APIs, `call`, `apply`, `bind`, `reduce`, `filter`, `some`, etc.
- https://javascript.info/ (Good source for JS fundamentals)
- https://www.youtube.com/@theavocoder (JS fundamentals)
- https://github.com/saumyadip25/Knowledge-Base (Important notes)

---

## Framework / Machine Coding

The machine coding round is designed to evaluate how efficiently you can live-code a given UI, task, or challenge within a limited time frame (typically 45 minutes to 1 hour). You can use any framework of your choice, such as React, Vue, or Angular.

### Key Focus Areas

- Writing modular, extensible, and maintainable code
- Effective time management
- Prioritize implementing core functionality first
- Focus on styling and polish only if time permits
- Evaluation is primarily based on functionality, code structure, and problem-solving approach

### Practice Approach

Practice these questions in CodeSandbox and try to solve them in 50 minutes like a real interview. For example: Build a N*N tic-tac-toe game.

### Resources

- https://learn.roadsidecoder.com/ (Machine Coding section)
- Roadside Coder YouTube channel
- Namaste System Design paid course by Akshay Saini
- Akshay Saini's YouTube platform (Free machine coding problems)
- https://devtools.tech/
- https://github.com/saumyadip25/Frontend-Machine-Coding
- https://www.greatfrontend.com/questions

**Note:** There are some problems which will overlap and you can skip them.

---

## System Design

The system design round is a crucial part of interviews for senior frontend roles. In this round, you typically don't need to write code, but you're expected to design the architecture and web view of complex systems based on the given problem.

### Fundamentals to Cover

Before diving into solving system design problems, strengthen your fundamentals:

- Communication protocols
- Databases
- Caching
- Offline support
- Other core concepts

Having a solid understanding of these will help you reason through trade-offs and design decisions confidently.

### Resources

- NamasteDev System Design course
- JS Café
- https://www.youtube.com/@DevtoolsTech
- https://namastedev.com/learn/namaste-frontend-system-design/hld-overview
- https://www.youtube.com/watch?v=5vyKhm2NTfw&list=PLI9W87-Dqn7j_x6QtR6sUjycJR7nQLBqT
- https://www.youtube.com/watch?v=sV_4pOGosnU&list=PL4CFloQ4GGWICE0Tz6iXKfN3XWkXRlboU
- https://frontendlead.com/system-design
- https://www.greatfrontend.com/front-end-system-design-playbook

### Practice Approach

Once you've covered the basics, start practicing problems on your own. Try designing the system first, perhaps on a whiteboard, before looking at others' solutions. This approach helps you deeply internalize the concepts and develop your own structured way of thinking.

---

## Miscellaneous Frontend / Other Topics

### Web Performance and Optimization

- Read about web vitals, optimization of HTML, JS, and CSS from https://web.dev/
- The above resource is the best resource available
- Try to read most of the topics from it
- If you have a NamasteDev System Design Course, go through all topics

### React Updates

- Read about recent hooks introduced in React 18 and React 19
- The interviewer might ask you if you have heard about them and how and where to use them

### Interview Experiences

- Try to search LeetCode interview experiences of frontend for different companies and practice them
- Practice 30 interview experiences from: https://study.learnyard.com/web/courses/6827a7b3101963b5e349142f?chapter=6828d1b55a77c2de8cb465ca

### Backend System Design

- Focus on backend system design at a high level
- Don't dive too deep right away
- Get comfortable with fundamentals like sharding, SQL vs. NoSQL trade-offs, and message queues
- Building this overview first will give you a strong foundation for designing robust systems

### Advanced Topics

- Read about micro-frontends and understand how they can be implemented using tools like Webpack Module Federation and Vite Module Federation
- Explore tutorials and explanations on Google and YouTube to get a practical understanding of how they work in real projects
- Read about web workers and service workers

### Project Experience

Be prepared with 3 different projects that you have worked upon in previous companies and the challenges you faced. You should explain this properly using the STAR framework.

---

## Data Structures and Algorithms

In many interviews during the online test or the initial rounds, you might face DSA questions.

### Key Points

- You should be comfortable solving problems in JavaScript or your preferred programming language
- In some interviews, especially for frontend roles, interviewers may specifically ask you to implement the solution in JavaScript
- Practice solving problems in both C++ and JavaScript to strengthen problem-solving skills and improve fluency in JavaScript

### Practice Approach

#### For Beginners

- Start by solving problems topic-wise
- Begin with easy ones and gradually move to medium-level problems to build a strong foundation
- Once you feel confident, start mixing problems from different topics to better mimic real interview scenarios

#### For Intermediate/Advanced

- Follow the NeetCode 150
- Regularly solve LeetCode Medium and Hard problems (typically 3 to 4 problems a day)
- Mix problems from different topics such as trees, dynamic programming, binary search, and graphs to stay well-rounded

### Interview Difficulty

- In most interviews, hard-level problems are rare
- Typically, you'll be asked medium to slightly hard questions
- Hard problems are usually seen in senior-level interviews at certain companies like PayPal, Quince, and Google

**Note:** In actual interviews, the topic isn't revealed, so you'll need to identify the concept behind the problem yourself. Practicing this way helps you develop the ability to recognize patterns and think analytically under pressure.

---

## Conclusion

This guide covers all the essential areas you need to prepare for frontend interviews. Focus on building strong fundamentals, practice consistently, and don't just memorize solutions but understand the underlying concepts. Good luck with your preparation!
