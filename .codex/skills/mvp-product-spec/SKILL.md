---
name: mvp-product-spec
description: Use when defining MVP scope, product strategy, user journeys, UX flows, functional specifications, user stories, acceptance criteria, authentication, roles, analytics, and accessibility requirements.
---

# MVP Product Specification

## Objective

Specify the smallest secure product that can prove the next business-critical hypothesis and create repeatable user value.

## Scope Filter

For each proposed feature ask:

1. Does it enable the core job and measurable outcome?
2. Does it test a critical assumption?
3. Is it required for security, trust, payment, or legal operation?
4. Can it be performed manually during beta?
5. Can the first ideal customer succeed without it?

Defer it unless the answer is compelling.

## MVP Charter

Define:

- Target user and buyer.
- Core job-to-be-done.
- Primary outcome.
- MVP hypothesis.
- Primary journey.
- Activation event.
- North-star metric and supporting metrics.
- Must-have capabilities.
- Security/trust baseline.
- Explicit non-goals.
- Manual operations.
- Launch criteria and budget/time boundary.

## Functional Specification

For each flow document:

- Trigger and preconditions.
- User steps and system response.
- Inputs, validation, outputs, and persistence.
- Authentication, role, and permission requirements.
- Happy path and unhappy path.
- Loading, empty, error, retry, cancellation, and recovery states.
- Analytics events with exact event names and properties.
- Accessibility and responsive behavior.
- Testable acceptance criteria.

## UX Rules

- Prioritize one clear primary action per screen.
- Use understandable language from customer discovery.
- Minimize setup before first value.
- Use sensible defaults and progressive disclosure.
- Preserve work on errors.
- Do not confuse visual novelty with product differentiation.

## Output

Create an `mvp_charter` or `functional_specification_packet` as the stage requires. Do not move unapproved product ideas into build scope.
