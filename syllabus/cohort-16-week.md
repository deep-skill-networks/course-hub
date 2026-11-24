# Cohort syllabus — 16 weeks, Live + Self-paced

**Cohort size:** 15–25 · **Live:** 3 hrs/week · **Self-paced:** 4–6 hrs/week · **Pods:** 4–5 learners each

## How a week works

| Block | Length | What happens |
|---|---|---|
| Before the session | ~1 hr | Short videos (6–10 min each) and a reading. Concepts are learned here so live time is spent on judgment. |
| Concept & architecture | 60 min | Trade-offs, whiteboarding, predict-then-reveal exercises |
| Build / design review | 60 min | Live capstone work, or critique of learner designs |
| Failure clinic | 60 min | A production incident, revealed in stages; pods race to diagnose it |
| After the session | 3–5 hrs | Labs, capstone milestone, weekly quiz |

Live sessions are split into two 90-minute sessions where possible.

## Pre-work (2–3 weeks, gated)

| Module | Focus | Gate |
|---|---|---|
| P1 Infra bootcamp | Docker, GitHub Actions, Terraform on AWS, Kubernetes basics (on a local kind cluster) | Write a production-grade Dockerfile and Kubernetes manifests; the grader deploys them and checks `/health` end to end |
| P2 ML foundations | Baselines, macro and per-language metrics, word vs character features, leakage, time-based evaluation | The leakage trap: find why a "98% accurate" model fails in production, and report the honest number |

Capstone milestone `ms0`: your capstone repository with CI green and its skeleton deployed to AWS. The P1 and P2 gates and `ms0` are due at the end of week 2. [START-HERE.md](../START-HERE.md) shows the order.

## Weeks 1–16

| Weeks | Module | Key topics | Capstone milestone |
|---|---|---|---|
| 1–2 | **M01** LLM internals & AI problem framing | The FDE role; tokenization and cost; attention, context and KV cache; why outputs are non-deterministic; why hallucination is structural; coding agents and reviewing their work; open and local models | `ms1` Problem brief + solution-ladder justification |
| 3–4 | **M02** ML vs GenAI baselines & cost modelling | Same task three ways (classical ML, prompted LLM, small fine-tuned model); total cost of ownership; automate-or-not scorecard | `ms2` Baseline comparison report |
| 5–6 | **M03** Retrieval & RAG done right | Chunking, embeddings, hybrid search, re-ranking, permission-aware retrieval, retrieval metrics, index lifecycle; when not to use RAG | `ms3` Retrieval with measured recall |
| 7–8 | **M04** Evals, structured outputs, tools & agents | Eval suites and statistics; calibrating LLM judges; harness engineering; agentic RAG and memory; durable state and human approval; multi-agent trade-offs | `ms4` Eval suite + one agent/tool feature |
| 9–10 | **M05** LLMOps: CI/CD, IaC, serving | Versioning prompts/models/indexes; eval-gated CI; canary and rollback; hosted vs self-hosted serving; AI gateways | `ms5` Deployed with IaC and eval-gated CI/CD |
| 11–12 | **M06** Observability, guardrails, security, cost | Tracing with OpenTelemetry; AI SLOs; guardrails; prompt injection and excessive agency; caching, routing and latency | `ms6` Tracing, SLOs, guardrails, threat model |
| 13–14 | **M07** Post-production: drift, online evals, SRE for AI | Silent failure detection; online evals; provider risk; runbooks, incident command, postmortems | `ms7` Online evals, drift alerts, runbooks |
| 15–16 | **M08** FDE in practice, game days & defense | Discovery and scoping; design docs; enterprise integration; incident communication; **game days** on your own system; capstone defense | `ms8` Defense + postmortems |

## The capstone

You build **one system** across all 16 weeks. Pick from approved problem domains, or bring a sanitised problem from your own work. Every capstone must compare at least one classical ML or rules-based approach against an LLM approach.

In weeks 15–16 we inject faults into your running system without warning. You detect them with your own monitoring, communicate with the "client", fix them and write a postmortem.

## Assessment

See [assessments/policy.md](../assessments/policy.md) for weights and certification rules.

## After the course: 12-month alumni phase

Fortnightly sessions (about 26 in the year): production incident teardowns, architecture reviews, quarterly radar briefings and project demos. You'll continue with your pod and pick an alumni project track.
