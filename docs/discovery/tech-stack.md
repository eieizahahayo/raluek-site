# Tech Stack — proposed, not yet confirmed

Recommendation, made without a stated preference from the founders (see chat 2026-09-28). Revisit once requirements-checklist.md's technical-decisions section is checked off.

- **Framework**: Next.js + Tailwind. Content-driven site with one form; grows into the full note-4 customization engine later without a rewrite.
- **Hosting**: Vercel free tier — fast to ship, easy custom domain.
- **Order storage**: Google Sheets as the database (form → API route → Sheets API). Matches "manual/spreadsheet ops" directly — the team works the sheet, no separate admin tool needed yet, zero cost.
- **Image uploads**: Vercel Blob or Cloudinary free tier, linked from the sheet row.

## Why not alternatives

- Hosted store builder (Shopify-style): overkill for a form-and-catalog site with no live checkout in v1; revisit if v1.1 adds real payments/stock.
- Fully custom backend/DB now: no need until order volume or feature set (live stock, tracking) outgrows a spreadsheet.

## Depends on (from requirements-checklist.md)

- Domain choice
- Whether a formal DB is wanted from day one instead of Sheets (e.g. if founders don't want to hand-manage a spreadsheet)
- Budget/hosting constraints, if any
