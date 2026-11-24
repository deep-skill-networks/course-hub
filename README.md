# Deep Skill Networks — AI Engineering & FDE Program

A production-first program for **experienced software engineers** moving into AI roles: Forward Deployed Engineer (FDE), AI Engineer, LLM Engineer, MLOps/LLMOps, and AI Platform/SRE.

Most AI courses stop at the demo. This one starts there. You will build a real system, prove it works with evaluations, deploy it reproducibly, watch it degrade in production, and fix it before the client notices.

> **Graduate profile:** You can walk into a client, scope an AI problem, pick the cheapest adequate solution, deploy it reproducibly, prove it works with evals, detect when it degrades, and lead the incident response.

---

## What makes this program different

- **Judgment before tools.** You will learn when *not* to use GenAI. Classical ML, rules, or no automation at all is often the right answer, and you'll prove it with cost and accuracy data.
- **Production failure is the curriculum.** Every module includes deliberately broken systems to diagnose and fix. Most failures are *silent*: the service returns HTTP 200 with a wrong answer.
- **One evolving capstone.** Instead of disconnected toy projects, you build one system for 16 weeks, then defend it to a "client" while we inject faults into it.
- **Fast, automatic feedback.** Quizzes and labs are graded automatically, usually within minutes, and every answer comes with an explanation, so you always know where you stand.
- **Foundations over hype.** Roughly 50% durable foundations, 35% patterns, 15% specific tools. A quarterly [technology radar](radar/README.md) keeps the tool layer current.

## Two ways to learn

| | Cohort (Live + Self-paced) | Fully Self-paced |
|---|---|---|
| Availability | Enrolling now: [program page](https://sanjaynegi.in/programs/) | **Coming soon.** [Join the free community](https://learn.sanjaynegi.in/l/adff39aacd) for free bootcamps and early access |
| Format | 16 weeks + 2–3 weeks of pre-work | Four stackable 4-week courses (SP1–SP4) |
| Live time | 3 hrs/week, in a batch of up to 15 | Monthly office hour |
| Pacing | Weekly deadlines with your cohort | Monthly start dates with peers at the same point (or start any time) |
| Self-paced work | 4–6 hrs/week | ~7–9 hrs/week |
| Capstone | One system built across all modules, defended at the end | A mini-capstone per course, which is also your final practical |
| Failure training | Live failure clinics + game days on your own system | Break-fix labs + incident replays |
| After the course | 12 months of fortnightly alumni sessions | Community channel. The 12-month alumni year unlocks when you complete all four courses, or as an upgrade |
| Details | [syllabus/cohort-16-week.md](syllabus/cohort-16-week.md) | [syllabus/self-paced-sp1-sp4.md](syllabus/self-paced-sp1-sp4.md) |

Please be realistic about time. Both formats ask for about **7–9 hours per week** in total. Learners who plan for that finish; learners who plan for 3 usually don't.

## Curriculum at a glance

| # | Module | You will be able to… |
|---|---|---|
| P1 | Infra bootcamp (pre-work) | Containerise, run CI, provision with Terraform, deploy to Kubernetes |
| P2 | ML foundations (pre-work) | Build and honestly evaluate a classical ML baseline |
| M01 | LLM internals & AI problem framing | Explain why LLMs behave as they do; frame a problem before choosing a technique |
| M02 | ML vs GenAI baselines & cost modelling | Show with data when classical ML beats an LLM; model total cost |
| M03 | Retrieval & RAG done right | Design, measure and debug retrieval |
| M04 | Evals, structured outputs, tools & agents | Build release-gating evals; design agents that fail safely |
| M05 | LLMOps: CI/CD, IaC, serving | Ship AI changes as safely as code changes |
| M06 | Observability, guardrails, security, cost & latency | See inside an AI system and defend it |
| M07 | Post-production: drift, online evals, SRE for AI | Catch degradation before the client does; run an incident |
| M08 | FDE in practice, game days & capstone defense | Run a client engagement end to end under pressure |

## Who this is for

- Software engineers, architects, SREs and tech leads with roughly 5+ years of experience.
- Comfortable with Python, Git, and deploying a web service. You do **not** need prior ML experience; the pre-work covers it.

## Getting started

**New here? Read [START-HERE.md](START-HERE.md) first.** It walks you through the whole program in order: setup, pre-work, the weekly routine and what happens after.

1. Read the [prerequisites](setup/prerequisites.md) and set up your accounts and tools.
2. Review [API keys and costs](setup/api-keys-and-costs.md). Every lab has a low-cost or free local-model path.
3. See the [repository map](repos.md) to understand how the course code is organised.
4. Keep the [glossary](glossary.md) handy.

## Repository contents

| Path | What it holds |
|---|---|
| [`START-HERE.md`](START-HERE.md) | Your path through the program, step by step |
| [`syllabus/`](syllabus/) | Week-by-week plans for both formats |
| [`setup/`](setup/) | Prerequisites, accounts, budgets |
| [`repos.md`](repos.md) | Map of every course repository and how access works |
| [`glossary.md`](glossary.md) | Terms used across the course |
| [`radar/`](radar/) | Quarterly technology radar: what to adopt, trial, assess or hold |
| [`case-library/`](case-library/) | Anonymised production incident case studies |
| [`assessments/`](assessments/) | Grading, certification and academic honesty policy |

## Questions and corrections

Batches, timings and fees are on the [program page](https://sanjaynegi.in/programs/).

Found a mistake or a broken link? [Open an issue](https://github.com/deep-skill-networks/course-hub/issues/new/choose). Corrections from learners are welcome and credited.

---

## About the mentor

**Sanjay Negi** brings 22+ years of industry experience and helps experienced software engineers and technology leaders transition into high-value AI roles, including **AI Engineer**, **Forward Deployed Engineer** and **GenAI Architect**. He has trained more than 1,100 experienced engineers.

<p align="center">
  <img src="assets/brand/skillupwithsanjay.png" alt="SkillUp with Sanjay logo" width="60">
</p>

<p align="center"><strong>#SkillUpWithSanjay</strong></p>

<p align="center">
  <a href="https://sanjaynegi.in/programs/" target="_blank" rel="noopener noreferrer"><strong>Join the program</strong></a>
  &nbsp;&middot;&nbsp;
  <a href="https://learn.sanjaynegi.in/l/adff39aacd" target="_blank" rel="noopener noreferrer">Free bootcamps</a>
  &nbsp;&middot;&nbsp;
  <a href="https://www.sanjaynegi.in" target="_blank" rel="noopener noreferrer">Website</a>
  &nbsp;&middot;&nbsp;
  <a href="https://www.linkedin.com/in/sanjay-negi-ai/" target="_blank" rel="noopener noreferrer">LinkedIn</a>
</p>
