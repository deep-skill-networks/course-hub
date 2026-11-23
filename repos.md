# Repository map

All course code lives in the [`deep-skill-networks`](https://github.com/deep-skill-networks) GitHub organization. Each repository is small enough to clone and finish in a sitting or a week. There is deliberately no single giant repo.

Repositories marked *planned* don't exist yet. Course repositories are private to enrolled learners, so they're written without links; you'll get access when you enrol. `shared-toolkit` is public: anyone can read and install it.

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
| `capstone-template` | Template your capstone repository is created from; you tag milestones `ms0`–`ms8` as you reach them | Learners | Live |
| [`shared-toolkit`](https://github.com/deep-skill-networks/shared-toolkit) | Reusable eval harness, tracing setup, Terraform modules, fault-injection library, practice fault packs, quiz exporter | Public | Live |

Instructor-only repositories (solutions, graded quizzes, hidden tests and game-day scenarios) also exist and are private.

## What's inside a module repository

```
mNN-<slug>/
├── README.md          # objectives, prerequisites, time and cost estimates, video links
├── .devcontainer/     # one-click environment (Codespaces or local)
├── labs/              # one self-contained folder per lab: starting code + instructions
├── notes/             # session notes and slide outlines
├── handouts/          # cheat sheets and one-pagers
├── practice/          # ungraded practice questions with answers
├── case-studies/      # incident replays: telemetry + brief
├── replay/            # recorded traffic for generating realistic telemetry
├── tests/             # public autograder tests (instant feedback)
├── config/models.yaml # provider and model in one place, with a local fallback
└── .github/workflows/ # feedback on every push, including a secret scan
```

Each lab folder has its own starting point, so you can start any lab even if you got stuck on the previous one. Reference solutions are released automatically after each deadline. Graded quizzes run in the learning platform, not in these repositories.

## How learner access works

- **Your repositories are created for you.** When you enrol (cohort) or buy a course (self-paced), we create your own private copies inside the `deep-skill-networks` organization: one capstone repository and one lab repository per module. You get write access; there's nothing to fork or set up.
- **You submit by pull request.** Open one pull request per lab or milestone. Put a one-line note on any significant AI assistance in the description.
- **Feedback is instant; grading is automatic.** Public tests run on every push so you can see how you're doing. The official grade comes from a separate grader that also runs hidden tests; the result is posted as a comment on your pull request, usually within an hour, and recorded in the learning platform.
- **What you keep.** After the course you may copy your capstone to your own account and make it public for your portfolio. Lab repositories stay private so solutions don't circulate.
- **Cohort learners** keep read access to the module repositories through the alumni year. **Self-paced learners** keep access to the courses they've bought.

The capstone template deploys to **AWS** (Lambda + ECR, built with Terraform, region `ap-south-1`); use your own AWS account with a budget alert.

We don't use GitHub Classroom, which GitHub shut down in August 2026. Templates, teams and Actions-based grading do the same job with standard GitHub features, and repository creation is automated for you.
