# Assessment and certification policy

Assessments here exist mainly to help you learn. Retrieval practice and feedback are some of the most reliable ways to make knowledge stick, so quizzes allow two attempts, every answer comes with an explanation, and labs give you feedback on every push.

## Cohort (Live + Self-paced)

| Component | When | Weight | How it's assessed |
|---|---|---|---|
| Diagnostic pre-test | Before week 1 | 0% | 30 questions; repeated at the end to measure your progress |
| Live session check-ins | Every session | 0% | Short polls, for participation and feedback |
| Weekly quizzes | Weekly | 15% | 10–12 scenario questions, two attempts (best counts), including three review items from earlier modules. Scored instantly |
| Labs | Weekly | 20% | Autograded with public and hidden tests; pass/fail with credit for stretch goals |
| Break-fix labs and incident replays | ~6 across the course | 15% | Break-fix: autograded (symptom gone, a new automated check added, and that check catches the fault). Replays: structured diagnosis form plus a short written reasoning answer |
| Design reviews | M03, M05, M08 | 15% | Rubric: framing, requirements, soundness, failure modes, operations plan, trade-offs. Scored by three peers and an AI-assisted rubric score; your score is the median |
| Capstone milestones `ms1`–`ms7` | Every two weeks | 15% | Automated milestone checks in CI, plus a required pod-mate review |
| Game day and capstone defense | M08 | 20% | Detection and recovery times measured automatically; defense scored live by a panel (mentor and two peers) against a rubric covering architecture, evals, production readiness, detection, incident handling and client communication |

**Certificate:** a weighted score of at least 70%, all milestones submitted, and the capstone defended.
**With distinction:** at least 85%, and you detected the hardest game-day faults through your own monitoring.

## Fully self-paced (each of SP1–SP4)

- At least 70% across quizzes
- Every lab passed
- A final practical: your mini-capstone (an autograded lab) plus one incident-replay diagnosis

Completing all four courses earns the program certificate.

## How grading works

Grading is automatic so you get feedback fast, whatever the time of day.

- **Quizzes** are scored instantly in the learning platform.
- **Labs and milestones:** public tests run on every push for instant feedback. When you open your pull request, a separate grader runs the official public and hidden tests and posts your result as a comment, usually within an hour. Editing the tests in your repository doesn't change your grade.
- **Written answers and designs** are scored against the published rubrics by peers and by an AI model that we calibrate against human-scored examples before each cohort. For designs, the AI score is one of four scores and the median counts. Your submissions are sent only to AI providers whose terms exclude training on submitted data.
- **Appeals:** if you think a score is wrong, appeal in the learning platform within 7 days. Labs are re-run and designs get an extra peer review; anything still unresolved goes to the mentor.

## Deadlines and extensions

- Cohort milestones are due at the end of their module's second week. Self-paced learners on a monthly start date get weekly soft deadlines.
- You can resubmit a lab as often as you like until the deadline.
- One no-questions-asked extension of one week is available per learner per course. Use the extension form in the learning platform; it applies automatically.
- If you miss a deadline or two sessions in a row, you'll get an automatic reminder, then a nudge from your pod buddy. If it happens again, the mentor will get in touch. That's support, not a penalty.

## Using AI tools
You're training to work alongside AI tools, so using them is allowed and expected: coding agents, chat assistants, anything. The rules:
1. **You must understand and be able to explain everything you submit.** Design reviews and the defense will test this.
2. **Disclose significant AI help** in your pull request description (one line is enough).
3. **Incident diagnoses must show your reasoning**, not just the answer.

## Academic honesty
- Don't share lab solutions or game-day details outside your cohort. Keep your lab repositories private; you may make your capstone public after the course.
- Discussing approaches with your pod is encouraged. Submitting someone else's work as your own is not.
- Breaches may lead to loss of credit for the work and, if repeated, removal from the program.
