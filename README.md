# THINGS TO PREPARE BEFORE FRONTEND INTERVIEW

## HTML

Your fundamentals in HTML should be strong - especially understanding how and why to use semantic HTML. Be familiar with the different semantic tags such as `<header>`, `<aside>`, and `<footer>`. You may be asked to design a page layout using only native HTML, ensuring that it follows proper semantic structure and accessibility principles.

Difference between HTML elements such as `<div>`, `<span>`, and `<a>` (anchor tag). Understand the purpose and semantic differences between commonly used HTML elements for example, when to use a `<div>` vs. a `<span>`, and the role of the `<a>` (anchor) tag for navigation and linking.

**Resources -**
- https://www.w3schools.com/html/ (Go through important tags only)
- https://www.codewithharry.com/tutorial/html-home

## CSS

Your CSS fundamentals should be very strong, many companies place significant emphasis on it. In my experience, I've been asked numerous CSS-related questions during interviews with companies like Meesho, Eightfold, ServiceNow, and Postman.

Some of the key CSS topics to focus on include selectors, positioning, units, display types, animations, and transitions. Additionally, make sure to have a strong grasp of modern layout techniques like Flexbox, CSS Grid, and other advanced CSS concepts, as many companies specifically look for expertise in these areas. Covering all major topics will help you stay confident and well-prepared.

