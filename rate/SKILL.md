---
name: rate
description: Rate proposed tasks, review remediations, or options by the user's required involvement. Use when asked to /rate work or apply an involvement-based difficulty rating.
---

# Rate

Measure the user's involvement, not elapsed time, implementation complexity, or
severity. When rating a finding, rate the work required to remediate it.

## Establish the evidence

Inspect the relevant artifacts and exhaust available, authorized independent
research before classifying work as needing the user's intervention. Resolve
questions from code, documentation, existing decisions, and accessible systems
yourself. Research the agent can complete is agent work, not user involvement.

Keep the requested scope: a rating request authorizes investigation, not
implementation or publication. If research needs unavailable access or exceeds
the authorized scope, state that limit and the specific next probe. Do not
invent certainty or pursue unbounded research to avoid an unknown rating.

## Choose a rating

- **oneshottable** — no user involvement needed; existing scope and evidence
  suffice. Name the entry point, affected files or artifacts, and the check that
  would prove completion. Without that evidence, use **unknown**.
- **immediately solvable** — one to four concrete answers from the user would
  make the work independently executable. Name the questions; do not count
  questions the agent can answer through research.
- **requires intervention** — after independent research, the work still needs
  substantive user discussion, planning, judgment, or decisions beyond a few
  concrete answers. Name the user-only decision and why it blocks execution.
- **unknown** — evidence is insufficient to categorize the work. Explain the
  uncertainty and name one probe that would resolve it, including whether the
  agent can run that probe or needs access or authorization.

Unknown is an evidence state, not a higher difficulty tier. A large refactor
can be oneshottable; a tiny behavior change can require a product decision.

## Report

Give each task or option its label, the evidence supporting it, and a recommended
next action. For every non-oneshottable item, identify what prevents a lower
involvement rating. Separate verified facts, inference, and uninspected areas.

Flag severity and blast radius separately when relevant. Oneshottable does not
waive review or authorization for migrations, destructive operations, production
credentials, or publication. An understood task awaiting approval can retain its
rating with the approval gate stated separately.

Use a short paragraph for one item or a compact table for several. Avoid time
estimates and a numeric score. Re-rate when new evidence or user answers resolve
the uncertainty.
