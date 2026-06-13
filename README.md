# imhaving.fun

Personal CV + **IMAF & H Consulting** site for **Michael House** — served by GitHub Pages at [imhaving.fun](https://michaelhouse.cv). This repo holds both the source and the deployed static output (single hand-written `index.html`, no build step).

| | |
|---|---|
| **Live (custom domain)** | https://imhaving.fun |
| **Live (GitHub default)** | https://sablister.github.io/pleasesendgrants/ |
| **Stack** | HTML + CSS, inline; Google Fonts via CDN |

## Files
- `index.html` — the site (self-contained: inline CSS/JS)
- `404.html` — minimal not-found page
- `CNAME` — custom domain (`imhaving.fun`)
- `.nojekyll` — serve files as-is (skip Jekyll)
- `assets/banner.txt`, `assets/terminal.txt` — raw ASCII used in the terminal panel
- `github-profile-README.md` — ASCII profile block to paste into a repo named `SABLISTER/SABLISTER`

## Content provenance
All content is drawn from the live sites **www.mike.condos** (CV) and **nothelp.help** (IMAF & H Consulting). No biographical details were invented; the nonprofit template's placeholder social links were excluded.

## GitHub Pages settings
Settings → Pages → Build and deployment → Source: **Deploy from a branch** → Branch **main** / **/(root)** → Save.
Custom domain: **imhaving.fun** → enable **Enforce HTTPS** once DNS resolves.

## DNS (DreamHost) — apex domain
```
A     @     185.199.108.153
A     @     185.199.109.153
A     @     185.199.110.153
A     @     185.199.111.153
CNAME www   sablister.github.io.
```
Remove any existing DreamHost A record on `@` that points to a DreamHost server (or set the domain to "DNS only") so it doesn't conflict.

## Update
Edit `index.html`, commit to `main` — Pages redeploys in ~1 minute.
