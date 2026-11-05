# StudyFlow User Flow Diagrams

These diagrams document two representative tasks in the StudyFlow Student Task Manager.

## Flow 1 — Create and Save a Task
The user opens the Dashboard, chooses Create Task, enters the task title, course, due date, and priority, and saves. The system validates required information. If information is missing or invalid, the user receives a validation message and returns to the form to correct it. When valid, the task is saved and becomes available in All Tasks.

## Flow 2 — Find and Complete a Task
The user opens All Tasks, searches or filters the list, selects a matching task, opens Task Details, and chooses Mark Complete. The system updates the task status and the task appears in Completed Tasks.

## Files
- `flow_1_create_and_save_task.png` — image export of Flow 1
- `flow_1_create_and_save_task.svg` — scalable vector export of Flow 1
- `flow_2_find_and_complete_task.png` — image export of Flow 2
- `flow_2_find_and_complete_task.svg` — scalable vector export of Flow 2

## Diagram conventions
- Green rounded rectangle: starting point
- Gray rounded rectangle: user action or system process
- Yellow diamond: decision point
- Blue rounded rectangle: end state
- Orange side note: validation error path

## Assumptions to verify against the prototype
These flows use the proposed StudyFlow information architecture. Confirm that the live prototype uses the same labels and behavior before submitting. In particular, the validation message and whether completed tasks automatically appear in a Completed Tasks view should match the implemented interface.
