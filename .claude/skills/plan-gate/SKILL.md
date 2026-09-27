---
name: plan-gate
description: Use before creating or editing any implementation file (code, config, infra, dependencies) in this repo. Blocks build work on Raluek while it's in the discovery phase, and once past discovery, requires an approved plan before multi-file or architecture-affecting edits.
---

# Plan Gate

Raluek is in **discovery**: the cost of building the wrong thing is higher than the cost of asking first.

## Rule

1. Check `docs/discovery/requirements-checklist.md`. If any item marked "must resolve before build" is unchecked, the project is still in discovery:
   - Allowed without asking: creating/editing files under `docs/`, `CLAUDE.md`, `.claude/`.
   - Not allowed without explicit sign-off: application code, framework scaffolding, new dependencies, hosting/build config.
   - If asked to do build work anyway, name the open checklist items and confirm the user wants to proceed ahead of them before doing it.

2. Once the checklist is finalized and build work starts: before a change that touches more than one file, or introduces a new dependency, pattern, or architecture decision, use EnterPlanMode and get approval before editing. Trivial, obviously-scoped single-file edits don't need this.

3. An earlier approval covers the scope it was given for, not later work that shifts scope — re-check when that happens.
