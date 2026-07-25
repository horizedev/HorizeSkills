---
name: agentic-awesome-skills
description: Use when working in the continuous idea-to-MVP workflow to select, activate, or apply the mapped Agentic Awesome Skills playbooks for founder framing, research, product definition, delivery, verification, or learning.
---

# Agentic Awesome Skills Integration

## Purpose

This repository uses its local skills as venture-specific adapters and Agentic Awesome Skills (AAS) as the reusable domain-playbook layer. The selected AAS stack is pinned in `aas-stack.json`; the role and workstream map lives in `workflow/aas-skill-map.yaml`.

## Procedure

1. Read `AGENTS.md`, `workflow/pipeline.yaml`, the current venture workbook, and the local skill that matches the task.
2. Read `workflow/aas-skill-map.yaml` to identify the task's workstream and exact AAS skill IDs.
3. When AAS Core or a materialized Codex stack is available, inspect and apply the mapped AAS playbooks. Use the full AAS catalog to find an additional relevant skill when the map has a genuine gap.
4. Keep AAS methods subordinate to founder intent, venture evidence, this repository's external-action boundary, and the current MVP scope.
5. Record the AAS skills used or the catalog gap in the workbook's work log when the work materially changes direction, scope, or delivery.

## Availability and Trust

- `aas-stack.json` is a pinned desired-state manifest, not proof that a skill is installed or executed.
- Use AAS Core's read-only catalog and manifest validation workflow before materializing skills. Do not silently install, update, or apply third-party skill content.
- The mapped catalog is `agentic-awesome-skills` v15.4.0. The repository and selected skill IDs are sourced from `https://github.com/sickn33/agentic-awesome-skills` and recorded in `workflow/aas-skill-map.yaml`.
- AAS skill content can contain upstream-specific directions. Apply it only when compatible with the venture, verified facts, authorization limits, and the current task.

## Coverage Rule

Use at least one mapped AAS playbook for every substantive workstream task when the stack is available. Do not use a generic method when a mapped specialist playbook covers the problem. Do not force irrelevant AAS skills into a task merely because they are in the manifest.
