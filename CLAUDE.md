# Raluek

Custom greeting cards paired with a gemstone ("Mongkol" product line). Thailand-market, ordered/fulfilled manually at launch via Line/IG/FB/TikTok.

## Phase: Discovery

No application code yet, by design. Work right now is confined to `docs/discovery/` until `docs/discovery/requirements-checklist.md` is finalized. See the `plan-gate` skill for the rule this enforces.

## Decisions so far (2026-09-28, not yet final — see checklist)

- v1 website = marketing/info site + a manual order form (reference code, PDPA consent). No live stone stock, no live card-preview builder, no order-tracking page yet.
- Ops run off a spreadsheet manually. No internal admin tool in v1.
- Proposed stack (pending confirmation): Next.js + Tailwind on Vercel, order form → Google Sheets via API route.

Full context: `docs/discovery/overview.md`. Site map: `docs/discovery/site-map.md`. Stack rationale: `docs/discovery/tech-stack.md`.

## Conventions

- Planning docs live under `docs/discovery/` while in discovery; later phases get their own `docs/<phase>/` folder rather than overwriting these.
- Source of truth for "what's decided vs. open" is `docs/discovery/requirements-checklist.md` — keep it current when a decision is made in conversation.

## Skills

- `plan-gate` — gates implementation work behind the discovery checklist and, later, behind an approved plan.
- `change-summary` — end-of-session recap of what changed/was decided/is still open.
- `token-lean` — terse response style for chat and tool use; exempts docs written for human/cofounder reading.
