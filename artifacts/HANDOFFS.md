# Handoff Contract

Every downstream stage consumes only approved upstream artifacts unless the founder explicitly permits an exception. Each artifact uses the common YAML envelope from its template and includes evidence, assumptions, open questions, risks, and a founder decision request.

| Stage | Input | Output Handoff | Owner Role | Founder Gate | Next Stage |
|---|---|---|---|---|---|
| 00 | `idea_brief` | `venture_intake_packet` | venture-orchestrator | G0: explore, park, kill | 01 |
| 01 | `venture_intake_packet` | `problem_validation_packet` | customer-discovery-analyst | G1: validate problem | 02 |
| 02 | `problem_validation_packet` | `market_opportunity_packet` | market-intelligence-analyst | G2: select segment/wedge | 03 |
| 03 | `market_opportunity_packet` | `demand_validation_packet` | demand-validation-designer | G3: fund business case | 04 |
| 04 | `demand_validation_packet` | `business_case_packet` | business-case-analyst | G4: approve economics/risk | 05 |
| 05 | `business_case_packet`, `demand_validation_packet` | `mvp_charter` | product-manager | G5: freeze MVP scope | 06 |
| 06 | `mvp_charter` | `functional_specification_packet` | ux-specification-designer | G6: approve UX/spec | 07 |
| 07 | `functional_specification_packet`, research outputs | `brand_go_to_market_packet` | brand-gtm-strategist | G7: approve brand/public message | 08 |
| 08 | approved product, brand, and business artifacts | `technical_design_packet` | solution-architect | G8: approve stack/security/budget | 09 |
| 09 | `technical_design_packet` | `operations_readiness_packet` | platform-operations-engineer | G9: authorize resources | 10 |
| 10 | approved functional, technical, operations artifacts | `release_candidate_packet` | mvp-implementation-engineer | G10: promote to UAT | 11 |
| 11 | `release_candidate_packet` | `production_readiness_packet` | qa-release-engineer | G11: invite beta users | 12 |
| 12 | `production_readiness_packet` | `beta_learning_packet` | product-analytics-analyst | G12: public launch, extend, pivot | 13 |
| 13 | `beta_learning_packet`, `brand_go_to_market_packet` | `launch_report_packet` | launch-growth-operator | G13: growth decision | 14 |
| 14 | `launch_report_packet` and operating data | `operating_review_packet` | support-insights-analyst | G14: scale, pivot, pause, exit | 14 |

## Common Quality Bar

An artifact is not ready for approval unless it:

1. Names the input artifact versions used.
2. Separates facts, inferences, and assumptions.
3. Includes source metadata for external claims.
4. Identifies evidence gaps and material risks.
5. Names the measurable exit criteria for the current stage.
6. Makes a single, clear founder decision request.
7. Does not claim external actions, customer commitments, legal clearance, deployment, or tests that did not occur.

## Common Founder Decision Format

```yaml
founder_decision:
  outcome: pending # go | revise | pivot | pause | park | kill | scale | optimize | exit
  decided_by: ""
  decided_at: ""
  rationale: ""
  constraints_or_feedback: ""
```
