# StudyFlow Phase 2 — Post-Mortem Reflections

## 1. What I learned from the card-sorting activity

The card-sorting activity helped me understand how users naturally group the different features in StudyFlow. Across the three participant results, there was strong agreement around several groups. Creating, editing, and deleting tasks were consistently grouped together, while searching and filtering tasks by course or priority were also commonly grouped together. Participants also tended to associate completed tasks, pending tasks, and task progress with one another.

The results showed that users do not always organize features in exactly the same way. For example, participants differed on where to place the Mark Complete action. Some associated it with task actions, while others grouped it with progress and completion tracking. There were also differences in how participants grouped sorting by due date and task details. This showed me that some features can reasonably fit into more than one category depending on how users think about their purpose.

## 2. How the results influenced the sitemap

I used the common patterns from the card-sorting results to organize the sitemap into clear navigation areas: Dashboard, Tasks, Find & Organize, and Progress & Deadlines.

The Tasks area contains the main task-management functions, including viewing tasks and creating new ones. Find & Organize contains search, course and priority filters, and sorting. Progress & Deadlines groups views such as pending, completed, overdue, and upcoming tasks, along with task progress.

Some decisions required interpretation because participants did not always agree. I placed Mark Complete as an action available from Task Details because it applies to an individual task, while the completed and pending views remain under Progress & Deadlines. I placed sorting by due date under Find & Organize because sorting is a way to organize the task list, even though some participants associated it more closely with deadlines. Task Details is reached by selecting an individual task rather than being treated as a separate top-level navigation destination.

## 3. What worked well

The card-sorting activity provided a useful starting point for designing the information architecture instead of relying only on my own assumptions. The repeated groupings made it easier to identify features that belong together. Creating the sitemap after reviewing the results also helped make the navigation structure more consistent and gave the two user flows a clear path through the application.

The two user flows helped connect the sitemap to realistic tasks: creating and saving a task, and finding and completing a task. The wireframes then showed how the screens and navigation could support those activities.

## 4. What could be improved

The study used only three participants, so the results provide an initial indication of how users might organize StudyFlow rather than a definitive representation of all users. A larger and more varied participant group could reveal additional patterns or different expectations.

Some card descriptions could also be interpreted in more than one way. For example, “Mark a Task as Complete” could be understood as a task-management action or as part of progress tracking. In a future session, I would make the card wording more specific where needed and ask participants to explain why they grouped certain cards together.

The activity focused on how users grouped feature names. It did not measure how quickly users could find features in an interactive interface or whether the resulting navigation would be easy to use in practice. A future iteration should include usability testing with representative tasks, such as creating a task, finding a task by course, and marking a task complete.

## 5. What I would do in the next iteration

In the next iteration, I would test the proposed sitemap and wireframes with additional users. I would ask participants to complete common StudyFlow tasks and observe whether they can locate the correct navigation areas without assistance. I would pay particular attention to the placement of Mark Complete, the relationship between Find & Organize and Progress & Deadlines, and whether users understand where to find overdue and upcoming tasks.

I would also test the keyboard navigation and accessibility recommendations against the implemented prototype. This would help identify issues that cannot be confirmed from a sitemap or wireframe alone, such as actual focus order, screen-reader announcements, contrast, and form validation behavior.

## 6. Overall reflection

Overall, this phase showed me how user research can guide the structure of an application. The card-sorting results gave me evidence for organizing StudyFlow's features, while the sitemap, user flows, and wireframes translated those findings into a proposed interface. The process also showed that information architecture involves making design decisions when participant preferences differ. Those decisions should be based on the patterns in the results, the purpose of each feature, and future usability testing.
