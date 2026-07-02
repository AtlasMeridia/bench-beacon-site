# Landing Page Workstream

This is the handoff note for ongoing `benbe.org` landing-page work.

## Current State

- The deployable site lives in `~/Projects/bench-beacon/site`.
- Vercel project: `bench-beacon`.
- Vercel root directory: `.`.
- Public URL currently verified: `https://www.benbe.org`.
- Current implementation is static HTML/CSS with no build step.
- Active brand CSS is vendored at `assets/brand/colors_and_type.css`.
- Reviewed brand exports live under `assets/brand/`.
- Local brand workspace lives at `~/Projects/bench-beacon/brand`.
- Master/collaboration assets live in Drive:
  `Website - benbe.org`.
- Paper cleanup comp:
  `https://app.paper.design/file/01KWG0V1M2FV7NXM9KAJ2JK4VQ`.

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

2026-07-01 cleanup pass:

- Primary CTA is the working session.
- Secondary CTA stays internal to the page: `See the method`.
- Hero promise is now artifact-led: messy AI work becomes a cleaned packet and
  smaller next action.
- BenBe is framed as a bounded demo surface, not the whole offer.
- The first viewport includes a visible session-packet panel so the artifact is
  obvious before scrolling.

## Working Rules

- Treat every file here as public.
- Do not add raw transcripts, recordings, private attendee details, or secrets.
- Prefer files under 300 lines when practical; 300+ lines are a review trigger,
  not a hard stop. The active brand CSS is explicitly approved for vendoring
  as-is.
- Use `README.md` for deployment facts.
- Use this file for design direction, backlog, and handoffs.
- Use `~/Projects/bench-beacon/brand` for design-system source, logos, marks,
  illustrations, and mockups; copy only reviewed web-ready exports here.
- Use the light cream-paper surface for the public landing page by default.
- Keep private infrastructure notes in `~/Projects/bench-beacon/ops`, not here.

## Verification

Before redeploying:

1. Open or serve the local page.
2. Check desktop and mobile with Playwright.
3. Confirm no horizontal overflow.
4. Confirm logo/assets load.
5. Confirm the live links still point where intended.

Last local verification: 2026-07-01.

- Served from `http://127.0.0.1:4173/`.
- In-app browser screenshots checked at 1440x900 and 390x844.
- No horizontal overflow at either viewport.
- No browser console warnings or errors.
- Link HEAD checks: Cal.com 200, GitHub archive/session links 200,
  `chat.benbe.org` 302 to Cloudflare Access.

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
