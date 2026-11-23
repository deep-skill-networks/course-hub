# Repository map

All course code lives in the [`deep-skill-networks`](https://github.com/deep-skill-networks) GitHub organization. Each repository is small enough to clone and finish in a sitting or a week. There is deliberately no single giant repo.

Repositories marked *planned* don't exist yet; they are written without links until they do.

| Repository | Purpose | Visibility | Status |
|---|---|---|---|
| `course-hub` (this repo) | Program overview, syllabus, setup, radar, case library | Public | Live |
| `prework-infra-bootcamp` | P1: Docker, GitHub Actions, Terraform/OpenTofu, Kubernetes, one cloud | Learners | Planned |
| `prework-ml-foundations` | P2: classical ML, metrics, leakage | Learners | Planned |
| `m01-llm-internals-and-framing` | M01 labs, notes, quizzes | Learners | Planned |
| `m02-ml-vs-genai-baselines` | M02 | Learners | Planned |
| `m03-rag-done-right` | M03 | Learners | Planned |
| `m04-evals-and-agents` | M04 | Learners | Planned |
| `m05-llmops-cicd` | M05 | Learners | Planned |
| `m06-observability-guardrails` | M06 | Learners | Planned |
| `m07-drift-and-online-evals` | M07 | Learners | Planned |
| `m08-fde-in-practice` | M08 | Learners | Planned |
| `capstone-template` | Template you create your own capstone repo from; milestone tags `ms0`–`ms8` | Learners | Planned |
| `shared-toolkit` | Reusable eval harness, tracing setup, Terraform modules, fault-injection library, quiz exporter | Learners | Planned |

Instructor-only repositories (solutions and game-day scenarios) also exist and are private.

## What's inside a module repository

```
mNN-<slug>/
├── README.md          # objectives, prerequisites, time and cost estimates, video links
├── .devcontainer/     # one-click environment (Codespaces or local)
├── labs/              # one folder per lab: starter code + instructions
├── notes/             # session notes and slide outlines
├── handouts/          # cheat sheets and one-pagers
├── quizzes/           # quiz items (YAML, single source of truth)
├── case-studies/      # incident replays: telemetry + brief
├── tests/             # autograder (behaviour checks)
├── config/models.yaml # provider and model in one place, with a local fallback
└── .github/workflows/ # grading on every push + nightly "does this still run?" check
```

Each lab has two tags: `labNN-start` (where you begin) and `labNN-end` (a reference point, released after the deadline for cohorts). If you get stuck, you can check out the next lab's start tag and keep going.

## How learner access works

- **Cohort learners** are added to a GitHub team for their cohort (for example `cohort-2027-01`), which grants read access to the module repositories for the duration of the course and alumni year.
- **Your own work** goes in your own repository: you create your capstone from `capstone-template` using GitHub's "Use this template" button, and do labs in your own copy of each module repo. Make these repositories private unless you want them in your public portfolio.
- **Grading** runs as GitHub Actions in your repository. A green check means the autograder passed; the details are in the workflow log.
- **Self-paced learners** get access to the repositories for the courses they've purchased.

We don't use GitHub Classroom, which GitHub shut down in August 2026. Templates, teams and Actions-based grading do the same job with standard GitHub features.
