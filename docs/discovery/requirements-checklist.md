# Requirements Checklist — Discovery → Build gate

Items marked **(blocking)** must be resolved before any implementation work starts — `plan-gate` enforces this. Everything else can be filled in during build but should be decided here if known.

## Scope

- [x] v1 feature scope confirmed: marketing site + manual order form, no live stock/preview/tracking (2026-09-28) — `overview.md`
- [ ] Site map confirmed or amended — `site-map.md`
- [ ] Order form field list confirmed or amended — `site-map.md`

## Brand & content assets (blocking)

- [ ] Business name spelling/style, logo
- [ ] Brand colors/fonts (or "no preference, propose one")
- [ ] Product photos: stone + card samples
- [ ] Copy: About us / What's Raluek / Mongkol product description
- [ ] "How to order" steps (plain-language walkthrough)
- [ ] Stone meanings list (rough draft acceptable)

## Product & ordering details (blocking)

- [ ] What stones are actually offered at launch (even an approximate list — affects the stone-preference field and meanings page)
- [ ] Pricing: shown on site, or "contact for pricing" — final price is negotiated over chat at v1
- [ ] Delivery: methods/partners to mention on-site (note 1.b.iv/v), even if not automated
- [ ] Payment: how customers pay (bank transfer QR, etc.) and what the order form should tell them post-submit

## Legal & compliance (blocking)

- [ ] PDPA consent text for the order form (draft one if founders don't have it — needs legal review either way)
- [ ] Business registration status — affects whether a tax invoice is needed/offered (note 2.f.vi.1-2)

## Technical decisions

- [ ] Domain name choice/availability (.com / .co.th / other)
- [ ] Confirm or reject proposed stack — `tech-stack.md`
- [ ] Google Sheets as order store acceptable, or prefer a real DB from day one
- [ ] Social handles to link: Line OA ID, IG, FB, TikTok

## Launch logistics

- [ ] Target launch date
- [ ] Who owns processing orders from the spreadsheet day-to-day
- [ ] Hosting/domain budget ceiling, if any

---
When every blocking item above is checked, discovery is done and `plan-gate` allows build work to start.
