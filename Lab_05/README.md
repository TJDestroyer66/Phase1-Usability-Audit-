# StudyFlow Usability Test Protocol and SUS Instrument

## 1. Study overview

**Project:** StudyFlow – Student Task Manager  
**Research question:** Does a guided, multi-step task-creation wizard (Interface B) improve usability compared with a traditional single-page task-creation form (Interface A)?  
**Study type:** Moderated, within-subjects usability study using concurrent think-aloud (CTA).  
**Recruitment target:** 3–5 participants who represent likely student users.  
**Estimated session length:** 25–35 minutes per participant.

### Interfaces
- **Interface A – Baseline:** traditional single-page task form.
- **Interface B – Wizard:** guided task creation with Details → Review → Done, validation, and success confirmation.

Use the same underlying task fields and equivalent task scenarios in both interfaces. Do not change the task requirements between conditions.

### Study design and order
Each participant completes both scenarios, one in each interface. Counterbalance order to reduce learning and order effects:
- Odd-numbered participant IDs: Scenario A in Interface A, then Scenario B in Interface B.
- Even-numbered participant IDs: Scenario A in Interface B, then Scenario B in Interface A.

With only 3–5 participants, treat results as formative and descriptive rather than statistically conclusive. Report individual results, medians, ranges, and observed patterns. Do not claim statistical significance from this small sample.

## 2. Study scope and task scenarios

### Task 1 – Add a course task (Scenario A)
"You have just received a new assignment for your Human-Computer Interaction course. It is called 'Accessibility Review'. Add it to your task list with a short description explaining that you need to review the course website for accessibility issues. Set the due date to [provide a date at least seven days in the future] and choose a priority that reflects the importance of completing it on time. Finish when you believe the task has been saved."

### Task 2 – Add a programming task (Scenario B)
"You have just been assigned a programming exercise for your Software Engineering course. It is called 'Unit Testing Exercise'. Add it to your task list with a short description explaining that you need to write and run unit tests for the assigned code. Set the due date to [provide a different date at least seven days in the future] and choose a priority that reflects the importance of completing it on time. Finish when you believe the task has been saved."

**Moderator preparation:** Before each session, confirm the two course names are available in both interfaces. Select future dates that are valid in the test environment. If course names or dates differ in the deployed prototype, substitute equivalent available values while preserving the scenario requirements. Do not read interface labels or tell participants where to click.

## 3. Participant screener

Recruit 3–5 participants who are plausible student task-manager users. Ask the following neutral questions. Do not collect names in the research dataset.

1. **How often do you use a website or app to organize school, work, or personal tasks?**  
   - Daily / Several times a week / About once a week / Less than once a week / Never
2. **How comfortable are you using a new website or app without help?**  
   - Not at all comfortable / Slightly comfortable / Moderately comfortable / Very comfortable / Extremely comfortable
3. **Which age range are you in?**  
   - 18–24 / 25–34 / 35–44 / 45–54 / 55 or older / Prefer not to say
4. **Do you use any accessibility features or assistive technologies when using a computer or mobile device?**  
   - No / Yes / Prefer not to say  
   If yes and they wish to share: screen reader, magnification, voice control, captions, keyboard-only navigation, other.
5. **Which device/input methods do you commonly use for web tasks?**  
   - Laptop/desktop with mouse / Laptop/desktop with keyboard only / Touchscreen / A combination / Other

**Recruitment guidance:** Aim for variation in age range, task-management frequency, device/input method, and voluntary accessibility-feature use. Do not exclude someone solely for using assistive technology. Confirm that the prototype and test environment can support their access needs before scheduling. For this formative study, prioritize people who use digital interfaces and can plausibly represent student users. Record only the minimum demographic information needed.

## 4. Moderator preparation checklist

Before the participant arrives:
- [ ] Confirm both interfaces load and have equivalent task fields.
- [ ] Reset both interfaces to a clean state; remove prior test tasks.
- [ ] Confirm course options and future due dates.
- [ ] Prepare participant ID (P01–P05); do not put names in filenames or logs.
- [ ] Open the observation workbook and prepare a timer.
- [ ] Confirm the participant has agreed to any screen/audio recording.
- [ ] Check that the participant can use their preferred input/accessibility technology.
- [ ] Keep the same device, browser, viewport, and network conditions where feasible.
- [ ] Assign the counterbalanced order before the session.

## 5. Informed consent and pre-test briefing script

Read this script consistently:

"Thank you for taking part. Today we are evaluating two versions of a student task-management interface. We are testing the design, not you. There are no right or wrong ways to use the system, and any difficulty you encounter is useful information about the interface.

Taking part is completely voluntary. You may pause, skip a question, or stop the session at any time without penalty or having to give a reason. Your decision will not affect your course standing or relationship with the research team.

