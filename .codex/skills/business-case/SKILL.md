---
name: business-case
description: Use when designing pricing, subscriptions, unit economics, revenue forecasts, MVP budgets, risk registers, legal issue spotting, privacy reviews, and business viability decisions.
---

# Business Case

## Objective

Determine whether validated demand can support a sustainable, appropriately risk-managed business.

## Pricing Approach

Start simply. Price against value created or cost avoided, while respecting customer budget and purchasing behavior.

For each proposed plan state:

- Target customer.
- Core value unlocked.
- Usage, seat, or feature boundary.
- Price, billing period, and trial policy.
- Reason the price is plausible.
- Evidence and uncertainty.

## Economics Model

Show formulas and assumptions:

```text
MRR = paying accounts x average monthly revenue per account
Gross profit = MRR - direct delivery costs
Gross margin = gross profit / MRR
LTV estimate = monthly gross profit per customer / monthly churn rate
```

Include model/API use, hosting, database, email, payment fees, support time, refunds, acquisition, and founder time where relevant. Provide low/base/high cases rather than one exact projection.

## Risk Review

Create a risk register for:

- Market and distribution.
- Concentration and founder dependency.
- Data and privacy.
- Security and abuse.
- Payments, chargebacks, refunds, and taxation.
- AI model cost, quality, availability, and data use.
- Regulatory or sector constraints.
- Vendor lock-in and service outage.

Legal, tax, privacy, and regulatory points are issue spotting only. Identify when professional advice is necessary.

## Output

Create `business_case_packet` with business model, pricing, revenue scenarios, unit economics, cost model, risk register, legal/privacy issue list, operating assumptions, investment limit, and go/no-go rationale.
