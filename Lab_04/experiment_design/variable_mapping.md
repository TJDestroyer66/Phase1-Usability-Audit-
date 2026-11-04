# Variable Mapping – Student Task Manager Experiment

## Independent variable

| Variable | Type | Levels | Description |
|---|---|---|---|
| Interface | Primary independent variable | A, B | A = traditional single-page form; B = guided multi-step wizard |

## Dependent variables

| Variable name | Role | Operational definition | Data type / unit |
|---|---|---|---|
| Task_Completion_Time_sec | Efficiency | Elapsed time from start cue until verified successful save; cap at 300 seconds for a five-minute limit | Numeric, seconds |
| Error_Count_Total | Effectiveness | Incorrect entries, rejected submissions, and participant corrections | Integer count |
| Task_Success_Binary | Effectiveness | 1 if task is saved and verified; otherwise 0 | Binary integer |
| SEQ_Rating | Subjective ease | Response to “Overall, how easy or difficult was this task?” | Integer, 1–7 |

## Confounds and controls

| Potential confound | Control |
|---|---|
| Prior task-manager familiarity | Ask the same pre-study familiarity questions; record responses |
| Typing/computer experience | Record relevant experience; use same computer and peripherals |
| Browser/display variation | Same browser/version and 1920 × 1080 display |
| Environmental distractions | Same quiet location where practical |
| Learning/order effects | Three AB and three BA sequences |
| Fatigue | Two-minute break between conditions |
| Scenario difficulty | Equivalent scenarios; balance assignment and record scenario |
| Network/system latency | Run locally where possible; keep save behavior equivalent |
| Researcher influence | Fixed instructions; no coaching |

## Other recorded fields

| Variable | Purpose |
|---|---|
| Participant_ID | Anonymous participant code |
| Presentation_Order | AB or BA |
| Period | 1 or 2 |
| Task_Scenario | Scenario assigned in that trial |
| Researcher_Assistance | Count of interventions |
| Researcher_Notes | Interruptions, technical problems, and qualitative observations |

## Measurement rules
- Start timing at the standardized start cue.
- Stop when the saved task is visibly verified, or at 300 seconds.
- Count errors consistently in both conditions.
- Ask the SEQ question immediately after each condition.
- Do not fabricate or pre-fill participant results.
