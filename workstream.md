# Landing Page Workstream

This is the handoff note for ongoing `benbe.org` landing-page work.

## Current State

- The deployable site lives in `~/Projects/bench-beacon-site`.
- Vercel project: `bench-beacon`.
- Vercel root directory: `.`.
- Public URL currently verified: `https://www.benbe.org`.
- Current implementation is static HTML/CSS with no build step.
- Brand mark lives at `assets/bench-beacon-mark.svg`.
- Master/collaboration assets live in Drive:
  `Website - benbe.org`.

## Design Direction

The page should feel like a practical working surface, not a polished portal.

Keep:

- Bench & Beacon as the first-viewport signal.
- Clear link between weekly sessions, reviewed artifacts, and BenBe.
- Direct language over marketing language.
- Restraint: no big decorative system, no stock-like hero treatment.

Improve next:

- Sharpen the one-line offer.
- Decide whether the first CTA is a call, BenBe, sessions, or a mailing list.
- Add one better visual asset if it helps explain the work.
- Make the session archive easier to browse once public sessions are selected.
- Add a small credibility/proof section from real session outputs.

## Working Rules

- Treat every file here as public.
- Do not add raw transcripts, recordings, private attendee details, or secrets.
- Keep files under 300 lines unless Kenny explicitly approves the larger file.
- Use `README.md` for deployment facts.
- Use this file for design direction, backlog, and handoffs.
- Keep private infrastructure notes in `bench-beacon-ops`, not here.

## Verification

Before redeploying:

1. Open or serve the local page.
2. Check desktop and mobile with Playwright.
3. Confirm no horizontal overflow.
4. Confirm logo/assets load.
5. Confirm the live links still point where intended.

After deploy:

```bash
curl -I https://www.benbe.org
vercel ls bench-beacon --scope kenny-lius-projects-3a563320
```

## Open Questions

- What is the primary buyer/user on the first landing page?
- Should the first public offer be a diagnostic call, a session archive, or BenBe?
- How public should session artifacts be before the offer is clearer?
- Should `benbe.org` eventually redirect to `www.benbe.org`, or should apex stay canonical?
