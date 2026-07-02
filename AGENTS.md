---
last_updated: 2026-07-01
---

# Bench & Beacon Site

This repository is the public source for `benbe.org`.

## Scope

Keep this repo focused on the deployable public website:

- static HTML/CSS/JS;
- web-ready image and SVG assets;
- public deployment config;
- public design/deployment notes in `README.md` and `workstream.md`.

Project memory, session notes, offer work, and broader Bench & Beacon context
belong in the AtlasCortex vault bundle at:

`~/Vaults/AtlasCortex/VENTURE/bench-beacon/`

## Safety

Treat every committed file as public.

Do not commit:

- raw transcripts or recordings;
- private attendee/client details;
- unreviewed live docs;
- credentials, tokens, keys, or `.env` files;
- internal VPS/debug notes.

Master and collaboration assets live in the Bench & Beacon Google Drive folder
`Website - benbe.org`; local brand-system and asset staging lives at
`~/Projects/bench-beacon/brand`. Commit only small reviewed web-ready exports here.

## Brand System

Use `~/Projects/bench-beacon/brand` as the source of truth before creating or
changing visual design.

- Vendor `brand/system/css/colors_and_type.css` into this deploy repo when the
  site needs the active tokens. This is explicitly approved even though the file
  exceeds the usual 300-line review threshold.
- Use reviewed exports from `brand/assets/**/exports/`; do not copy archive
  files directly into production.
- The public landing page should use the light cream-paper brand surface by
  default. Reserve `workbench` mode for product/agent panels and `observatory`
  mode for media/title-card moments.

## Deployment

Vercel project: `bench-beacon`

Deploy from this repo root:

```bash
vercel --prod --yes --scope kenny-lius-projects-3a563320
```
