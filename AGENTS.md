<!-- read in full — kept under 150 lines -->
# Portfolio — Agent Guide

Personal portfolio site for Rubén Jiménez Mejías. Static site built with MkDocs Material, hosted on GitHub Pages.

## Quick Reference
- Live: https://rubenayla.xyz/ (moving from rubenayla.github.io/portfolio/)
- Repo: https://github.com/rubenayla/portfolio
- Stack: MkDocs Material (Python), deployed via GitHub Pages
- Domain: rubenayla.xyz (Cloudflare DNS)

## Structure
```
docs/
  index.md          — homepage
  about.md          — personal bio, links, CV
  projects/         — one .md per project
  images/           — project images organized by subfolder
  files/            — CV PDFs, downloadable files
mkdocs.yml          — site config, nav, theme
```

## Local Development
Do NOT use `mkdocs serve` — it has path prefix issues. Instead:
```bash
uv run mkdocs build && python3 -m http.server 8005 --directory site
```
Then visit http://localhost:8005/. Kill stale processes with `lsof -ti:8005 | xargs kill -9`.

## Agent Files
- `.agents/tasks.md` — task board (TODO / In Progress / Done)
- `.agents/notes.md` — project notes, decisions, context
- `.agents/error-log.md` — mistake log

## Conventions
- No emojis in content (user preference)
- Keep descriptions technical and concise
- Images go in `docs/images/{project-name}/`
- Downloadable files go in `docs/files/`
