<!-- consult selectively — grep, never read in full -->
# Error Log

## 2026-04-06 — mkdocs serve path prefix issue
**What:** `mkdocs serve` adds `/portfolio/` prefix based on `site_url`, causing 404s on localhost.
**Root cause:** MkDocs serve uses site_url to compute paths.
**Prevention:** Always use `uv run mkdocs build && python3 -m http.server 8005 --directory site` for local preview. Documented in AGENTS.md.