Also cover what techniques are used to optimise CSS performance since CSS is render blocking. [https://www.w3schools.com/css/css_performance.asp]

**Note -** Companies prefer candidates who have a strong understanding of core CSS concepts rather than relying solely on frameworks or preprocessors like SASS or Tailwind CSS.

**Resources -**
- W3school CSS
- CodeWithHarry CSS videos
- MDN CSS

## JAVASCRIPT

A strong grasp of JavaScript fundamentals is crucial and consistently evaluated in interviews across companies. It forms the core foundation for working with any framework or library, so mastering the basics is essential before diving into advanced concepts.

**Important JavaScript Topics (I may have missed a few, so make sure to cover everything thoroughly):**
- Hoisting
- Asynchronous JavaScript (Promises, Async/Await, Event Loop)
- this keyword and its behavior
- Functions and Closures
- Currying
- Objects and their manipulation
- call, apply, and bind methods
- Event Propagation (capturing and bubbling)
- Debouncing and Throttling
- Prototypes and Inheritance
- Classes and Constructors
- Interview Patters

**In many places you are asked output based questions on javascript so concepts should be very clear.**

**Resources**
- https://bigfrontend.dev/quiz (Solve output based questions from start. Cover the important ones)
- Watch all videos of Roadside coder for better practise - https://learn.roadsidecoder.com/new-courses/1/content?activeTab=Content (Javascript) [Paid course]
- Watch Akshay Saini (Namaste Javascript Series [free on youtube])
- Use GreatFrontEnd's JavaScript questions to structure your practice: start with Easy to build momentum, progress to Medium to deepen understanding, and tackle a few Hard problems if time permits. (https://www.greatfrontend.com/questions/javascript-interview-questions).
- Cover important topics like polyfills for promise, promise APIs, call, apply, bind, reduce, filter, some, etc.
- https://javascript.info/ (Good source for JS fundamentals)
- https://www.youtube.com/@theavocoder (JS fundamentals)
- https://github.com/saumyadip25/Knowledge-Base (You can refer this also some important notes)

## FRAMEWORK/MACHINE CODING

The machine coding round is designed to evaluate how efficiently you can live-code a given UI, task, or challenge within a limited time frame (typically 45 minutes to 1 hour). You can use any framework of your choice, such as React, Vue, or Angular. The key focus areas are writing modular, extensible, and maintainable code while effectively managing your time. Prioritize implementing core functionality first, and focus on styling and polish only if time permits. Evaluation is primarily based on functionality, code structure, and problem-solving approach.

Practice these questions in codesandbox and try to solve them in 50 minutes like a real interview. I.e Build a N*N tic tac toe game.

**Resources -**
- You can solve all problems from https://learn.roadsidecoder.com/ in Machine Coding section. You can also see and try to solve the problems mentioned in his youtube channel.
- Solve all questions from Namaste System Design paid course by Akshay Saini. Also solve Machine coding problems from his youtube platform which is free.
- There is a platform called https://devtools.tech/ you can solve the problems from here also to get better.
- You can also refer and solve these important and good questions from my github - https://github.com/saumyadip25/Frontend-Machine-Coding.
- There are problems which are there in greatfrontend as well which are good and can be solved to get more confidence. The link is - https://www.greatfrontend.com/questions

**Note:** There are some problems which will overlap and you can skip it.

## SYSTEM DESIGN

The system design round is a crucial part of interviews for senior frontend roles. In this round, you typically don't need to write code, but you're expected to design the architecture and web view of complex systems based on the given problem.

Before diving into solving system design problems, it's important to strengthen your fundamentals such as communication protocols, databases, caching, offline support, and other core concepts. Having a solid understanding of these will help you reason through trade-offs and design decisions confidently.

I personally followed the NamasteDev System Design course, which provides a great foundation. You can also explore other excellent resources like:

**JS Café**
- https://www.youtube.com/@DevtoolsTech
- https://namastedev.com/learn/namaste-frontend-system-design/hld-overview
- https://www.youtube.com/watch?v=5vyKhm2NTfw&list=PLI9W87-Dqn7j_x6QtR6sUjycJR7nQLBqT
- https://www.youtube.com/watch?v=sV_4pOGosnU&list=PL4CFloQ4GGWICE0Tz6iXKfN3XWkXRlboU
- https://frontendlead.com/system-design
- https://www.greatfrontend.com/front-end-system-design-playbook

Or simply explore YouTube and Google for specific topics you want to dive deeper into. Personally, I found the NamasteDev and GreatFrontend system design resources particularly helpful. However, the other channels mentioned are equally valuable and definitely worth exploring for a broader understanding.

Once you've covered the basics, start practicing problems on your own. Try designing the system first perhaps on a whiteboard before looking at others' solutions. This approach helps you deeply internalize the concepts and develop your own structured way of thinking.

## MISCELLANEOUS FRONTEND/OTHER TOPICS

You should read about web vitals, optimisation of html, js and css from https://web.dev/.

The above resource is the best resource which is present. Try to read most of the topics from it. Also I would recommend that if you have a NamasteDev System Design Course, go through all topics.

Read about recent hooks introduced in React-18, React-19. The interviewer might ask you if you have heard it and how and where to use it.

Try to search leetcode interview experiences of frontend for different companies and practise them. I practised these 30 interview experiences from this source - https://study.learnyard.com/web/courses/6827a7b3101963b5e349142f?chapter=6828d1b55a77c2de8cb465ca.

Focus on backend system design at a high level, don't dive too deep right away. Get comfortable with fundamentals like sharding, SQL vs. NoSQL trade-offs, and message queues. Building this overview first will give you a strong foundation for designing robust systems.

Read about micro-frontends and understand how they can be implemented using tools like Webpack Module Federation and Vite Module Federation. Explore tutorials and explanations on Google and YouTube to get a practical understanding of how they work in real projects.

Read about web workers and service workers.

Also be prepared with 3 different projects that you have worked upon in previous companies and the challenges you faced. You should explain this properly using the STAR framework.

## DATA STRUCTURES AND ALGORITHMS

In many interviews during the online test or the initial rounds you might face DSA questions.

You should be comfortable solving problems in JavaScript or your preferred programming language.

However, in some interviews, especially for frontend roles, interviewers may specifically ask you to implement the solution in JavaScript, so it's important to be well-prepared for that.

During my preparation, I practiced solving problems in both C++ and JavaScript, which helped me strengthen my problem-solving skills and improve my fluency in JavaScript.

I followed the NeetCode 150 and regularly solved LeetCode Medium and Hard problems, typically 3 to 4 problems a day.

I made it a habit to mix problems from different topics such as trees, dynamic programming, binary search, and graphs to stay well-rounded.

If you're a beginner, start by solving problems topic-wise, beginning with easy ones and gradually moving to medium-level problems to build a strong foundation. Once you feel confident, start mixing problems from different topics to better mimic real interview scenarios. In actual interviews, the topic isn't revealed, so you'll need to identify the concept behind the problem yourself, practicing this way helps you develop the ability to recognize patterns and think analytically under pressure.

In most interviews, hard-level problems are rare. Typically, you'll be asked medium to slightly hard questions.

Hard problems are usually seen in senior-level interviews at certain companies like PayPal, Quince, and Google (based on what I've heard).
