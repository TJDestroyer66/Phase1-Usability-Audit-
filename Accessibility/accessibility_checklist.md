# StudyFlow — Accessibility Checklist (WCAG 2.1 AA)

## Scope and status
This checklist is based on the StudyFlow Phase 2 sitemap and wireframes. It is a design and implementation checklist, not evidence of a completed accessibility audit or conformance claim. Test the working prototype before reporting any item as passed.

## Perceivable
- [ ] Provide text alternatives for meaningful icons and images (1.1.1).
- [ ] Do not use color alone to communicate task priority, completion, overdue status, or errors (1.4.1).
- [ ] Ensure text contrast is at least 4.5:1 for normal text and 3:1 for large text (1.4.3).
- [ ] Ensure meaningful non-text controls and graphical indicators have sufficient contrast (1.4.11).
- [ ] Support text resizing up to 200% without loss of content or functionality (1.4.4).
- [ ] Reflow content at narrow viewport widths without unnecessary two-dimensional scrolling (1.4.10).
- [ ] Ensure text spacing adjustments do not cause content loss (1.4.12).

## Operable
- [ ] Make all functionality available from a keyboard (2.1.1).
- [ ] Ensure there are no keyboard traps (2.1.2).
- [ ] Provide visible focus indicators (2.4.7).
- [ ] Use descriptive page titles, headings, and link purposes (2.4.2, 2.4.4, 2.4.6).
- [ ] Provide a skip link or another way to bypass repeated navigation (2.4.1).
- [ ] Ensure focus is not obscured by sticky or fixed content (2.4.11, WCAG 2.2 criterion; include only if evaluating beyond 2.1 AA).
- [ ] Provide adequate time to complete tasks if any time limits exist (2.2.1).

## Understandable
- [ ] Set the page language in the document (`<html lang="en">`) (3.1.1).
- [ ] Use consistent navigation and identify repeated components consistently (3.2.3, 3.2.4).
- [ ] Label form fields and identify required inputs (3.3.2).
- [ ] Identify input errors in text and provide correction suggestions when known (3.3.1, 3.3.3).
- [ ] Do not rely on placeholder text as the only label.
- [ ] Ensure controls have predictable names and behavior.

## Robust
- [ ] Use valid, semantic HTML where possible (4.1.1).
- [ ] Ensure names, roles, and values for controls are exposed to assistive technology (4.1.2).
- [ ] Announce important dynamic status messages, such as “Task saved” or “Task marked complete,” without unnecessarily moving focus (4.1.3).

## StudyFlow-specific checks
- [ ] Dashboard summary cards expose their values as text; progress is not conveyed by a ring/color alone.
- [ ] Upcoming deadline items have meaningful task names and due dates.
- [ ] All Tasks search, Course filter, Priority filter, and Sort by controls have visible labels.
- [ ] Task rows can be opened using a keyboard and have understandable accessible names.
- [ ] Create Task fields have labels, required-field instructions, and associated validation errors.
- [ ] Task Details actions (Edit, Mark Complete, Delete) have clear names and distinguishable purposes.
- [ ] Delete confirmation, if implemented, is keyboard accessible and returns focus appropriately.
- [ ] Completed Tasks includes completion dates as readable text.
- [ ] Empty states and search-result counts are communicated in text and announced when updated.

## Suggested manual test procedure
1. Navigate each of the five screens using only `Tab`, `Shift + Tab`, `Enter`, `Space`, arrow keys, and `Escape` where relevant.
2. Check that the visible focus indicator is easy to locate at every step.
3. Complete the Create Task flow using only the keyboard, including a validation error case.
4. Complete the Find and Complete Task flow using only the keyboard.
5. Test browser zoom at 200% and a narrow viewport.
6. Use a screen reader (such as NVDA with Firefox or Chrome) to verify landmarks, headings, form labels, table headers, and dynamic status announcements.
7. Record actual results and fix issues before claiming WCAG conformance.

## Important note
A checklist or wireframe alone cannot establish WCAG 2.1 AA compliance. Compliance requires testing the implemented interface, including contrast measurements, keyboard behavior, screen-reader output, responsive behavior, and form error handling.
