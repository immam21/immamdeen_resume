# Immamdeen S. — Portfolio

A single-page, static portfolio site (`index.html`) with an SRE monitoring-dashboard visual theme. No build step, no framework — just HTML/CSS/JS.

## Files
- `index.html` — the entire site (styles + script inline)
- `resume.pdf` — downloadable résumé, linked from the nav, hero, and contact section

## Deploy to Vercel

### Option A — Vercel CLI (fastest)
```bash
npm i -g vercel
cd portfolio
vercel
```
Follow the prompts (link/create a project, accept defaults — no build command needed since it's static). Then `vercel --prod` to push to production.

### Option B — GitHub + Vercel dashboard
1. Push this folder to a new GitHub repo.
2. Go to vercel.com → **Add New Project** → import the repo.
3. Framework preset: **Other** (Vercel auto-detects static HTML). Leave build command empty, output directory as root.
4. Deploy.

## Customizing
- Colors, fonts, and spacing are all CSS variables at the top of `index.html` (`:root`) — change once, applies everywhere.
- To swap the résumé, just replace `resume.pdf` with the same filename.
- Update contact details, links, and copy directly in the HTML — every section is clearly labeled with comments (`<!-- HERO -->`, `<!-- SKILLS -->`, etc.).
- If you want a custom domain, add it under Project → Settings → Domains once deployed.
