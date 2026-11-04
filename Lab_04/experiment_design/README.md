# Lab 04 – Experimental User Study Plan

## Project
**Student Task Manager**

## 1. Interface Task Selection and Empirical Problem Framing

### Target workflow
This study evaluates the workflow for creating and saving a new academic task in the Student Task Manager.

Participants will enter a task title, description, course, due date, and priority, then save the task and verify that it was created successfully.

### Interfaces being compared
- **Interface A – Baseline:** A traditional single-page form displaying all task fields together.
- **Interface B – Treatment:** A guided multi-step task-creation wizard that divides the same information into manageable stages and provides clear instructions, validation, and a review step.

Both interfaces must use the same task requirements, options, and save behavior. The intended difference is the interaction design, not the underlying functionality.

### Empirical rationale
A single-page form may make users manage several fields and requirements at once. This can increase cognitive load, contribute to input mistakes, and make it harder to identify what needs attention. The wizard is intended to make the workflow easier to understand by presenting information in stages and providing timely feedback.

The study will test whether the wizard improves task completion time, reduces errors, and improves perceived ease of use.

## 2. Research hypotheses

### Hypothesis 1 – Completion time
- **H1:** Participants will complete the task-creation workflow significantly faster with Interface B than with Interface A.
- **H0:** There will be no statistically significant difference in task completion time between Interface A and Interface B.

### Hypothesis 2 – Errors
- **H1:** Participants will make significantly fewer input and validation errors with Interface B than with Interface A.
- **H0:** There will be no statistically significant difference in error count between Interface A and Interface B.

### Hypothesis 3 – Perceived ease
- **H1:** Participants will report higher Single Ease Question (SEQ) ratings after using Interface B than after using Interface A.
- **H0:** There will be no statistically significant difference in SEQ ratings between Interface A and Interface B.

These are proposed hypotheses. They are not claims about results.

## 3. Variables and operational definitions

### Independent variable
**Interface design**, with two levels:
1. A – traditional single-page form.
2. B – guided multi-step wizard.

### Dependent variables

| Measure | Operational definition | Unit / scale |
|---|---|---|
| Task completion time | Elapsed time from the researcher’s start cue until successful save confirmation | Seconds |
| Total error count | Number of incorrect entries, rejected submissions, or participant corrections during the task | Count |
| Task ease (SEQ) | Response to “Overall, how easy or difficult was this task?” | 1–7 |

SEQ anchors: 1 = Very difficult; 2 = Difficult; 3 = Somewhat difficult; 4 = Neither difficult nor easy; 5 = Somewhat easy; 6 = Easy; 7 = Very easy.

A task is successful when the requested task is saved and the participant can verify its presence. If the participant cannot finish within five minutes, record task success as 0 and record the elapsed time as 300 seconds. Note any assistance or interruption.

### Potential confounds and controls

| Potential confound | Control strategy |
|---|---|
| Prior task-manager experience | Ask the same brief familiarity questions before testing; record responses |
| Typing speed and computer experience | Record relevant experience; use the same computer, keyboard, and mouse |
| Browser and display differences | Use the same browser/version and 1920 × 1080 display setting |
| Environmental distractions | Test in the same quiet location where practical |
| Learning and order effects | Counterbalance AB and BA interface order |
| Fatigue | Provide a two-minute break between conditions |
| Task difficulty | Use equivalent scenarios with the same number and type of required fields |
| Network or system latency | Run locally where possible and use equivalent save behavior |
| Researcher influence | Use a fixed script and do not coach participants through the interface |

## 4. Experimental design and sampling

### Design
Use a **within-subjects design**: every participant tests both interfaces. This allows each participant to serve as their own comparison and reduces the influence of stable individual differences such as typing speed or general computer familiarity.

### Participants
Plan for **6 participants**. Three participants will complete A then B (AB), and three will complete B then A (BA). This meets the assignment’s minimum of five planned participants per condition; because this is a within-subjects design, all six participants use both conditions.

### Target users and eligibility
Target users are adults who use a desktop or laptop and can reasonably relate to managing academic tasks.

Inclusion criteria:
- At least 18 years old.
- Comfortable using a desktop or laptop.
- Able to understand the study instructions.
- Voluntarily provides informed consent.

Do not automatically exclude people who use assistive technology. Provide reasonable accommodations where possible and document any accommodation that could affect the measurements. Exclude project developers and anyone who has already practiced the exact experimental task.

### Counterbalancing matrix

| Participant | Order | Period 1 | Period 2 |
|---|---|---|---|
| P01 | AB | A | B |
| P02 | BA | B | A |
| P03 | AB | A | B |
| P04 | BA | B | A |
| P05 | AB | A | B |
| P06 | BA | B | A |

Use equivalent but different task scenarios in the two periods. Balance scenario assignment across interface and order so that one interface does not always receive the easier or more familiar scenario. Record the actual scenario used in the data sheet.

The order balance is:
- N_AB = 3
- N_BA = 3