With your permission, we would like to record the screen and, if separately agreed, audio so we can accurately review interactions and comments. We will also take notes about task progress and interface behavior. Research records will use a participant code rather than your name. Files will be stored in the team's access-restricted project storage, shared only with authorized project members, and used for this class research. We will remove direct identifiers from analysis files and will not include identifiable recordings in public repository materials. Recordings will be deleted after the project review period, or earlier if required by course policy. You may decline recording and still participate if the study can be conducted with notes only.

Do you have any questions? Do you agree to participate? Do you separately agree to screen recording? Do you separately agree to audio recording?"

**Consent record:** Record yes/no for participation, screen recording, and audio recording in a restricted consent record stored separately from the analysis workbook. Do not place signed consent forms or identifying information in the public GitHub repository. Follow instructor/institutional requirements if they specify a retention period or consent form.

## 6. Concurrent think-aloud instructions

Read verbatim:

"As you work through each task, please say out loud what you are thinking. You can describe what you expect to happen, what you are looking for, what you think a control will do, and anything that seems confusing or surprising. You do not need to explain every action. I may occasionally remind you to keep talking, but I will not tell you where to click or how to complete the task."

Allowed neutral reminder, only after a period of silence:
- "Please keep talking."
- "What are you thinking right now?"

Do not:
- suggest a control, label, navigation path, or next action;
- praise or criticize a choice ("good", "that's right", "almost");
- answer questions about how the interface works;
- point, lean toward, or look conspicuously at the correct control;
- rush the participant or communicate frustration.

If asked for help, say: "Please do what you would naturally do if I were not here. I can clarify the task wording, but I cannot guide you through the interface." If the participant cannot proceed and requests help, provide the minimum necessary prompt, record the exact assistance, and score the task as assisted (0.5) if they ultimately complete it.

## 7. Task administration and neutral handouts

Give one scenario at a time. Read the scenario exactly as written in Section 2. Start timing immediately after finishing the prompt. Stop timing when the participant performs the terminal action that indicates the task is complete (for example, saves/submits and reaches a confirmation or the task is visibly present in the list). If the participant declares completion but the system has not saved the task, continue timing until the terminal action or declare failure at the session limit.

**Time limit:** Use a consistent 5-minute maximum per task. If the participant reaches the limit without completion, stop the task and record terminal failure (0). Do not silently extend the limit for one participant.

After each task, ask:
"Overall, how easy or difficult was this task to complete?"

SEQ response scale:
1 Very difficult | 2 | 3 | 4 Neither easy nor difficult | 5 | 6 | 7 Very easy

Then administer the SUS instrument for that interface after the participant has completed the task associated with that interface. If the participant completes two tasks in one interface, administer SUS once after the interface's tasks, not after every task. Keep the questionnaire wording and response order identical.

## 8. Performance metrics and operational definitions

| Variable | Definition / rule |
|---|---|
| Task_Time_sec | Seconds from end of scenario prompt to terminal user action. Use the same start/stop rule for every participant. |
| Task_Success | 1 = completed independently; 0.5 = completed after moderator assistance/prompt; 0 = terminal failure or time limit reached. |
| Error_Count | Count discrete observable errors: wrong navigation destination, dead click/nonresponsive control activation, invalid or rejected input, or an action that must be reversed because it was incorrect. Count each distinct occurrence once. Do not count normal exploration as an error unless it meets a rule above. |
| SEQ | Single Ease Question rating, 1–7, collected immediately after each task. |
| SUS | Ten-item standardized questionnaire, collected separately for each interface. |

**Terminal action:** successful save/submit followed by visible confirmation or evidence that the task appears in the task list.  
**Assistance:** any moderator guidance beyond the standardized neutral think-aloud reminder or clarification of task wording.  
**Error-count consistency:** log the event and timestamp or brief description so another reviewer can audit the count. Do not infer an error from facial expression alone.

## 9. Observation log fields

For each task, record:
- participant ID, interface, task ID, condition order;
- start time, end time, elapsed seconds;
- success level, error count, SEQ;
- navigation missteps, dead clicks, input errors;
- facial expressions (observable description only, e.g., "frowned and paused"; do not infer emotion);
- verbalized friction (brief exact quote where possible);
- physical hesitation (e.g., hand stopped above mouse, repeated scanning);
- ergonomic/posture adjustments (e.g., moved closer to screen, changed grip);
- moderator assistance and exact wording;
- additional notes.

Avoid subjective labels such as "confused" unless supported by a participant statement or observable behavior. Do not record sensitive personal details.

## 10. SUS questionnaire instrument

Use `sus_survey.html` for the digital instrument. The ten canonical items and alternating polarity are preserved. Participants answer each item on a five-point scale:
1 Strongly Disagree · 2 Disagree · 3 Neither Agree nor Disagree · 4 Agree · 5 Strongly Agree.

