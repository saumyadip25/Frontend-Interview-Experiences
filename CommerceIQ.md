# CommerceIQ Interview Experience

## Role Information

- **Position:** SDE-2 (Frontend)
- **Application Date:** October 2025
- **Application Method:** Applied through Career Site
- **Total Rounds:** 3 (Completed 1)

---

## Round 1: Machine Coding

**Duration:** 60 minutes

**Problem: Task Queue Visualizer**

Build a React/Vue/Svelte/Angular component to manage and visualize a task queue with the primary focus on demonstrating strong state management, clear visual representation of asynchronous processes, and handling concurrency.

---

### Level 1: The Basics - Unlimited Parallelism

**Goal:** Create a UI where users can add tasks to a queue, and all tasks start processing immediately in parallel.

**Requirements:**

1. **Add Tasks**

   - Implement an input field and button to add new tasks to the queue

2. **Display Queue**

   - Show a list of all added tasks

3. **Visualize Progress**

   - Each task must have its own progress bar
   - Progress bar updates from 0% to 100%

4. **Automatic Execution**
   - Tasks start processing automatically when added
   - Fixed completion time: 2 seconds per task
   - All tasks run concurrently without limits

---

### Level 2: The Executor - Limited Concurrency

**Goal:** Introduce concurrency constraints to create a true queuing system where only a limited number of tasks can run simultaneously.

**Requirements:**

1. **Concurrency Limit**

   - Maximum of 3 tasks can process in parallel
   - Additional tasks must wait in a pending state

2. **Queueing Logic**

   - When 3 tasks are already running, new tasks enter "pending" state
   - When a running task completes, automatically start the next pending task
   - Maintain FIFO (First In, First Out) order for pending tasks

3. **Clear Status Indication**
   - Visually distinguish between three states:
     - **Running:** Currently processing (max 3)
     - **Pending:** Waiting to be processed
     - **Completed:** Finished execution

---

### Bonus Level: Advanced Features (Optional)

**Goal:** Enhance the application with more user control and sophisticated logic.

**Optional Enhancements:**

1. **Reset Functionality**

   - Add a "Reset" button to clear all tasks
   - Reset UI to initial state
   - Clear running, pending, and completed tasks

2. **Custom Execution Times**

   - Allow users to specify task duration when adding
   - Provide dropdown with options (e.g., 1s, 4s, 8s)
   - Each task can have different execution time

3. **Task Prioritization**
   - Introduce priority levels: High, Medium, Low
   - High-priority tasks in pending queue process before lower-priority ones
   - Implement priority-based queue instead of FIFO

---

### Key Focus Areas

**State Management:**

- Task structure (id, status, progress, duration, priority)
- Queue management for pending tasks
- Tracking concurrent execution count

**Asynchronous Operations:**

- Simulating task processing with timers
- Progress updates at regular intervals
- Handling task completion and queue transitions

**UI/UX Clarity:**

- Immediate visibility of system state
- Clear representation of each task's status
- Visual feedback for all transitions

**Code Quality:**

- Clean, readable, and maintainable code
- Proper component structure
- Efficient state updates

**Note:** Styling is secondary to functionality. The primary focus is clear visual feedback and accurate state representation rather than polished design.

---

## My Implementation

**Completed:** Level 1 and Level 2

I successfully implemented both the basic unlimited parallelism (Level 1) and the advanced concurrency-limited executor (Level 2). The solution included:

- Task addition with unique IDs
- Progress bar visualization for each task
- Concurrent execution with a limit of 3 tasks
- Automatic queue management (moving pending tasks to running state)
- Clear visual distinction between running, pending, and completed tasks

**Minor Issue in Level 2:**

There was a small bug in the Level 2 implementation related to the queue management logic. However, the interviewer acknowledged it was a minor issue and did not express concern about it, as the overall approach and implementation were solid.

---

## Overall Experience

**Result:** Withdrew after Round 1

The first round went reasonably well. I was able to complete both Level 1 and Level 2 within the time limit, demonstrating good understanding of state management, asynchronous operations, and React component architecture. I did not had time for Bonus Levels.
After completing the first round, the recruiter reached out to schedule the next interview rounds. At that point, I informed them that I did not wish to continue with the interview process. The reason was I was tired and needed some break because I was giving interview and preparing since last 2.5 months.
