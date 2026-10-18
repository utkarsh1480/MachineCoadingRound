# Assignment Round 2 — Todo List Application

## Instructions

Please read all requirements before starting the assignment.

1. Spend the first 5 minutes reviewing the requirements and planning your implementation.
2. **Time limit: 45 minutes.**
3. Use **HTML, CSS, and vanilla JavaScript only**.
4. Do not use React, Vue, Angular, Bootstrap, Tailwind CSS, jQuery, or other libraries/frameworks.
5. Use a code editor such as Visual Studio Code.
6. You may consult documentation to verify HTML, CSS, and JavaScript behavior.
7. Implement the application yourself and be prepared to explain your decisions.
8. Test the application with different task states and viewport sizes.

## Overview

Build a small **Todo List Application** called **My Tasks**. Users should be able to add tasks, mark them as completed, delete tasks, filter tasks by status, and retain their tasks after refreshing the page.

The focus is on DOM manipulation, event handling, state management, CSS Flexbox, and browser `localStorage`.

## Detailed Requirements

### 1. Initial layout

The page should contain:

- A heading: **My Tasks**
- A text input for entering a task.
- An **Add Task** button.
- A task list.
- Three filters: **All**, **Active**, and **Completed**.
- A remaining-task counter.

Create a clean, readable layout with consistent spacing and a responsive design.

### 2. Adding tasks

- A user can type a task into the input and click **Add Task** to add it.
- Pressing **Enter** in the input should also add the task.
- Empty or whitespace-only tasks must not be added.
- After adding a valid task, clear the input.
- Each task should have a unique identifier in your JavaScript state.
- Multiple tasks may have the same text; deleting or completing one should affect only that specific task.

### 3. Completing tasks

- Each task must have a checkbox or equivalent control.
- Selecting it marks the task as completed.
- Selecting it again returns the task to active status.
- Completed tasks should have a visible visual distinction, such as a strikethrough.

### 4. Deleting tasks

- Each task must have a delete button.
- Deleting a task removes only that task from the list and application state.
- The remaining-task count should update after deletion.

### 5. Filtering tasks

Provide three filters:

- **All:** show every task.
- **Active:** show only incomplete tasks.
- **Completed:** show only completed tasks.

The selected filter should be visually distinguishable. Filtering must not delete or modify tasks; it only changes which tasks are displayed.

### 6. Remaining-task counter

Display the number of active tasks. For example:

- `0 tasks remaining`
- `1 task remaining`
- `3 tasks remaining`

Use correct singular/plural wording.

### 7. Empty states

Show a helpful message when:

- There are no tasks at all.
- The selected filter has no matching tasks.

Do not display a blank task-list area without feedback.

### 8. Persistence with localStorage

- Save the task list to `localStorage`.
- Restore saved tasks when the application loads.
- Add, complete, and delete actions must be reflected in storage.
- Refreshing the page must not remove saved tasks.
- Handle missing or invalid stored data gracefully.

### 9. Styling and responsive behavior

- Use **Flexbox** for the input/action row and individual task rows.
- Make the page usable on desktop, tablet, and mobile.
- Prevent long task text from breaking the layout.
- Provide consistent padding, spacing, borders, and typography.
- Add hover and keyboard-focus states to interactive controls.
- Make completed tasks visually distinct.
- Use semantic HTML and accessible labels where appropriate.

## Technical Constraints

- Use three separate files: `index.html`, `style.css`, and `script.js`.
- Do not use CSS Grid for the main task layout; use Flexbox.
- Do not use inline event handlers such as `onclick="..."`; attach events in JavaScript.
- Avoid unnecessary global variables.
- Keep the task data separate from the DOM where practical.
- Use reusable functions for rendering and updating state.
- Do not insert user-entered task text as raw HTML. Use safe DOM APIs or `textContent`.
- Ensure all buttons have an appropriate `type`.
- Keep the code readable and consistently formatted.

## Suggested Project Structure

```text
todo-list/
├── index.html
├── style.css
└── script.js
```

## Acceptance Checklist

Before submitting, verify each item:

- [ ] The page displays the heading, input, Add Task button, filters, counter, and list.
- [ ] A task can be added by clicking Add Task.
- [ ] A task can be added by pressing Enter.
- [ ] Empty and whitespace-only tasks are rejected.
- [ ] The input clears after a valid task is added.
- [ ] Each task has a working completion control.
- [ ] Completed tasks have a visible style change.
- [ ] Each task has a working delete button.
- [ ] All, Active, and Completed filters work correctly.
- [ ] The selected filter is visually indicated.
- [ ] The remaining-task count is accurate and uses correct singular/plural wording.
- [ ] Empty states are displayed appropriately.
- [ ] Tasks persist after refreshing the page.
- [ ] Invalid stored data does not crash the application.
- [ ] The layout works at desktop, tablet, and mobile widths.
- [ ] Long task names do not cause horizontal overflow.
- [ ] HTML, CSS, and JavaScript are separated into the required files.
- [ ] User-entered task text is rendered safely.
- [ ] Controls are keyboard-accessible and have visible focus styles.

## Evaluation Rubric

| Category | Marks |
|---|---:|
| UI and Flexbox layout | 20 |
| Add, complete, and delete functionality | 30 |
| Filtering and task counter | 20 |
| `localStorage` persistence | 15 |
| Responsive design, accessibility, and code quality | 15 |
| **Total** | **100** |

### Suggested Score Interpretation

- **90–100:** Strong solution with reliable behavior and clean implementation.
- **75–89:** Good solution with a few missing edge cases or polish issues.
- **60–74:** Core features work, but some requirements are incomplete.
- **Below 60:** Revisit DOM manipulation, event handling, and state updates.

## Suggested Time Management

| Time | Goal |
|---|---|
| 0–5 minutes | Read requirements and plan state/data structure |
| 5–12 minutes | Build HTML and basic CSS layout |
| 12–27 minutes | Implement add, complete, delete, and rendering |
| 27–35 minutes | Add filters and remaining-task counter |
| 35–40 minutes | Add `localStorage` persistence |
| 40–45 minutes | Test edge cases and responsive behavior |

This schedule is a guide; prioritize core functionality first if you are running behind.

## Interview Follow-up Questions

Be ready to explain:

1. How does `addEventListener` work?
2. What is the difference between `event.preventDefault()` and `event.stopPropagation()`?
3. How would you represent tasks in an array of objects?
4. Why should each task have a unique ID?
5. What is the difference between `map()`, `filter()`, and `forEach()`?
6. How can you render user input safely and avoid injecting raw HTML?
7. What is `localStorage`, and how does it differ from `sessionStorage`?
8. Why does `localStorage` store strings, and how do `JSON.stringify()` and `JSON.parse()` help?
9. How should the counter behave when completed tasks are deleted?
10. How would you test filtering when there are no matching tasks?

## Submission

Submit the following files:

1. `index.html`
2. `style.css`
3. `script.js`
4. A screenshot of the desktop layout.
5. A screenshot of the mobile layout.

Name the project folder **`todo-list`**. Before submitting, test adding, completing, deleting, filtering, and refreshing the application.

**Important:** This document describes the assignment only; it does not include a solution. Complete the challenge independently, then use the acceptance checklist to review your implementation.

**Good luck!**
