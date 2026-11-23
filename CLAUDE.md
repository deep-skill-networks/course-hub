# Conventions for Claude sessions in the deep-skill-networks org

This file tells Claude how to work in this repository and its sibling course repos.

## Context
- This is the public front door of the Deep Skill Networks AI Engineering & FDE Program.
- Audience: experienced software engineers. Write for peers: direct, precise, no hype, no filler.
- The mentor's planning knowledge base (program blueprint, module catalog, failure library, templates) lives in the mentor's Claude project, and the build plan (module specs, decisions, roadmap) lives in the mentor's local course plan. Neither is in this repo. Ask for the relevant file if a task depends on it.

## Working rules
- Never commit to `main`. Work on a branch named `<type>/<short-slug>` (types: `setup`, `content`, `lab`, `fix`, `radar`) and open a pull request.
- Keep this repo free of solutions, graded quiz items or answer keys, hidden tests, game-day fault details, learner data, grades, pricing drafts and secrets. Those belong in private repos or the learning platform.
- Grading is automated: never write course material that needs the mentor to mark it by hand. Use autograded tests, structured forms, peer rubrics or calibrated AI-assisted rubric scoring.
- Use course IDs consistently: modules `M01`–`M08`, pre-work `P1`/`P2`, self-paced courses `SP1`–`SP4`, labs `Lxx.y`, failure scenarios `FS-<AREA>-NN`, design cases `SD-NN`, capstone milestones `ms0`–`ms8`, alumni tracks `AP-NN`, case-library entries `CASE-NNN`, bootcamps `BC-NN`.
- Do not hyperlink repos that don't exist yet; write their names in code formatting instead, so the link check stays green.
- Anything that changes quickly (model names, prices, framework versions, spec status) must be checked against a current source and dated. Prefer naming open standards over vendors.
- Indian context matters: costs in ₹ alongside $, DPDP Act for privacy, Indic and code-mixed language examples.

## Style
- Sentence-case headings. Short paragraphs. Tables where readers will compare.
- British/Indian English spelling is fine; be consistent within a file.
- Every new markdown file must be linked from somewhere (README, a folder README, or `repos.md`).
- Every repo's README ends with the standard "About the mentor" footer from this repo's README. Other repos reference the logo by its absolute URL in this public repo rather than copying it.
- No pricing or fees anywhere in GitHub; they live in the enrolment platform. No cohort dates either: repos use week numbers (week 1–16) so they can be reused by every cohort; dates live in each cohort's calendar.
