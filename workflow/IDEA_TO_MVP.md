# Continuous Idea-to-MVP Framework

## Purpose

Turn any useful founder input into a coherent, testable MVP without forcing the founder to express an idea in a particular order. A founder may begin with a customer problem, a product image, a feature list, a visual direction, a business model, a personal observation, a technical possibility, or a mixture of all of them.

The workflow preserves that input, makes its meaning explicit, fills gaps with researched and clearly labeled reasoning, and keeps the emerging MVP close to the founder's intended outcome.

## One Living Artifact

Each venture has one current artifact:

```text
ventures/<venture-slug>/artifacts/idea-to-mvp-workbook.md
```

It is the shared context for research, product definition, delivery, and verification. Contributors update relevant sections, retain a short direction log, and link supporting material in `evidence/`. It replaces serial handoff packets and approved-predecessor rules.

## AAS Integration

`aas-stack.json` pins the exact Agentic Awesome Skills catalog version and selected skill IDs for this workflow. `workflow/aas-skill-map.yaml` maps every role and local venture skill to those IDs. The manifest is validated desired state, not proof that a third-party skill is already materialized or has been used.

Use the AAS Core read-only catalog and validation flow before materializing skills. When an AAS stack is available, each substantive workstream task uses the mapped relevant playbook and records it in the workbook Work Log. When the map has a real gap, search the full catalog, select a non-redundant suitable skill, and record the selection or catalog gap.

## Workstreams

### Founder Intent and Venture Framing

Capture everything the founder knows or imagines. Classify each entry so it remains useful without being mistaken for evidence:

- `commitment`: a non-negotiable outcome, audience, constraint, or product principle.
- `preference`: a desired feature, interaction, visual reference, business model, or implementation preference that may be traded off.
- `hypothesis`: a belief about customers, value, demand, market, or delivery that needs evidence.
- `inspiration`: a starting point or reference that can inform creative exploration.
- `open_question`: an important unknown that needs a decision or test.

Produce a product thesis, alternative interpretations where needed, an assumption map, and an explicit list of founder-intent tensions. Never quietly replace a founder preference with generic product advice.

### Integrated Opportunity Research

Run customer discovery, desk research, competitive analysis, demand-test design, pricing analysis, business viability, and issue spotting as one connected evidence loop. Research can refine the original direction, but it cannot erase it without recording why.

Use the smallest credible test for the highest-risk assumption. Draft outreach and experiments freely; execute external activity only after authorization. Keep real results, contradictory evidence, source limitations, and negative findings.

### Product, Experience, and Market Definition

Turn intent and evidence into an MVP that has one clear core outcome, a bounded primary journey, explicit non-goals, a testable experience, an initial product narrative, and measurable success signals. Product design, brand direction, UX, features, analytics, and scope are designed together rather than passed through serial stages.

Creative synthesis is expected here. New ideas are welcome when they make the MVP more coherent or valuable, but they must be marked as an inference or assumption and traced back to founder intent, evidence, or a stated design principle.

### Integrated MVP Delivery

Architecture, security, privacy, operations, implementation, code review, and quality verification run as one delivery loop. Technical discoveries can revise scope; scope revisions can revise delivery design. Use actual test output, not agent assertions.

The core endpoint is a reviewable, tested MVP package with known issues, risk treatment, and a clear path to an authorized controlled release. A beta, public launch, and ongoing growth are optional post-MVP activities.

## Working Rhythm

1. Read the idea brief, current workbook, evidence, decisions, and relevant app materials.
2. Choose the highest-leverage unresolved question or the next in-scope delivery slice.
3. Use the mapped specialist role and AAS playbooks from `workflow/aas-skill-map.yaml`.
4. Update the workbook and evidence links. Preserve prior intent and explain material changes in the direction log.
5. Feed discoveries back into affected workstreams immediately; do not wait for a stage boundary.
6. Record an optional decision when a material direction, scope, or risk changes.
7. Request authorization only if an action would contact people, spend money, publish, provision paid or production infrastructure, handle sensitive data, or otherwise create an external side effect.

## Evidence Standard

- Label all substantive statements as `fact`, `inference`, or `assumption`.
- For external facts, record source URL, retrieval date, relevant evidence, and confidence.
- Do not invent interviews, user behavior, customer commitments, market figures, test results, legal conclusions, or security claims.
- State geography, sample size, date range, and limitations for market or customer claims when applicable.
- Absence of evidence is not evidence of absence.

## External Authorization Boundary

Internal work is continuous. The following still need explicit founder authorization because they create external effects: outreach, interviews, surveys, publishing, paid spend, domains, cloud resources, credentials, production changes, deployment, data collection, or public legal/security/performance claims.

Use `ventures/<venture-slug>/decisions/authorization-and-decision-record-template.md` when a durable record is useful. An authorization applies only to the action and scope recorded; it is not an approval gate for subsequent internal work.

## MVP Completion Package

The MVP package is complete when the workbook can point to:

- A preserved founder-intent record and coherent product thesis.
- An evidence-backed or transparently assumption-led target user, problem, outcome, wedge, and business boundary.
- A focused MVP scope, primary journey, experience specification, product narrative, and measurement plan.
- A minimal delivery design with data, authorization, privacy, security, operational, and cost considerations.
- Traceable implementation and actual verification evidence.
- Known issues, residual risks, evidence gaps, and any external actions that remain unauthorized.

This is a completion check, not a gate. Work may continue on any unresolved item according to risk and founder priorities.
