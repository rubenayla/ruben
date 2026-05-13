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
- Videos in `docs/videos/`. Policy: hero/loop videos self-hosted as MP4; demo videos (watched start-to-end) on YouTube. Hero MP4 = `kart-hero.mp4`.

## Gotchas
- **Raw HTML `<video src>` / `<iframe src>` relative paths are NOT rewritten by mkdocs** like markdown links are. A page at `/projects/kart/` (directory URL) referencing `../videos/X.mp4` resolves to `/projects/videos/X.mp4` (404). Use `../../videos/X.mp4` to reach `/videos/X.mp4`. Markdown image/link syntax does get rewritten — only raw HTML tags hit this.

## Related repos / sources
- **kart-docs (team repo)**: `/Users/rubenayla/repos/kart-docs` — MkDocs Material, public team technical reference. Same framework as this portfolio. URL: https://um-driverless.github.io/kart_docs/
- **kart LinkedIn campaign source**: `~/Library/CloudStorage/GoogleDrive-ruben.jimenezmejias@gmail.com/My Drive/ruben-files/videos/kart/linkedin/` — canonical source for the weekly LinkedIn posts that feed the portfolio's Build Journey. Each post is a folder under `posts/scheduled/<YYYY-MM-DD>_<slug>/` containing `post.md` (literal LinkedIn body), `rationale.md`, `history.md`, and media files. `published.md` is the durable archive of what's gone live. See that folder's own `AGENTS.md` for the full system.

## Build Journey
- **Single-page scroll**: all posts live in `docs/build-journey/index.md` as sequential `## <title> { #<anchor> }` sections, oldest first. No per-post pages — older split layouts have been removed. Each section has a stable URL via its anchor (e.g. `/build-journey/#motor`).
- **Per-post anatomy inside the index**:
  ```markdown
  ## <Editorial title> { #<anchor-slug> }

  *<YYYY-MM-DD> · [Original on LinkedIn →](<URL from published.md>)*

  <post body — see migration rules below>

  ![alt](../images/build-journey/<YYYY-MM-DD>-<slug>/<file>){ loading=lazy }
  ```
- **Adding a newly-published post** (triggered by step 11 of the LinkedIn campaign's `AGENTS.md` at-publish workflow):
  1. Confirm the post is in the LinkedIn folder's `published.md` (not just `scheduled/`).
  2. Append a new `## ... { #anchor }` section before the closing `*That's the latest post...*` stanza.
  3. Update the "Jump to:" line at the top to include the new anchor.
  4. Copy referenced images/thumbnails into `docs/images/build-journey/<YYYY-MM-DD>-<slug>/`.
  5. Strip LinkedIn-only cruft from `post.md`: trailing hashtag block, `@Ü Motorsport...` team-tag line, the docs-URL line if it duplicates an inline link.
  6. Restore `**bold**` / `*italic*` markdown that was flattened for LinkedIn (use `rationale.md` if it documents intended emphasis).
  7. All images get `{ loading=lazy }` — page weight grows with each post.
  8. Local build only; do not commit/push until user reviews (status promotions are user-only).
- **Future page split**: when the page gets unwieldy (~30+ posts, or load-time becomes noticeable), split by year — `index.md` becomes the latest, prior years move to `2026.md`, etc. Anchors per post are stable within each page.

## Video assets — validated-only rule
- For kart Story/Build-Journey embeds and YouTube uploads, source candidate videos from LinkedIn `published.md` (`Media used:` lines with `.mp4`) — never from `ls docs/videos/`. The raw repo MP4s are unvetted (some lack audio, some are weak clips); LinkedIn-published = user-validated.
- If no published videos exist yet, say so and wait — do not substitute repo MP4s.
- Exception: `kart-hero.mp4` (silent autoplay loop on the home page) is allowed to stay self-hosted regardless.
- YouTube URLs for kart videos are tracked in `.agents/youtube-urls.md`.
