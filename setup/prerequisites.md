# Prerequisites

## Skills you should already have
- Comfortable writing Python (functions, classes, virtual environments, packages).
- Everyday Git: branches, pull requests, resolving simple conflicts.
- You have deployed a web service or API before, in any language.
- Basic command line and HTTP/REST.

You do **not** need prior ML, Docker, Kubernetes or Terraform experience. The pre-work modules (P1, P2) cover them, and each ends with a self-check so you know you're ready.

## Accounts
| Account | Why | Notes |
|---|---|---|
| GitHub | All course code, labs and autograding | You'll be added to your cohort's team in the `deep-skill-networks` org. Send us your GitHub username. |
| One cloud provider | Deploying your capstone | The cloud is announced per cohort. Use a free tier or credits, and set a billing alert on day one. |
| At least one LLM API provider | Labs that need a frontier model | Optional for many labs, thanks to local models. See [API keys and costs](api-keys-and-costs.md). |

## Machine
- **Recommended:** 16 GB RAM, a recent multi-core CPU, 30 GB free disk. This runs small open models locally (roughly 3–8B parameters, quantised).
- **Lower-spec machine?** Every lab ships with a dev container that runs in GitHub Codespaces or locally in VS Code. Codespaces includes a monthly free usage quota for personal accounts; check GitHub's current limits.
- A GPU is **not** required. Labs that need one use a short, capped cloud session.

## Tools to install
| Tool | Purpose |
|---|---|
| Git | Version control |
| VS Code (or another editor with dev container support) | Opening labs in a ready-made environment |
| Docker Desktop, Podman, or Rancher Desktop | Running containers and dev containers locally |
| Python 3.11+ and `uv` (or `pip`) | Running labs outside the container |
| Ollama (or another local model runner) | Free local-model path for labs |
| Terraform or OpenTofu, `kubectl` | Introduced in P1; installed inside the dev container too |

The dev container in each lab repository includes everything a lab needs, so local installs are a convenience, not a requirement.

## Before week 1 checklist
- [ ] GitHub username sent; invitation to the cohort team accepted
- [ ] A lab repository opens in a dev container (locally or in Codespaces)
- [ ] A local model answers a prompt via Ollama, **or** an API key is set up with a spending limit
- [ ] Cloud account created with a billing alert
- [ ] P1 and P2 self-checks passed
