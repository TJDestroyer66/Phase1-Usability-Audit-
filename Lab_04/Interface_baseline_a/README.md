# Interface A — Traditional Single-Page Form

This folder contains the baseline version of the StudyFlow Student Task Manager for the HCI comparison study.

## How to run
1. Keep `index.html`, `styles.css`, and `script.js` together in this folder.
2. Open `index.html` in a modern web browser.
3. Select **Add task** to open the task form.

## Interface A behavior
- All task fields are displayed on one screen.
- Participants enter title, course, optional description, due date, and priority.
- Required fields and due-date validation are applied.
- Participants select **Save task** directly; there is no separate review step.
- The task is added to the dashboard and a confirmation toast is displayed.

## Study comparison
- Interface A: this single-page form.
- Interface B: the existing multi-step wizard in the original project.
- Keep Interface B unchanged so the two study conditions remain distinct.
- Both versions use the same dashboard layout, task fields, validation requirements, and local browser storage key.

## Important testing note
The prototype stores tasks in the browser's local storage. Before each participant session, use a clean browser profile or clear the site's local storage so previous test entries do not affect the next session.
