---
name: mvp-technical-design
description: Use when designing an MVP architecture, database schema, data model, APIs, authentication, roles, permissions, security controls, environments, observability, backups, and cloud cost estimates.
---

# MVP Technical Design

## Objective

Design the simplest secure, observable, low-operations architecture that meets the approved MVP charter and functional specification.

## Default Architecture Principle

Start managed and modular, not distributed:

- One web application where possible.
- Managed authentication, database, and storage.
- Managed payments, email, analytics, error tracking, and hosting.
- Few integrations.
- No microservices unless the MVP has a demonstrated need.

## Required Decisions

Document:

- System boundaries and architecture diagram.
- Local, preview, and production environment responsibilities.
- Data classification and minimization.
- Database entities, keys, relationships, constraints, and retention.
- Authentication, sessions, roles, authorization, and tenant isolation.
- APIs, webhooks, integrations, and idempotency.
- Storage access control.
- Secrets, key rotation, vendor access, and MFA.
- Error handling, monitoring, logs, alerts, audit trails, and analytics.
- Rate limiting, abuse prevention, and AI spend controls where relevant.
- Backup, restore, incident response, rollback, and dependency failure plan.
- Fixed and variable cost estimates.

## Threat Model

For each material threat include:

- Asset at risk.
- Actor and capability.
- Attack or failure path.
- Likelihood and impact.
- Preventive and detective control.
- Verification method.
- Residual risk and owner.

## Security Baseline

- Least privilege and server-side authorization.
- Never trust client-provided role or tenant identifiers.
- Secrets never in source control or client bundles.
- Validate input and fail safely.
- Encrypt in transit; use vendor-managed encryption at rest where suitable.
- Redact sensitive data from logs and traces.
- Define deletion, export, and retention behavior before collecting data.

## Output

Create `technical_design_packet`; do not provision resources or claim compliance/certification.
