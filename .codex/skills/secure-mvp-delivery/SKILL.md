---
name: secure-mvp-delivery
description: Use when setting up MVP environments, credentials, runbooks, CI/CD, implementation, code review, testing, production UAT, release candidates, and deployment readiness.
---

# Secure MVP Delivery

## Objective

Turn approved product and technical designs into a testable, operable release candidate without bypassing security, quality, or founder approvals.

## Environment Baseline

Maintain:

- Local development.
- Preview/staging for review and testing.
- Production for real users only.

For each, document ownership, access, secrets, data policy, deployment path, monitoring, and recovery.

## Implementation Rules

- Map each code change to an approved user story and acceptance criterion.
- Use small changes and reviewable commits/PRs.
- Treat migrations as reversible or explicitly guarded.
- Enforce authorization on the server and database layer.
- Validate inputs at trust boundaries.
- Keep secrets out of source, browser bundles, logs, fixtures, and screenshots.
- Use feature flags or guarded rollout for meaningful risk.
- Record actual test commands and outputs.

## Required Verification

- Signup, login, logout, reset/recovery.
- Authorization and tenant/data isolation.
- Core happy path and important unhappy paths.
- Payment, cancellation, and webhook behavior when applicable.
- Email delivery and notification failures.
- Analytics events and error tracking.
- Dependency/API failure behavior.
- Backup/restore procedure where customer data exists.
- Responsive and basic accessibility checks.
- Monitoring, alert, rollback, and support readiness.

## Release Discipline

The agent may create a release candidate and test it in approved non-production environments. Production deployment, beta invitations, DNS changes, billing activation, and public launch always require founder approval.

## Output

Create `operations_readiness_packet`, `release_candidate_packet`, or `production_readiness_packet` according to the stage. Report blockers plainly; never substitute an LLM assertion for a test result.
