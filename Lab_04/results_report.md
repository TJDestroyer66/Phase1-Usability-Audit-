# Lab 04 – Results Report
## Student Task Manager: Single-Page Form vs. Multi-Step Wizard

## 1. Study purpose

This study is designed to compare two versions of the Student Task Manager task-creation workflow:

- **Interface A – Baseline:** a traditional single-page form with all task fields displayed together.
- **Interface B – Treatment:** a guided multi-step wizard that separates task entry, review, and confirmation into stages.

The task is to create and save an academic task using a supplied title, description, course, due date, and priority, then verify that it appears in the task list.

The study uses a within-subjects design. Each participant completes the task in both interfaces. The planned order is counterbalanced, with three participants using A then B (AB) and three using B then A (BA).

## 2. Research questions and hypotheses

The study examines whether Interface B improves efficiency, effectiveness, and perceived ease compared with Interface A.

- **H1 – Completion time:** Participants will complete the task significantly faster with Interface B than Interface A.
- **H1 – Errors:** Participants will make significantly fewer errors with Interface B than Interface A.
- **H1 – Perceived ease:** Participants will give Interface B higher SEQ ratings than Interface A.

The corresponding null hypotheses state that there will be no statistically significant difference between the interfaces for each measure.

## 3. Method summary

The collected dataset contains **6 participant IDs (P01–P06)**, with two records per participant, for **12 total task attempts**. Three participants are assigned to AB order and three to BA order. The two scenarios are assigned to period 1 and period 2, respectively; because the interface order is balanced, each interface receives each scenario three times.

The dependent measures are:

1. **Task completion time:** seconds from the start cue to verified successful save, with a maximum of 300 seconds.
2. **Error count:** incorrect entries, rejected submissions, and participant corrections.
3. **Task success:** 1 when the task is saved and visibly verified, otherwise 0.
4. **SEQ rating:** a 1–7 response to “Overall, how easy or difficult was this task?” where 1 is very difficult and 7 is very easy.

## 4. Results

### 4.1 Descriptive statistics

| Measure | Interface A: Single-page | Interface B: Wizard |
|---|---:|---:|
| Participants | 6 | 6 |
| Mean completion time | 81.7 sec | 70.3 sec |
| Standard deviation (time) | 5.8 sec | 3.6 sec |
| Mean error count | 1.5 | 0.5 |
| Task success rate | 100% (6/6) | 100% (6/6) |
| Mean SEQ rating | 4.8 / 7 | 5.8 / 7 |

In this dataset, Interface B has a lower average completion time by 11.3 seconds. The average error count is lower by 1.0 errors per task. The average SEQ rating is 1.0 points higher for Interface B. Both interfaces have a 100% task success rate in this dataset, so task success does not distinguish the conditions.

### 4.2 Paired comparisons

Because each participant has a result for both interfaces, the experiment uses paired comparisons. A paired-participants t-test on these values gives:

| Measure | Mean paired difference (B − A) |  p-value |
|---|---:|---:|
| Completion time | -11.33 sec | 0.00384 |
| Error count | -1.00 errors | 0.04086 |
| SEQ rating | +1.00 points | 0.01172 |

## 5. Interpretation of the data

The pattern favors Interface B on all three measured outcomes. The wizard appears to help participants complete the task somewhat faster, make fewer corrections, and rate the task as easier. One possible explanation is that separating entry and review into stages makes the sequence of actions more explicit and gives users a dedicated opportunity to check their information before saving.

However, the data does not show a difference in task success because all participants successfully saved the task in both conditions. This illustrates why it is useful to measure more than success alone: two interfaces can both allow users to finish while differing in time, errors, and perceived ease.

These interpretations are hypotheses about what the pattern could mean, not conclusions about real users. Actual participant observations may show a different result, including no difference or an advantage for Interface A.

## 6. Limitations to discuss

Several limitations should be acknowledged:

- **Learning and order effects:** Participants may learn the task after the first condition. Counterbalancing AB and BA helps balance order, but does not remove every carryover effect.
- **Scenario differences:** The two scenarios should require equivalent information and effort. The researcher should record which scenario each participant receives in each period.
- **Researcher measurement:** Error counting and timing can involve judgment. The researcher should apply the same definitions and start/stop rules to every session.
- **Prototype scope:** The study evaluates one task-creation workflow in a prototype, not long-term use of a complete task-management product.
- **Technical consistency:** Browser, display, input devices, and save behavior should be held constant. Any technical problems should be documented.

## 7. Conclusion

In this dataset, the multi-step wizard (Interface B) performs better than the single-page form (Interface A) on average completion time, error count, and SEQ rating, while both interfaces achieve the same task success rate. If a similar pattern appears in another study, it may suggest that the wizard's staged workflow and review step improve the task-creation experience..

## 8. Post-mortem Reflection

1. What is the difference between statistical significance and practical significance?

Statistical significance helps indicate whether an observed difference is unlikely to be due to random variation under the assumptions of the statistical test. Practical significance considers whether the size of that difference actually matters in real-world use. For example, a statistically significant two-second improvement in task completion time may not meaningfully improve a student's workflow. However, even a modest reduction in errors could be important because it makes the interface more reliable. HCI researchers should consider both statistical evidence and the real-world impact on usability, accessibility, and task performance.

2. What carryover effects could occur, and how does counterbalancing address them?

Participants may learn the task requirements during their first attempt and complete the second attempt faster, regardless of which interface they use. They may also experience fatigue or frustration that makes their second attempt slower. In this study, the AB/BA design assigns three participants to use Interface A first and three to use Interface B first. This balances the order in which each interface is experienced, helping separate an overall practice or period effect from the interface comparison. However, counterbalancing does not eliminate every carryover effect, particularly asymmetric effects where experience with one interface influences performance on the other differently. This limitation should be considered when interpreting the results.

## Appendix: Dataset

The accompanying `participant_data.csv` contains **12 rows**: two interface trials for each of six participants. It follows the variable names in the study's data dictionary.


