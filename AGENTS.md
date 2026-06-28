---
last_updated: 2026-06-27
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

`~/Vaults/AtlasCortex/VENTURE/business-dev/bench-beacon/`

## Safety

Treat every committed file as public.

Do not commit:

- raw transcripts or recordings;
- private attendee/client details;
- unreviewed live docs;
- credentials, tokens, keys, or `.env` files;
- internal VPS/debug notes.

Master and collaboration assets live in the Bench & Beacon Google Drive folder
`Website - benbe.org`; commit only small web-ready exports here.

## Deployment

Vercel project: `bench-beacon`

Deploy from this repo root:

```bash
vercel --prod --yes --scope kenny-lius-projects-3a563320
```

