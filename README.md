# Bench & Beacon Site

Static first-pass landing page for `benbe.org`.

For ongoing design work, start with
[`workstream.md`](./workstream.md).

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

## Current Deployment

- Production deployment: `dpl_7DPriyRsJZLjHaqqxgTQGQwNRwfS`
- Stable checked URL: `https://www.benbe.org`
- DNS: `benbe.org` and `www.benbe.org` point to `76.76.21.21`

Deploy manually from the repo root:

```bash
cd /Users/atlas/Projects/bench-beacon-site
vercel --prod --yes --scope kenny-lius-projects-3a563320
```
