# Bench & Beacon Site

Static first-pass landing page for `benbe.org`.

For ongoing design work, start with
[`workstream.md`](./workstream.md).

The active Bench & Beacon brand source lives outside this deploy repo at
`~/Projects/bench-beacon/brand`; reviewed CSS/assets are vendored into
`assets/brand/` when used by the static site.

## Vercel Settings

- Project name: `bench-beacon`
- Project ID: `prj_11S5pKiDrmrqqPbdUUtAFHtWD2pv`
- Team: `Atlas Meridia` (`kenny-lius-projects-3a563320`)
- Git repository: `AtlasMeridia/bench-beacon-site`
- Root Directory: `.`
- Framework Preset: Other
- Build Command: none
- Output Directory: `.`
- Production domains: `benbe.org`, `www.benbe.org`

`chat.benbe.org` stays on the VPS behind Cloudflare Access.

## Deployment Verification

- Stable checked URL: `https://www.benbe.org`
- DNS: `benbe.org` and `www.benbe.org` point to `76.76.21.21`
- Latest production deployment changes on push; verify with
  `vercel ls bench-beacon --scope kenny-lius-projects-3a563320`.

Deploy manually from the repo root:

```bash
cd /Users/atlas/Projects/bench-beacon/site
vercel --prod --yes --scope kenny-lius-projects-3a563320
```
