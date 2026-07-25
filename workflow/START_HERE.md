# Run a Venture With Codex

## 1. Create a Venture Workspace

```sh
cp -R ventures/_template ventures/<venture-slug>
```

Complete the initial idea brief with everything that may matter: observations, problems, product ideas, feature ideas, visual direction, business ideas, constraints, references, and doubts. A polished problem statement is not required.

## 2. Create the Living Workbook

```sh
cp artifacts/templates/idea-to-mvp-workbook.md \
  ventures/<venture-slug>/artifacts/idea-to-mvp-workbook.md
```

The workbook is the current source of truth. It is updated continuously rather than handed from stage to stage.

## 3. Start With Founder Intent

Use the following prompt pattern in Codex:

```text
Act as venture-orchestrator for venture <venture-slug>.
Read AGENTS.md, workflow/pipeline.yaml, workflow/IDEA_TO_MVP.md, aas-stack.json,
workflow/aas-skill-map.yaml, the idea brief, current workbook, evidence, decisions, and relevant
app materials. Preserve every founder contribution as a commitment, preference, hypothesis,
inspiration, or open question. Update the workbook with a product thesis, assumption map,
evidence gaps, and next work. Do not take an external action without explicit founder authorization.
```

## 4. Work Continuously

Use the workstream that resolves the highest-risk uncertainty or next delivery need:

- `founder-intent`: venture framing and preservation of founder direction.
- `opportunity-research`: customer, market, demand, pricing, business viability, and risk evidence.
- `mvp-definition`: scope, UX flows, product narrative, and measurement plan.
- `delivery-loop`: architecture, operations, implementation, code review, testing, and verification.
- `mvp-learning`: optional authorized beta, launch, support, and growth work.

Each role reads the workbook, applies its local skill and mapped AAS playbooks, then updates the relevant sections, Direction Log, and Work Log. Research and delivery can run in parallel and can revise prior work when evidence changes.

## 5. Review Quality

After meaningful work, check:

- Is founder intent preserved, classified, and still visible?
- Is every key claim sourced or labeled as an inference or assumption?
- Are customer evidence and research findings real rather than invented?
- Does the MVP remain focused on one core outcome and primary journey?
- Do scope, design, technical, and risk changes have a rationale in the Direction Log?
- Are actual test results distinct from planned or unexecuted checks?

## 6. External Authorization

Internal work is ungated. Explicit founder authorization is still required before actions that affect the outside world:

- Customer outreach, interviews, surveys, messages, or calls.
- Publishing, ads, testimonials, pricing, legal pages, or public claims.
- Purchases, paid services, domains, cloud resources, or paid APIs.
- Production credentials, DNS, payment settings, production infrastructure, deployment, or production data.
- Personal or sensitive data collection and handling.

Record a durable authorization or material decision with `decisions/authorization-and-decision-record-template.md` when useful.

## Role Prompts

| Workstream           | Roles                                                                                                              | Workbook Focus                            |
| -------------------- | ------------------------------------------------------------------------------------------------------------------ | ----------------------------------------- |
| Founder intent       | `venture-orchestrator`                                                                                             | Intent, frame, assumptions, direction log |
| Opportunity research | `customer-discovery-analyst`, `market-intelligence-analyst`, `demand-validation-designer`, `business-case-analyst` | Evidence, alternatives, viability, risks  |
| MVP definition       | `product-manager`, `ux-specification-designer`, `brand-gtm-strategist`                                             | Scope, flows, narrative, measurement      |
| Delivery loop        | `solution-architect`, `platform-operations-engineer`, `mvp-implementation-engineer`, `qa-release-engineer`         | Architecture, build, tests, verification  |
| Reviews              | `research-evidence-auditor`, `code-quality-reviewer`, `security-risk-reviewer`, `legal-privacy-risk-spotter`       | Independent evidence and risk checks      |
| Optional learning    | `product-analytics-analyst`, `launch-growth-operator`, `support-insights-analyst`                                  | Authorized learning, launch, support      |

## Visual Guide

Open `mvp-workflow.html` locally. It illustrates how founder input flows through connected workstreams, how AAS skills support each role, and where explicit external authorization remains necessary.
