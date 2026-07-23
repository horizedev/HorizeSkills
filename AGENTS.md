# Product Pipeline Instructions

This repository is a human-gated venture operating system. Treat `workflow/pipeline.yaml` and `artifacts/HANDOFFS.md` as the source of truth for stage order and handoff requirements.

## Operating Rules

1. Identify the current venture directory and current stage before doing work.
2. Read every approved upstream artifact listed in the stage's `inputs` before generating output.
3. Use the matching agent role and skill named in `workflow/pipeline.yaml`.
4. Create one draft output artifact from the corresponding file in `artifacts/templates/`.
5. Preserve the YAML frontmatter and complete every required section. Do not replace unknowns with invented facts.
6. Mark claims as `fact`, `inference`, or `assumption`. Every external factual claim requires a source URL, retrieval date, evidence, and confidence.
7. End every task with: `artifact produced`, `evidence gaps`, `risks`, `founder decision needed`, and `next agent role`.
8. Never silently advance a stage. Only the founder can record `go`, `revise`, `pivot`, `pause`, or `kill` at a gate.

## Approval and External-Action Policy

The following always require explicit founder approval in the current artifact or task:

- Customer outreach, interviews, surveys, emails, direct messages, or calls
- Publishing content, social posts, ads, testimonials, pricing, or legal pages
- Purchases, paid subscriptions, domains, cloud resources, or API usage that incurs cost
- Creating or changing production credentials, DNS, payment settings, or infrastructure
- Deploying to production, changing database schema in production, or accessing production data
- Sending messages, collecting personal data, or handling sensitive customer information
- Claiming compliance, legal validity, security certification, or performance results

Drafts are allowed. External side effects are not.

## Artifact Statuses

- `draft`: generated or revised by an agent; never a valid input to a downstream gated stage unless the founder explicitly allows it.
- `reviewed`: reviewed but awaiting a decision.
- `approved`: founder approved; valid upstream input.
- `rejected`: not usable; do not route downstream.
- `superseded`: retained for audit history but replaced by a newer approved version.

## Venture Directory Layout

```text
ventures/<venture-slug>/
  00-input/idea-brief.md
  artifacts/
  evidence/
  decisions/
  app/                 # Separate product source repository after Stage 10 approval
```

## Research Integrity

- Do not create fictional interviews, quotes, customer commitments, pricing observations, test outcomes, or legal conclusions.
- Distinguish absence of evidence from evidence of absence.
- State sample size, geography, date range, and source limitations for market claims.
- Escalate regulated areas, privacy questions, contracts, tax, employment, medical, financial, children's, or jurisdiction-specific issues to a qualified professional.

## Delivery Discipline

- Prefer the smallest test or implementation that resolves the highest-risk assumption.
- Keep scope inside the approved MVP charter. Log requested scope changes instead of implementing them.
- Use deterministic tools and tests for validation. LLM judgment does not replace a test result, security review, or founder approval.
- Do not commit secrets, customer data, access tokens, or production exports.
