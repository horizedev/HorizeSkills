---
name: product-pipeline-governance
description: Use when starting, routing, reviewing, approving, revising, pausing, or closing a venture in the end-to-end product pipeline.
---

# Product Pipeline Governance

## Purpose

Run an evidence-led venture as a gated state machine. Agents generate bounded work products. The founder decides when capital, reputation, customer access, legal exposure, or production risk is incurred.

## Required Reading

Before any stage work, read:

1. `AGENTS.md`
2. `workflow/pipeline.yaml`
3. `artifacts/HANDOFFS.md`
4. Current venture's `00-input/idea-brief.md`
5. All approved upstream artifacts and current decision records

## Stage Procedure

1. Identify the current stage from the last founder decision.
2. Verify approved inputs match the stage's `inputs` list.
3. Select the stage's agent role and skill.
4. Copy the matching template into `ventures/<slug>/artifacts/<stage>-<artifact>.md`.
5. Produce a draft only. Preserve all frontmatter fields.
6. Validate sources, assumptions, risks, and acceptance criteria.
7. Request a single founder decision and list valid routes from `pipeline.yaml`.
8. Do not start the next stage until the founder records an approved `go` decision.

## Artifact Rules

Every artifact must include:

- Artifact metadata and status.
- Exact upstream artifact versions.
- Evidence sources and limitations.
- Facts, inferences, and assumptions separated.
- Risks, unresolved questions, and exit criteria.
- Founder decision request with allowed outcomes.
- Next-stage handoff summary.

## Gate Rules

The following gates always require human approval:

- G0: choose to explore.
- G1: problem is worth further validation.
- G2: customer segment and wedge are worth testing.
- G3: spend time and money on a business case.
- G4: approve economics, risk posture, and MVP investment.
- G5: freeze MVP scope.
- G6: approve functional specification and UX direction.
- G7: approve name, messaging, pricing, and public-facing assets.
- G8: approve architecture, vendors, security baseline, and cost.
- G9: authorize accounts, credentials, domains, and environment setup.
- G10: promote a release candidate to production UAT.
- G11: invite private-beta users.
- G12: conduct public launch.
- G13/G14: scale, pivot, pause, kill, or begin exit work.

## Stop Conditions

Route to `pause` or `kill` rather than forcing progress if:

- No repeated painful problem is evidenced.
- Customers will not commit money, time, data, or behavior change.
- The reachable market cannot support the founder's goals.
- Regulatory, security, or operational risks exceed capacity.
- The MVP cannot be safely built within the approved budget and timeframe.

## Review Checklist

- Does the artifact answer the stage question rather than describe a generic business?
- Is each strong conclusion proportional to evidence?
- Are negative findings included?
- Are decision criteria measurable?
- Does it distinguish what happened from what should happen next?
