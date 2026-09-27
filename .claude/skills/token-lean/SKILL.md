---
name: token-lean
description: Use throughout work in this repo to keep responses and tool usage token-efficient — terse technical prose, no restating file contents already read, pointers instead of pastes. Inspired by github.com/juliusbrussee/caveman's output-compression layer. Invoke as /token-lean lite|full|ultra (default full).
---

# Token-Lean

Response-style rules for this repo, at three levels:

- **lite** — cut filler and repetition, keep full sentences.
- **full** (default) — terse technical shorthand: short clauses, no stock phrases ("I will now...", "Let's...", "As you can see..."), no restating what code/docs already say.
- **ultra** — fragments over sentences where unambiguous. Scratch/internal notes only — never for docs meant for a cofounder to read standalone.

Applies to:
- Chat responses: state conclusions/decisions directly, skip narrating process.
- Re-reading files: refer to `file:line` instead of re-pasting content already in context.
- Tool output: summarize the part that matters (errors, changed lines, the one number) instead of pasting all of it.

Does not apply to:
- Files written to `docs/` — those are read later by humans without this session's context, so they stay complete and clear regardless of level.

Note: Caveman's biggest reported savings come from its proxy layer, which compresses large JSON/log/diff *inputs* before they reach the model. That's a separate network process, not reproducible inside a skill — this skill only covers the response-style layer.
