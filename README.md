# Portfolio (MkDocs Material)

This is a ready-to-upload portfolio site for a **Mechatronics & Autonomous Systems Engineer**.  
It uses **MkDocs Material** and deploys automatically to **GitHub Pages** via Actions.

## Quick Start (no local install)
1. Create a new **public** repo on GitHub named `portfolio`.
2. Upload *all* files from this folder into the repo.
3. Go to **Settings → Pages** and set: **Build and Deployment: GitHub Actions**.
4. Push/commit — the site will build. Your site will be at:  
   `https://YOUR-USERNAME.github.io/portfolio`

## (Optional) Edit locally
- Install Python 3.10+
- `pip install -r requirements.txt`
- `mkdocs serve` → open http://127.0.0.1:8000
- `mkdocs build` (outputs to `site/`)

## Where to add content
- `docs/index.md` — your landing page (featured projects)
- `docs/projects/*` — one page per project
- `docs/projects/final-year-project/*` — multi-page dissertation
- `docs/modules/year-*.md` — year-by-year summaries
- `docs/about.md` — short bio + contact links

## Custom domain (optional)
- Buy a domain, add a CNAME in repo, and configure DNS to point to GitHub Pages.