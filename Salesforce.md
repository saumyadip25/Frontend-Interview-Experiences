# Salesforce Frontend Interview Experience

**Role:** Senior Member of Technical Staff (Frontend)  
**Application Date:** September 2025  
**Application Method:** Salesforce Career Site  
**Total Rounds:** 6

---

## Timeline

- Applied through career site
- Received recruiter call after 3-4 days

---

## Round 1: Online HackerRank Assessment

**Duration:** 60 minutes

### Questions

1. **Graph-based problem**
2. **Dynamic Programming on strings**

---

## Round 2: Hiring Manager Round

**Duration:** 45 minutes

### Topics Covered

1. **Current work experience** - tech stack and cultural fit questions
2. **FPS (Frames Per Second)**
   - What is it and why is it important?
   - What type of animations should not be used and why?
3. **System Design Problem:** Design a "Send message" functionality on Slack
   - Tag people in messages
   - UI component design
   - Communication protocols to be used
4. **What is canvas and why is it better for performance**

---

## Round 3: JS, HTML, CSS and React Fundamentals

**Duration:** 60 minutes

### Questions Asked

#### HTML & CSS

1. What is semantic HTML? Why should we follow semantic HTML instead of using only divs?
2. Difference between Flexbox and Grid
   - **Practical:** Implement a layout using CSS Grid (know the syntax)
3. How do you make your app responsive? (media queries, relative sizes, etc.)

#### JavaScript

4. What are `call`, `apply`, and `bind`? Explain differences
   - **Coding:** Write a polyfill for `bind`
5. What is the Critical Rendering Path? Explain CSSOM
6. How does the Event Loop work?

#### React

7. What does the `forwardRef` hook do? What do you know about `useImperativeHandle` hook?
8. How will you implement the data model for a chat application?
9. What is props drilling and how to fix it?
10. What is Client Side Rendering? When is it beneficial?

#### Performance

11. What are different resource hinting techniques?
12. How would you improve the INP (web vital)?

---

## Round 4: System Design - Google Maps

**Duration:** 60 minutes

**Problem:** Design maps.google.com

### Topics Discussed

- Canvas vs DOM rendering
- Tile-based rendering
- Level of Detail (LOD): Show different detail levels based on zoom (Suggested by interviewer)
- Debouncing/Throttling: Limit expensive operations during pan/zoom gestures
- State Management (Map state, Layer state, UI state)
- Caching Strategy
- APIs & Microservices
  - Tile service: Serves map tiles at different zoom levels
  - Geocoding API: Convert addresses to coordinates
  - Directions API: Calculate routes between points
  - Places API: Search and retrieve place information
  - Real-time data APIs: Traffic, transit updates
- User Interactions (Gesture handling, Event delegation, Touch optimization)
- Web Workers: Offload heavy computations (route calculations) to background threads
- Responsive design: Adapt UI for different screen sizes
- Keyboard navigation: Arrow keys for panning, +/- for zoom
- Screen reader support: Announce location changes, search results
- Error tracking: Monitor failed tile loads, API errors

**Note:** There was no right and wrong solution for this because this was a conversation where we had to build something from scratch. The interviewer was friendly and guided me in right direction wherever I was stuck.

---

## Round 5: System Design - WhatsApp Web

**Duration:** 60 minutes

**Problem:** Design web.whatsapp.com

- Since I had already solved and seen this question, it went really well with the lead engineer
- There were some new scenarios which were encountered by interviewer but I was able to come up with an approach

---

## Round 6: Culture Fit and Collaboration

**Duration:** 60 minutes  
**Interviewer:** LMTS (Lead Member of Technical Staff)

### Questions Asked

1. How do you handle conflicts?
2. How will you handle conflicts with the QA team?
3. Tell me about a scenario where you pushed a bug to production that caused an issue. What did you do?
   - Created RCA (Root Cause Analysis)
   - Added E2E tests
   - Other mitigation steps
4. Tell me about a scenario when working with someone was very difficult and how you handled it
5. Few more cultural questions

---

## Interview Feedback

### Positive

- Interviewers were friendly and collaborative
- Guidance provided when stuck

---

## Final Verdict: OFFER ACCEPTED

**Team:** Slack

