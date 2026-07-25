---
name: secure-mvp-delivery
description: Use when setting up MVP environments, credentials, runbooks, CI/CD, implementation, code review, testing, production UAT, release candidates, and deployment readiness.
---

# Secure MVP Delivery

## Objective

Turn the current product and technical definition into a testable, operable MVP without bypassing security, quality, or external-action authorization.

## AAS Methods

When the configured AAS stack is available, apply `saas-mvp-launcher`, `full-stack-orchestration-full-stack-feature`, `testing-qa`, `e2e-testing`, `cloud-devops`, `production-code-audit`, and the accessibility or security review skills that fit the work. Read `workflow/aas-skill-map.yaml` and record the AAS methods used or any catalog gap in the workbook Work Log.

## Environment Baseline

Maintain:

- Local development.
- Preview/staging for review and testing.
- Production for real users only.

For each, document ownership, access, secrets, data policy, deployment path, monitoring, and recovery.

## Implementation Rules

- Map each code change to a current user story and acceptance criterion.
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

The agent may create a release candidate and test it in local or authorized non-production environments. Production deployment, beta invitations, DNS changes, billing activation, and public launch always require explicit founder authorization.

## Output

Update the workbook's Delivery Design, Build Traceability, Verification Evidence, Risk Register, External Authorization Log, Direction Log, and Work Log. Report blockers plainly; never substitute an LLM assertion for a test result.
