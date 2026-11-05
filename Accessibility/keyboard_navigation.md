# StudyFlow — Keyboard Navigation Plan

## Purpose
This plan defines the expected keyboard behavior for the five wireframed StudyFlow screens. It is a proposed interaction specification and should be verified against the implemented prototype.

## Global keyboard behavior
- `Tab`: Move forward through interactive elements in a logical reading order.
- `Shift + Tab`: Move backward through interactive elements.
- `Enter`: Activate links and buttons; submit a form when focus is on its submit button.
- `Space`: Activate buttons and toggle native checkboxes or other native controls when focused.
- `Arrow keys`: Operate native select controls and radio groups according to browser/platform behavior. If custom menus are implemented, provide the expected arrow-key behavior and focus management.
- `Escape`: Close an open menu, dialog, or popover and return focus to the control that opened it.
- Focus must always be visible and must not be hidden behind sticky headers, overlays, or other content.

## Recommended tab order by screen

### Shared header and navigation
1. Skip to main content link (visible on focus).
2. StudyFlow home link.
3. Global task search field.
4. Search submit button, if separate.
5. Notifications control, if interactive.
6. Account/profile control.
7. Primary navigation links and expandable navigation controls.
8. Main content controls in visual and reading order.
9. Footer/help links.

Do not add `tabindex` values greater than zero. Prefer the natural DOM order. If navigation groups are collapsible, their toggle buttons must expose expanded/collapsed state and the contained links must only be tabbable when visible.

### Dashboard
- After shared navigation, move through the task summary content (non-interactive summary values are not added to the tab order).
- Continue to Upcoming Deadlines links or task actions in reading order.
- Then Task Progress details, if interactive.
- Finish with View All Deadlines and Create Task actions in a logical order matching the visual layout.
- Do not make static charts or summary cards keyboard-focusable unless they perform an action.

### All Tasks
- After shared navigation, focus the search field and its submit control.
- Continue through Course filter, Priority filter, and Sort by control.
- Move through task rows in order. Each task name/action must be keyboard-accessible.
- Continue through pagination controls, if present.
- Provide a clear empty-results message when search/filtering returns no tasks.

### Create Task
- After shared navigation, move through Task Title, Course, Due Date, Priority, and Description in that order.
- Continue to Cancel and Save Task controls.
- Required fields must be identified in their labels or associated instructions.
- On invalid submission, present errors in text, associate them with fields, and move focus to an error summary or the first invalid field.
- On successful save, announce confirmation and place the user somewhere predictable, such as the new task's details page or All Tasks with the new task visible.

### Task Details
- After shared navigation and any breadcrumb links, move to the task title/context and then available actions: Edit, Mark Complete, Delete.
- If actions are buttons, they must have visible focus indicators.
- If Delete opens a confirmation dialog, move focus into the dialog, keep focus within it while open, support Escape to cancel where appropriate, and return focus to Delete when closed.
- After Mark Complete, announce the status update and keep focus in a predictable location.

### Completed Tasks
- After shared navigation, move through search, filters, and sorting controls.
- Continue through completed task entries and their completion dates.
- If pagination is present, make each control keyboard-operable and clearly named.
- If the list is empty, provide a helpful text message and a clear way to return to All Tasks.

## Verification checklist
- [ ] All interactive elements can be reached using only the keyboard.
- [ ] Focus order follows the visual and semantic reading order.
- [ ] Focus indicator is clearly visible.
- [ ] No keyboard trap occurs.
- [ ] Menus and dialogs support expected keyboard behavior.
- [ ] Focus is restored appropriately after closing overlays.
- [ ] Forms can be completed and submitted without a mouse.
- [ ] Dynamic updates and validation messages are announced to assistive technology.
