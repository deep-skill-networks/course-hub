# API keys and costs

Every lab states its expected cost up front. Our target is **under ₹100 (about $1) per lab** on paid APIs, and **₹0** if you use the local-model path.

## Rules
1. **Never commit a key.** Each repo has a `.env.example`; copy it to `.env`, which is git-ignored. Every lab's grading workflow scans for leaked secrets, and push protection is turned on in course repositories.
2. **Set a hard spending limit** in every provider console before you create a key. Set an email alert at 50% of it.
3. **Use a separate key for the course**, so you can revoke it without affecting other work.
4. **Prefer the local path** for exploration. Switch to a paid model only when a lab says the comparison matters.

## Choosing a model in a lab
Each lab has one configuration file, `config/models.yaml`, where you choose the provider and model. It always lists a local fallback. You never edit code to switch models.

## Cloud spending
- Use free tiers or credits, and create a **budget alert** on day one.
- Every lab that creates cloud resources includes a `make destroy` (or `terraform destroy`) step. Run it when you finish.
- GPU sessions are short and capped. Never leave a GPU instance running overnight.

## If you leak a key
Revoke it in the provider console immediately, then create a new one. Rewriting git history doesn't help once a key has been pushed, because it may already have been copied.

Prices and free tiers change often, so this page deliberately doesn't list them. Check each provider's pricing page when you set up.
