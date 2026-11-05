# StudyFlow — Semantic Structure Annotations

## Purpose
This document describes the proposed semantic page structure for the StudyFlow Student Task Manager, based on the Phase 2 sitemap and wireframe set. These are implementation annotations and recommendations; they are not a claim that the current prototype has already implemented or passed these checks.

## Shared page structure

Use a consistent structure across the Dashboard, All Tasks, Create Task, Task Details, and Completed Tasks screens.

```html
<body>
  <a class="skip-link" href="#main-content">Skip to main content</a>

  <header>
    <a href="/" aria-label="StudyFlow home">StudyFlow</a>
    <form role="search" aria-label="Search tasks">
      <label for="global-task-search">Search tasks</label>
      <input id="global-task-search" type="search" />
      <button type="submit">Search</button>
    </form>
    <nav aria-label="Account navigation">
      <!-- Profile and notification links or buttons -->
    </nav>
  </header>

  <nav aria-label="Primary navigation">
    <!-- Dashboard, Tasks, Find & Organize, Progress & Deadlines -->
  </nav>

  <main id="main-content">
    <h1><!-- Unique title for the current page --></h1>
    <!-- Page-specific content -->
  </main>

  <footer>
    <!-- Help and relevant support links -->
  </footer>
</body>
```

## Page-specific annotations

### 1. Dashboard
- Use one `<main>` landmark and one clear `<h1>` such as “Dashboard”.
- Group summary values (Total Tasks, Completed, Overdue) in a labelled section, for example `<section aria-labelledby="task-summary-heading">`.
- Use headings for “Upcoming Deadlines” and “Task Progress”.
- If a progress graphic conveys information, provide equivalent text (for example, “42% complete”) so the value is not communicated by color or shape alone.
- Make “View All Deadlines” a descriptive link to the relevant deadline view.
- The “Create Task” call to action should be a real button or link with an accessible name.

### 2. All Tasks
- Put the task list controls in a labelled search/filter region.
- Use a real `<form role="search">` for task search, with a visible `<label>`.
- Give each filter and sort control a visible label, such as “Course”, “Priority”, and “Sort by”.
- Represent tabular task data with a semantic `<table>` and `<th scope="col">` headers when the information is genuinely tabular.
- If tasks are presented as cards instead, use a list (`<ul>` / `<li>`) with a heading/link for each task.
- Make the task name itself a keyboard-accessible link or button to open Task Details.

### 3. Create Task
- Use a `<form>` with explicitly associated `<label>` elements for Task Title, Course, Due Date, Priority, and Description.
- Indicate required fields in text, not only with an asterisk or color.
- Use appropriate input types (for example, `type="date"` for the due date where supported).
- Connect validation feedback to the relevant field with `aria-describedby`; set `aria-invalid="true"` when a field has an error.
- Place an error summary near the top of the form when submission fails, and move focus to it or announce it appropriately.
- Use a submit button labelled “Save Task”; Cancel should be a link or button with a clear destination/action.

### 4. Task Details
- Use a descriptive `<h1>` containing the task name.
- Group task metadata in a labelled section or definition list (`<dl>`, `<dt>`, `<dd>`).
- Use buttons with clear accessible names for Edit, Mark Complete, and Delete.
- For destructive actions such as Delete, provide a confirmation step with a clear explanation and keyboard-accessible Cancel and Confirm actions.
- After a task is marked complete, announce the status change with a polite live region (for example, `role="status"`).

### 5. Completed Tasks
- Use a unique `<h1>` such as “Completed Tasks”.
- Provide a labelled search field and visible labels for filters/sort controls.
- Use a semantic table or list, consistent with the All Tasks representation.
- Include completion date as text, not only as a visual badge or icon.
- If the list updates dynamically, announce the result count or empty state with a polite status message.

## Navigation and interaction notes
- Use `<nav>` landmarks only for groups of navigation links; give each a distinct accessible label when there is more than one.
- Use links for navigation and buttons for actions.
- Keep navigation labels consistent with the sitemap: Dashboard, Tasks, Find & Organize, and Progress & Deadlines.
- Indicate the current page with `aria-current="page"` on its navigation link.
- Use a visible skip link to bypass repeated navigation.
- Avoid using ARIA when native HTML semantics already provide the required meaning.
