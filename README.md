# Continuous Idea-to-MVP

A Codex-ready, founder-directed operating system for turning any raw product direction into a coherent, testable MVP.

Start with whatever the founder has: a problem, product concept, feature ideas, visual direction, workflow, business model, customer observation, technical insight, or constraint. The framework preserves those inputs, identifies their confidence, fills gaps through research and creative synthesis, and continuously aligns product definition, design, delivery, and verification around the intended MVP.

## What Is Included

- `AGENTS.md`: repository-wide operating rules for Codex.
- `.codex/agents/`: specialist Codex roles mapped to continuous workstreams.
- `.codex/skills/`: venture-specific local skills plus the AAS integration skill.
- `aas-stack.json`: a pinned Agentic Awesome Skills v15.4.0 manifest for Codex.
- `workflow/aas-skill-map.yaml`: exact AAS skill mappings for every role and workstream.
- `artifacts/templates/idea-to-mvp-workbook.md`: one living artifact for the whole MVP journey.
- `workflow/pipeline.yaml`: a machine-readable workstream map.
- `workflow/IDEA_TO_MVP.md`: the operating framework and external-action boundary.
- `workflow/START_HERE.md`: practical instructions and prompts for running a venture.
- `mvp-workflow.html`: a no-dependency responsive visual guide.

## Quick Start

1. Open this directory as a trusted Codex project.
2. Create a venture from the supplied template:

   ```sh
   cp -R ventures/_template ventures/<your-venture-slug>
   ```

3. Fill in `ventures/<your-venture-slug>/input/idea-brief.md` with every useful thought, not only a polished problem statement.
4. Copy `artifacts/templates/idea-to-mvp-workbook.md` into `ventures/<your-venture-slug>/artifacts/idea-to-mvp-workbook.md`.
5. In Codex, select the `venture-orchestrator` role and ask it to frame the venture and update the workbook.
6. Use specialist roles continuously as questions arise. They can research, define, design, build, and verify in parallel where useful.
7. Open `mvp-workflow.html` in a browser for the workstream guide.

## Suggested First Prompt

```text
Act as venture-orchestrator for venture <your-venture-slug>.
Read AGENTS.md, workflow/pipeline.yaml, workflow/IDEA_TO_MVP.md, aas-stack.json,
workflow/aas-skill-map.yaml, the idea brief, the current workbook, evidence, decisions,
and relevant app materials. Preserve every founder contribution as a commitment, preference,
hypothesis, inspiration, or open question. Use the founder-intent AAS methods when available.
Update the living workbook with a coherent product thesis, assumptions, evidence gaps, and the
highest-leverage next work. Do not contact anyone, spend money, publish, provision paid or
production resources, or take another external action without explicit authorization.
```

## Workflow Model

```text
Founder intent <-> Opportunity research <-> MVP definition
       ^                    |                    |
       |                    v                    v
       +-------------- Delivery and verification
                            |
                            v
                 Optional authorized learning and launch
```

The core endpoint is a reviewable, tested MVP package. Controlled beta, public launch, growth, and operations are optional post-MVP loops, not mandatory workflow stages.

## Important Constraints

- Internal work has no approval gates. Agents may revise research, scope, design, architecture, and implementation continuously while preserving history and rationale.
- External actions still require explicit founder authorization: outreach, publishing, spending, paid services, domains, credentials, production changes, deployment, personal-data handling, and public legal/security/performance claims.
- Research claims require source URLs, retrieval dates, direct evidence, and confidence levels.
- Agents must never invent customer interviews, commitments, market figures, test results, legal advice, or security attestations.
- Keep product and customer data out of prompts unless the required controls, consent, and redaction are in place.
- Use a separate product repository for generated application code when useful. Keep this repository as the venture context and evidence archive.

## Codex Compatibility

This project follows current Codex project-local conventions:

- Agent roles: `.codex/agents/*.toml`
- Skills: `.codex/skills/<skill-name>/SKILL.md`
- Repository instructions: `AGENTS.md`

Codex versions can differ in how their UI exposes specialist roles. If a role is not directly selectable, paste its `developer_instructions` into a Codex task or ask the main agent to use that role's file as its operating brief.

## Agentic Awesome Skills

This repository integrates [Agentic Awesome Skills](https://github.com/sickn33/agentic-awesome-skills) through the pinned `aas-stack.json` and `workflow/aas-skill-map.yaml`. AAS Core is the preferred integration: Codex searches the local catalog and validates the agent-selected manifest before any skill materialization. The map covers founder framing, research, business viability, product and UX definition, architecture, security, delivery, testing, accessibility, analytics, launch, and support.

To materialize the pinned Codex stack, first configure AAS Core through its documented preview flow, review the resulting plan, and only then apply it. The repository itself does not install third-party skills automatically.

## Recommended Automation

If this becomes an automated system, preserve the continuous workbook model. Use workflow automation for reminders, evidence collection, and traceability, not to recreate internal approval gates. Keep explicit authorizations for real-world side effects.
