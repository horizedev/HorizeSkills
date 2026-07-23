---
venture_id: ""
artifact_id: ""
artifact_type: business_case_packet
version: 1
status: draft
stage: "04"
created_at: ""
created_by: business-case-analyst
input_artifacts:
  - demand_validation_packet: ""
sources: []
---

# Business Case Packet

## Decision Question

Does the validated opportunity justify the approved MVP investment given economics, risk, founder capacity, and operating constraints?

## Business Model

- Customer type: B2B / B2C / prosumer / marketplace / other
- Buyer:
- Revenue model:
- Billing frequency:
- Why this model fits observed behavior:

## Pricing Hypotheses

| Plan | Target Customer | Core Value / Limit | Monthly Price | Annual Price | Evidence | Uncertainty |
|---|---|---|---:|---:|---|---|
|  |  |  |  |  |  |  |

## Revenue and Unit Economics

### Formula Inputs

| Input | Low | Base | High | Source / Assumption |
|---|---:|---:|---:|---|
| Reachable accounts |  |  |  |  |
| Paid conversion |  |  |  |  |
| ARPA |  |  |  |  |
| Monthly churn |  |  |  |  |
| Direct delivery cost / account |  |  |  |  |
| Acquisition cost |  |  |  |  |

### Scenario Outputs

| Scenario | Paying Accounts | MRR | Gross Margin | Estimated CAC Payback | Key Assumption |
|---|---:|---:|---:|---:|---|
| Low |  |  |  |  |  |
| Base |  |  |  |  |  |
| High |  |  |  |  |  |

## MVP Investment and Operating Budget

- Maximum MVP build time:
- Maximum MVP build cost:
- Expected monthly fixed cost:
- Expected monthly variable cost / active account:
- Required runway:
- Cost-stop threshold:

## Legal, Privacy, and Compliance Issue Spotting

| Issue | Triggering Fact | Potential Impact | Urgency | Missing Information | Professional Needed |
|---|---|---|---|---|---|
|  |  |  |  |  |  |

This is issue spotting, not legal, tax, accounting, or regulatory advice.

## Risk Register

| Risk | Likelihood | Impact | Mitigation | Owner | Residual Risk |
|---|---|---|---|---|---|
|  |  |  |  |  |  |

## Investment Recommendation

- Recommendation:
- Conditions required before MVP work:
- What would invalidate the business case:

## Facts, Inferences, and Assumptions

### Facts

### Inferences

### Assumptions

## Stage Exit Criteria

- [ ] Pricing and economic assumptions are transparent.
- [ ] Cost and capacity limits are explicit.
- [ ] Material privacy/legal/security issues are identified for professional review.
- [ ] A bounded MVP investment decision is possible.

## Founder Decision

```yaml
founder_decision:
  outcome: pending # go | revise | pivot | pause | kill
  decided_by: ""
  decided_at: ""
  rationale: ""
  constraints_or_feedback: ""
```

## Approved Handoff to Stage 05

- Next role: `product-manager`
- Next skill: `mvp-product-spec`
- Required inputs: approved `business_case_packet` and `demand_validation_packet`
- Requested work: define the smallest secure MVP that proves the next business-critical hypothesis.
