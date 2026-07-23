# Run a Venture With Codex

## 1. Create a Venture Workspace

```sh
cp -R ventures/_template ventures/<venture-slug>
```

Complete the initial idea brief. Use a short, concrete problem from direct experience rather than a solution description.

## 2. Start at the Current Stage

Use the following prompt pattern in Codex:

```text
Act as <agent-role>. Run <stage-id> for venture <venture-slug>.
Read AGENTS.md, workflow/pipeline.yaml, artifacts/HANDOFFS.md, all approved input artifacts,
and the matching skill. Create the matching output artifact as a draft in the venture artifacts
directory. Follow its template exactly. Do not take external action or cross the human gate.
```

## 3. Review the Handoff

For each draft, check:

- Are all mandatory sections present?
- Is every key claim cited or labeled as an assumption?
- Are customer evidence and research findings real rather than inferred?
- Does the output meet the stage's exit criteria?
- Is the recommended decision supported by evidence?

Record a decision in the artifact's `founder_decision` section. Change `status` to `approved` only after you approve it.

## 4. Route Deliberately

At every gate choose one outcome:

- `go`: approve artifact and start the next listed stage.
- `revise`: return to the current agent with precise feedback.
- `pivot`: return to the named earlier stage with a changed segment, problem, wedge, or model.
- `pause`: keep the venture open but do not run downstream agents.
- `kill`: archive the venture and document learning.

## 5. Build the MVP

After Stage 9 is approved:

1. Create or attach a separate application repository at `ventures/<venture-slug>/app/`.
2. Give the `mvp-implementation-engineer` the approved functional specification, technical design, and operations readiness packet.
3. Require pull requests, tests, a release candidate packet, and a founder approval before production UAT.
4. Treat Stage 11 production UAT as the final readiness check before inviting beta users.

## Stage Prompt Shortcuts

| Stage | Role | Ask For |
|---|---|---|
| 00 | `venture-orchestrator` | `venture_intake_packet` |
| 01 | `customer-discovery-analyst` | `problem_validation_packet` |
| 02 | `market-intelligence-analyst` | `market_opportunity_packet` |
| 03 | `demand-validation-designer` | `demand_validation_packet` |
| 04 | `business-case-analyst` | `business_case_packet` |
| 05 | `product-manager` | `mvp_charter` |
| 06 | `ux-specification-designer` | `functional_specification_packet` |
| 07 | `brand-gtm-strategist` | `brand_go_to_market_packet` |
| 08 | `solution-architect` | `technical_design_packet` |
| 09 | `platform-operations-engineer` | `operations_readiness_packet` |
| 10 | `mvp-implementation-engineer` | `release_candidate_packet` |
| 11 | `qa-release-engineer` | `production_readiness_packet` |
| 12 | `product-analytics-analyst` | `beta_learning_packet` |
| 13 | `launch-growth-operator` | `launch_report_packet` |
| 14 | `support-insights-analyst` | `operating_review_packet` |

## Visual Guide

Open `mvp-workflow.html` locally. It illustrates each step, the active agent and skill, the produced handoff, the founder gate, and allowed routes.