This balances which interface is encountered first. It does not eliminate every individual carryover effect, so interpret results cautiously.

## 5. Ethical safeguards

### Participant briefing and consent script
“Thank you for agreeing to participate in this usability study. Today, you will evaluate two designs of a Student Task Manager application. You will be asked to create and save an academic task in each design.

We are evaluating the software interfaces, not your intelligence, computer skills, or personal abilities. There are no right or wrong ways to approach the interface. Mistakes are useful because they help us identify parts of the design that may need improvement.

Your participation is voluntary. You may stop at any time without penalty. We will record task performance information such as completion time, errors, and your ease rating. Your results will be identified by a participant code rather than your name. We will not use real academic records or personal student information.

If screen recording is proposed, it will only occur with your separate permission. Do you have any questions? Do you voluntarily agree to participate?”

Obtain informed consent before starting. Follow any course or institutional research requirements. Do not claim formal ethics approval unless it has actually been granted.

### Privacy and accessibility
- Use participant IDs P01–P06 rather than names in the dataset.
- Use fictional course and assignment information.
- Collect only information needed for the study.
- Store study data in a restricted-access location.
- Obtain separate permission before recording screens or audio.
- Report findings without identifying participants.
- Allow participants to withdraw.
- Check keyboard access, visible focus, labels, contrast, semantic structure, and understandable validation feedback in both interfaces. Consider WCAG 2.1 AA as a design reference.

## 6. Test protocol

### Before each session
1. Prepare the assigned interface order and two equivalent task scenarios.
2. Confirm the same browser, display, keyboard, and mouse are being used.
3. Read the participant briefing and obtain consent.
4. Ask the same short questions about task-manager familiarity.
5. Explain that the participant should work normally and that the interface—not the participant—is being evaluated.

### For each condition
1. Read the task scenario exactly as written.
2. Start timing at the end of the instruction/start cue.
3. Observe without pointing out controls or suggesting actions.
4. Stop timing when the successful save confirmation is visible and the task is verified.
5. Record errors using the same definition for both interfaces.
6. Ask the SEQ question immediately after the task.
7. Record notes and any researcher assistance.

Provide a two-minute break between conditions.

### Standard task instruction
“Imagine that you are a college student who needs to add a new assignment to your task manager. Using the information provided, create a task with the specified title, description, course, due date, and priority. Save the task and verify that it was successfully created. Please work as you normally would. I can clarify the task instructions, but I will not guide you through the interface.”

### Researcher rules
- Do not coach participants or explain where controls are located.
- Do not express approval or disapproval of actions.
- Apply the same error-counting rule in both conditions.
- Record any assistance, interruption, or technical problem.
- Do not pause the timer for ordinary interface interaction.
- If a technical failure prevents a fair test, document it and repeat only under a consistent, predefined procedure.

### Session schedule
Allow approximately 15–20 minutes per participant, including consent, two task attempts, ratings, and debriefing.

## 7. Data analysis plan

For each participant, compare their A and B results.

Report descriptive statistics for completion time, error count, and SEQ rating by interface. Also report task success rates.

For inferential comparisons:
- Use a paired-samples t-test for paired measurements when the paired differences reasonably meet the test’s assumptions.
- Consider a Wilcoxon signed-rank test when those assumptions are not reasonable.
- Report effect sizes and confidence intervals where feasible.
- With only 6 participants, treat the study as exploratory and avoid overstating generalizability.

Do not invent or pre-fill results. Analyze only data actually collected. Consider order and scenario assignment when interpreting differences.

## 8. Post-mortem reflection

### 1. Why distinguish statistical significance from practical significance?
Statistical significance helps indicate whether an observed difference is unlikely to be due to random variation under the test assumptions. Practical significance asks whether the size of that difference matters in real use. For example, a statistically significant two-second improvement may not meaningfully improve a student's workflow. A modest reduction in errors, however, could be operationally important. HCI researchers should consider both statistical evidence and the real-world impact on usability, accessibility, and task performance.

### 2. What carryover effects could occur, and how does counterbalancing address them?
Participants may learn the task requirements during their first attempt and complete the second attempt faster, regardless of interface. They may also experience fatigue or frustration that makes the second attempt slower. In a balanced AB/BA design with three participants in each order, each interface appears first for three participants and second for three participants. This balances the average position of each interface across the sample and helps separate an overall period effect from the interface comparison. It does not mathematically remove all carryover effects, especially asymmetric effects that depend on which interface came first, so these should be acknowledged as a limitation.

## 9. Submission checklist

- [ ] Both Interface A and Interface B are available and have equivalent functionality.
- [ ] `experiment_design/` directory is added to the project repository.
- [ ] This report is included.
- [ ] Research protocol and variable mapping files are included.
- [ ] Data dictionary and blank data collection sheet are included.
- [ ] Scenario assignment is balanced and recorded.
- [ ] Participant consent and study requirements are addressed.
- [ ] Actual data are collected before reporting results.
- [ ] Files are committed and pushed to the public course repository.