**Administration:** Refer to the tested version as "this system" consistently. Administer one complete SUS after Interface A and another complete SUS after Interface B. Do not change item wording, scale direction, or item order. Avoid explaining what a participant should answer.

### SUS scoring
For each participant and each interface:
- Odd items (1, 3, 5, 7, 9): contribution = response − 1.
- Even items (2, 4, 6, 8, 10): contribution = 5 − response.
- Sum the ten contributions (range 0–40).
- SUS = sum × 2.5 (range 0–100).

A higher score indicates better perceived usability. SUS is not a percentage. Do not interpret it as a percent correct. Preserve item-level responses and calculate the total from the raw data. Do not impute missing answers; ask the participant to complete any accidentally skipped item if they are willing. If an item remains missing, mark that SUS record incomplete and do not calculate a total.

## 11. Accessibility-first survey and environment audit

The included HTML questionnaire uses native radio groups and explicit labels. Before deployment, test the actual hosted page with keyboard-only navigation and at least one screen reader/browser combination available to the team.

| Check | Acceptance criterion |
|---|---|
| Programmatic labels | Every question has a `fieldset`/`legend`; every radio input has an associated `label` with matching `for` and `id`. |
| Keyboard operation | Tab reaches each group; arrow keys move among radio options; Space selects; keyboard focus is clearly visible. |
| Focus visibility | Visible focus indicator is not removed and is distinguishable against the page background (WCAG 2.1 SC 2.4.7). |
| Contrast | Normal text and rating labels have at least 4.5:1 contrast against their backgrounds (WCAG 2.1 SC 1.4.3). |
| Required responses | Missing answers are identified in text; an error summary/status uses `role="alert"` or `aria-live="polite"` and focus is moved to the first unanswered group when appropriate. |
| Zoom/reflow | At 200% zoom and narrow viewport, questions and options remain readable without horizontal scrolling for ordinary content. |
| Screen reader | Question legend, item number/text, and selected response are announced in a logical order. |
| Touch target | Radio controls/labels are comfortably clickable and do not require precise pointer movement. |

The presence of accessible markup does not by itself prove WCAG conformance. Document the browser, assistive technology, and manual checks actually performed. Do not claim full WCAG 2.1 AA compliance until verified.

## 12. Data handling and analysis plan

- Use participant IDs P01–P05. Keep consent records separately from research data.
- Store raw observation data and questionnaire exports in access-restricted project storage.
- Public repository should contain blank templates and de-identified protocol materials only; never commit names, consent forms, raw recordings, or identifiable participant data.
- Preserve raw observations. Do not overwrite raw values with calculated values.
- Summarize each interface using per-participant values, median and range for time, error count, SEQ, and SUS. Report completion proportions and assistance levels.
- With 3–5 participants, use descriptive comparisons and qualitative themes. Treat findings as exploratory; the sample is too small to support strong population-level claims.

## 13. Post-mortem reflection

### 1. Why does SUS alternate positive and negative phrasing?
The alternating positive and negative wording helps reduce acquiescence bias, the tendency for respondents to agree with statements regardless of their actual opinion. Because the respondent must consider both favorable and unfavorable statements, the pattern can encourage more attentive responses and make straight-lining less likely. It does not eliminate response bias, so item wording and order must remain standardized and scoring must reverse-code the negative items correctly.

### 2. How can moderator cues corrupt task-time and error data?
A moderator's gaze, pointing, facial expression, tone, or leading question can signal the intended control or next step. This may shorten task time, prevent an error, or cause a participant to change course, making performance appear better than it would be independently. The protocol prevents this by using a fixed script, neutral reminders only, a consistent timing rule, no directional help, and explicit logging of any assistance. The moderator remains still and neutral, avoids looking toward target controls, and records deviations so affected results can be interpreted appropriately.

## 14. Repository submission checklist

Recommended repository layout:

```text
repository-root/
├── README.md
├── empirical_usability/
│   ├── usability_logging_sheet.xlsx
│   ├── usability_logging_template.csv
│   └── sus_survey.html
└── (existing StudyFlow prototype files)
```

Before submitting:
- [ ] Add this protocol to the public course repository as `README.md` or export it as `Usability_Protocol_SUS.pdf`.
- [ ] Add the blank Excel/CSV observation template under `empirical_usability/`.
- [ ] Deploy `sus_survey.html` using GitHub Pages or another approved hosting platform.
- [ ] Open the deployed survey URL in a private/incognito window and test all ten items, validation, scoring, and CSV export.
- [ ] Complete and document the accessibility audit; do not claim untested conformance.
- [ ] Confirm no participant-identifying information is in the public repository.
- [ ] Submit the repository URL and live survey URL in Canvas, following the instructor's exact submission field requirements.
