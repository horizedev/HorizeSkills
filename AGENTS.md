# Idea-to-MVP Operating Instructions

This repository is a continuous, evidence-led operating system for turning founder intent into a testable MVP. Treat `workflow/pipeline.yaml`, `workflow/IDEA_TO_MVP.md`, and the current venture's `artifacts/idea-to-mvp-workbook.md` as the source of truth.

## Operating Rules

1. Identify the venture directory and read its `input/idea-brief.md`, current workbook, evidence, decisions, and relevant app materials before working.
2. Treat every founder contribution as meaningful input. Preserve product ideas, feature ideas, visual or interaction preferences, business ideas, constraints, and personal observations; classify each as a commitment, preference, hypothesis, inspiration, or open question rather than discarding it because it is incomplete.
3. Use the matching role and workstream in `workflow/pipeline.yaml`. Read `aas-stack.json` and `workflow/aas-skill-map.yaml`, then apply the mapped Agentic Awesome Skills playbooks when they are available.
4. Work continuously across connected workstreams. Internal research, synthesis, specification, design, implementation, review, and revision do not require an approved predecessor or a stage transition.
5. Update the relevant sections of `artifacts/idea-to-mvp-workbook.md` from `artifacts/templates/idea-to-mvp-workbook.md`. Keep history and rationale instead of replacing earlier founder intent or evidence without explanation.
6. Preserve YAML frontmatter and complete applicable sections. Do not replace unknowns with invented facts.
7. Mark claims as `fact`, `inference`, or `assumption`. Every external factual claim requires a source URL, retrieval date, evidence, and confidence.
8. Use creativity to connect well-supported founder intent into a coherent product direction, but label every new leap as an inference or assumption and state how it could be tested.
9. End every task with: `workbook updated`, `evidence gaps`, `risks`, `next work`, `external authorization needed`, and `next agent role`.

## External-Action Authorization Policy

The following always require explicit founder authorization in the current task or an authorization record. These are real-world safety boundaries, not internal workflow gates:

- Customer outreach, interviews, surveys, emails, direct messages, or calls
- Publishing content, social posts, ads, testimonials, pricing, or legal pages
- Purchases, paid subscriptions, domains, cloud resources, or API usage that incurs cost
- Creating or changing production credentials, DNS, payment settings, or infrastructure
- Deploying to production, changing database schema in production, or accessing production data
- Sending messages, collecting personal data, or handling sensitive customer information
- Claiming compliance, legal validity, security certification, or performance results

Drafts, plans, prototypes, and local non-production work are allowed. External side effects are not.

## Artifact Statuses

- `draft`: incomplete or exploratory work.
- `active`: current working artifact; it may be used by any internal workstream.
- `blocked`: work cannot continue without evidence, access, a decision, or an external authorization.
- `superseded`: retained for history but replaced by a newer current version.
- `archived`: no longer active.

## Venture Directory Layout

```text
ventures/<venture-slug>/
  input/idea-brief.md
  artifacts/idea-to-mvp-workbook.md
  evidence/
  decisions/
  app/                 # Product source repository when implementation begins
```

## Research Integrity

- Do not create fictional interviews, quotes, customer commitments, pricing observations, test outcomes, or legal conclusions.
- Distinguish absence of evidence from evidence of absence.
- State sample size, geography, date range, and source limitations for market claims.
- Escalate regulated areas, privacy questions, contracts, tax, employment, medical, financial, children's, or jurisdiction-specific issues to a qualified professional.

## Delivery Discipline

- Prefer the smallest test or implementation that resolves the highest-risk assumption.
- Keep scope inside the current MVP definition. Log requested scope changes, their rationale, and their effect on founder intent before implementing them.
- Use deterministic tools and tests for validation. LLM judgment does not replace a test result, security review, or an external-action authorization.
- Do not commit secrets, customer data, access tokens, or production exports.
