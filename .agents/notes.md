<!-- consult selectively — grep, never read in full -->
# Site Notes

## 2026-04-06 — Domain migration plan
Moving from `rubenayla.github.io/portfolio/` to `rubenayla.xyz`.
- Keeps GitHub Pages as host (static, zero maintenance)
- Cloudflare DNS CNAME points rubenayla.xyz to rubenayla.github.io
- MkDocs `site_url` already updated to https://rubenayla.xyz/
- Backlinks to rubenayla.xyz also strengthen partle.rubenayla.xyz (same root domain)
- Old URL should redirect (GitHub handles this automatically when custom domain is set)

## 2026-05-21 — Renamed repo portfolio → ruben
Repo + local dir renamed from `portfolio` to `ruben` (GitHub: `rubenayla/ruben`, local: `~/repos/ruben`). Reason: scope grew past a portfolio — it's now a personal hub (portfolio, writing, standards, references, ideas, things I like, CV — everything about me). Picked an identity-based name so it stays true if the domain changes (e.g. `.xyz` → `.com`); `ruben` over `rubenayla` to avoid the GitHub profile-repo special case (a repo named exactly the username renders its README on the profile page). Public URL unaffected (custom domain `rubenayla.xyz` via `docs/CNAME`); GitHub auto-redirects the old repo URL. External path reference updated in `~/repos/dv-hardware/.agents/tasks.md`.

## 2026-04-06 — Backlink strategy
High-DR profile sites for SEO backlinks. Profiles should be personal (Rubén as engineer) with Partle featured as a project. Bios drafted in partle repo at `.agents/posts/profile-bios.md`. Screenshots for dribbble/behance at `.agents/posts/screenshot-*.png`.

Target platforms: about.me (DR92), linktr.ee (DR92), behance (DR92), dribbble (DR91), crunchbase (DR91), producthunt (DR90), dev.to (DR90), gumroad (DR90), medium (DR94), carrd (DR89), hashnode (DR88), substack (DR88), indiepa.ge (DR67).
