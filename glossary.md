# Glossary

Terms used across the course. Short definitions here; each is taught properly in the module noted.

| Term | Meaning | Module |
|---|---|---|
| **ADLC** | Agent development lifecycle: spec → plan → agent implements → human reviews → tests and evals | M01 |
| **Agent** | A system where the model chooses which steps and tools to use. Compare *workflow*. | M04 |
| **AI gateway** | A central layer in front of model providers for auth, quotas, routing, fallback, caching, redaction and cost attribution | M05 |
| **Autograder** | Automated tests that check a lab submission's behaviour | All |
| **Canary release** | Sending a small share of traffic to a new version before full rollout | M05 |
| **Cascade** | Routing most traffic to a cheap model and escalating only low-confidence cases to an expensive one | M02 |
| **Chunking** | Splitting documents into pieces for indexing and retrieval | M03 |
| **Context window** | The maximum number of tokens a model can consider at once | M01 |
| **Cost per successful task** | Total cost (tokens, infrastructure, human review, maintenance) divided by tasks completed correctly, not by requests | M02 |
| **Data drift / concept drift** | Inputs change (data drift), or the relationship between inputs and the right answer changes (concept drift) | M07 |
| **DPDP Act** | India's Digital Personal Data Protection Act, 2023, and its 2025 Rules | M06, M08 |
| **Durable execution** | Running long workflows so they survive crashes and resume from checkpoints | M04 |
| **Embedding** | A vector representation of text (or other data) where similar meanings are close together | M03 |
| **Error budget** | The amount of unreliability an SLO allows before releases slow down | M06 |
| **Eval / golden set** | A versioned set of test cases with expected outcomes used to measure quality | M04 |
| **Excessive agency** | An agent with more permissions or autonomy than its task needs | M06 |
| **FDE** | Forward Deployed Engineer: an engineer embedded with a client to take a product from problem to production | M01, M08 |
| **Game day** | A planned exercise where faults are injected into a running system to practise detection and response | M08 |
| **Groundedness / faithfulness** | Whether an answer is supported by the retrieved sources | M03 |
| **Guardrails** | Checks on inputs and outputs: validation, PII redaction, topic limits, policy enforcement | M06 |
| **Hallucination** | Fluent output that isn't supported by facts or sources | M01 |
| **Harness** | The code around a model: the agent loop, context assembly, tools, retries, verification | M04 |
| **Hidden tests** | Autograder tests you can't see, run by the official grader so that passing reflects the skill rather than the visible tests | All |
| **HITL** | Human in the loop: a person approves, corrects or decides at defined points | M02, M04 |
| **Hybrid search** | Combining keyword search (such as BM25) with vector search | M03 |
| **Idempotency** | An operation that has the same effect if run once or several times | M04 |
| **Incident replay** | A case study where you diagnose a failure from exported traces, metrics and logs | All |
| **KV cache** | Stored attention keys and values that speed up generation but consume memory as context grows | M01 |
| **LLM-as-judge** | Using a model to score outputs against a rubric; must be calibrated against human labels | M04 |
| **MCP** | Model Context Protocol: an open protocol for connecting models to tools and data | M04 |
| **Milestone** | One of the capstone checkpoints `ms0`–`ms8`, roughly every two weeks | All |
| **MRR / nDCG** | Ranking metrics for retrieval: MRR rewards putting the first relevant result high; nDCG scores the whole ranking with graded relevance | M03 |
| **MTTD / MTTR** | Mean time to detect / mean time to resolve | M07 |
| **OHIFP** | Our debugging method: Observe → Hypothesise → Isolate → Fix → Prevent | All |
| **Online eval** | Evaluating a sample of real production traffic continuously | M07 |
| **OpenTelemetry (OTel)** | Open standard for traces, metrics and logs; includes GenAI conventions | M06 |
| **p95 / p99** | The latency (or other value) that 95% / 99% of requests stay under; better than averages for user experience | M02, M06 |
| **Pod** | A fixed group of 4–5 learners who review each other's work and keep each other on track, through the alumni year | All |
| **Postmortem** | A blameless written analysis of an incident with action items | M07 |
| **Prompt injection** | Input that makes a model follow an attacker's instructions. *Indirect* injection arrives through content such as documents or web pages. | M06 |
| **Quantisation** | Storing model weights at lower precision to cut memory and cost, with some quality trade-off | M01, M05 |
| **RAG** | Retrieval-augmented generation: retrieving relevant content and giving it to the model as context | M03 |
| **Re-ranking** | A second, more precise model reorders retrieved results | M03 |
| **Recall@k** | The share of relevant items that appear in the top *k* retrieved results | M03 |
| **Red-teaming** | Deliberately attacking your own system (for example with prompt injection) to find weaknesses before someone else does | M06 |
| **Runbook** | Step-by-step instructions for handling a known type of incident | M07 |
| **Semantic caching** | Reusing a stored answer for a new request that is similar, not identical; cheap but risky without a strict threshold and evals | M06 |
| **Shadow deployment** | Running a new version on copies of live traffic without showing its output to users | M05 |
| **Silent failure** | A failure where the system keeps responding normally but the answers are wrong | All |
| **SLO / SLI** | Service level objective (the target) and indicator (the measured value) | M06 |
| **Solution ladder** | Our decision framework: no automation → rules → classical ML → small model → LLM → RAG → workflow → agent → multi-agent | M01, M02 |
| **Temperature** | A sampling setting; higher values give more varied output | M01 |
| **Token** | The unit of text a model reads and writes; also the unit of most API pricing | M01 |
| **Tracing** | Recording each step of a request (retrieval, prompt, model call, tools) with timings, tokens and cost | M06 |
| **TTFT** | Time to first token: how long before a streamed response starts appearing | M05, M06 |
| **Workflow** | A predefined sequence of steps, some of which call a model. Usually preferable to an agent when steps are predictable. | M04 |
