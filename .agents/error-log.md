<!-- consult selectively — grep, never read in full -->
# Error Log

## 2026-04-06 — mkdocs serve path prefix issue
**What:** `mkdocs serve` adds `/portfolio/` prefix based on `site_url`, causing 404s on localhost.
**Root cause:** MkDocs serve uses site_url to compute paths.
**Prevention:** Always use `uv run mkdocs build && python3 -m http.server 8005 --directory site` for local preview. Documented in AGENTS.md.

## 2026-05-13 — Asked the user to re-export videos that were already local
**What:** User picked three kart videos from Google Photos (cone-slalom, first-autonomous-run, dashboard-handheld) for portfolio + LinkedIn draft use. I created sidecars and draft rationale entries marking each as "pending export from Google Photos," and even drafted ffmpeg commands for the user to run. The user pushed back: *"it should be available already with our videos. I just looked at Google Photos and all the videos were stored there. We exported from there to get our set of videos locally."* A 60-second `ffprobe` sweep of `~/ruben-files/videos/kart/01_main/` found an exact match for the slalom video (`sec7_kart_with_cones_camera_mast.MOV`, 1920×1080, 28.38s) — the local pool I should have searched **before** declaring anything pending.
**Root cause:** I treated Google Photos screenshots as the canonical source and never checked the local raw-media pool that the LinkedIn campaign's own `AGENTS.md` explicitly documents as the shared kart-media pool (`media/` symlink to `../01_main/`). The path was in front of me — I just didn't traverse it. Same failure mode as the "grep all instances before declaring done" pattern: I solved the user's surface ask without sanity-checking the premise.
**Prevention:**
- **Before recommending a re-export, re-download, or any user-side data fetch**, exhaustively check local sources. For kart videos: `find ~/ruben-files/videos/kart/01_main -type f \( -iname "*.mp4" -o -iname "*.mov" \)` + `ffprobe` matching on duration/resolution against the screenshot's metadata.
- The kart raw-media pool has a canonical INDEX.md at `~/ruben-files/videos/kart/01_main/INDEX.md` — read it before suggesting exports. It also documents the deliberate choice of a central INDEX over per-file sidecars (2026-04-22 history), so future media-metadata work should go in INDEX.md's Reserved/Used/Tagged tables, not duplicated as sidecars unless they serve a different scope (e.g., portfolio-local ratings).
- General rule: any time the next action is "user does work," budget ≥1 minute proving the work isn't already done before asking.
