# StudyFlow Card Sorting Results and Analysis

## 1. Study overview
| Item |
|---|---|
| Product | StudyFlow student task manager |
| Method | Open card sort |
| Number of cards | 15 |
| Participants | 3 (P01–P03) |
| Goal | Understand how users naturally group StudyFlow tasks and navigation functions |

Participants were asked to group the 15 cards into categories that made sense to them and provide a name for each category. No category names were supplied.

## 2. Participant grouping summary

### P01
- **Task Management:** View All Tasks; Create a New Task; Edit an Existing Task; Delete a Task; View Task Details
- **Task Organization:** Search for a Task; Filter Tasks by Course; Filter Tasks by Priority; Sort Tasks by Due Date
- **Task Progress:** Mark a Task as Complete; View Completed Tasks; View Pending Tasks; View Overdue Tasks; View Upcoming Deadlines; View Task Progress

### P02
- **Managing Tasks:** Create a New Task; Edit an Existing Task; Delete a Task; View Task Details
- **Finding Tasks:** View All Tasks; Search for a Task; Filter Tasks by Course; Filter Tasks by Priority
- **Deadlines:** Sort Tasks by Due Date; View Overdue Tasks; View Upcoming Deadlines
- **Completion Tracking:** Mark a Task as Complete; View Completed Tasks; View Pending Tasks; View Task Progress

### P03
- **Task Actions:** Create a New Task; Edit an Existing Task; Delete a Task; Mark a Task as Complete
- **Task Navigation:** View All Tasks; Search for a Task; View Task Details; Filter Tasks by Course; Filter Tasks by Priority
- **Tracking and Deadlines:** View Completed Tasks; View Pending Tasks; Sort Tasks by Due Date; View Overdue Tasks; View Upcoming Deadlines; View Task Progress

## 3. Patterns in the data
- **Task maintenance is consistent:** All three grouped Create, Edit, and Delete together.
- **Finding tasks is consistent:** All three grouped Search, Filter by Course, and Filter by Priority together, although their category labels varied.
- **Task status is related:** All three grouped View Completed Tasks and View Pending Tasks together.
- **Deadlines are related:** All three grouped View Overdue Tasks and View Upcoming Deadlines together.
- **Some functions are ambiguous:** Mark a Task as Complete was grouped with progress by P01/P02 but with task actions by P03. View Task Details was grouped with management by P01/P02 but navigation by P03.

## 4. Similarity matrix interpretation
`similarity_matrix.csv` records how many participants placed each pair of cards in the same category.
- 3 means all three participants grouped the pair together.
- 2 means two participants grouped the pair together.
- 1 means one participant grouped the pair together.
- 0 means no participants grouped the pair together.

For example, Create a New Task and Edit an Existing Task score 3, meaning all three participants placed them together. The matrix is a useful way to identify strong relationships before proposing navigation categories.

## 5. Initial information architecture recommendation
Based on these fictional patterns, a reasonable structure to investigate would be:

- **Tasks**
  - All Tasks
  - Create Task
  - Task Details
  - Search Tasks
- **Organize**
  - Filter by Course
  - Filter by Priority
  - Sort by Due Date
- **Progress and Deadlines**
  - Pending Tasks
  - Completed Tasks
  - Mark Complete
  - Overdue Tasks
  - Upcoming Deadlines
  - Task Progress

This is a proposed interpretation, not a proven final sitemap. Validate it against real participant results and any usability feedback.

## 6. Limitations

Small sample size: The study includes only three participants. While their groupings reveal some common patterns, this is not enough to represent the preferences of all StudyFlow users. Additional participants could produce different categories or identify relationships that were not apparent in these results.

Subjective category creation: Because this was an open card sort, participants were free to create and name their own categories. This allowed their individual mental models to influence the results, but it also meant that similar groups could have different names. For example, categories such as "Task Management," "Managing Tasks," and "Task Actions" may represent similar ideas even though the labels are different.

## 7. Files in this folder
- `card_deck.csv`: deck of 15 cards.
- `p01_card_sort.csv` through `p03_card_sort.csv`: participant-level category assignments.
- `p01_session_notes.md` through `p03_session_notes.md`: notes and comments.
- `session_log.csv`: session metadata.
- `all_participant_results.csv`: combined assignments.
- `similarity_matrix.csv`: pairwise co-sorting counts.
- `participant_data_template.csv`: participant data.
