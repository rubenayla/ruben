# Engineering Notes for Agents

## Local Development & Preview Protocol

To avoid common pitfalls with MkDocs serving and port conflicts, follow this protocol for previewing the portfolio.

### 1. Reliable Site Serving
Do **not** use `mkdocs serve` for final verification. It can introduce path prefixes (like `/portfolio/`) based on the `site_url` config, which causes confusion and 404 errors. Instead, build the site and serve the static files directly.

**Command:**
```bash
uv run mkdocs build && nohup python3 -m http.server 8005 --directory site > /dev/null 2>&1 &
```

### 2. Handling Port Conflicts
If the server fails to start or shows a 404/Connection Refused, port `8005` is likely held by a stale process. Forcefully clear it before starting a new server.

**Cleanup Command:**
```bash
lsof -ti:8005 | xargs kill -9
```

### 3. Verification Protocol
- **Check the Port:** Always verify if something is listening before telling the user to visit the URL.
- **Verify Content:** Use `curl -I http://127.0.0.1:8000/index.html` to confirm a `200 OK` response.
- **Pathing:** Serving from the `site/` directory ensures `http://127.0.0.1:8000` maps directly to `index.html`.

### Why this matters
Using the standard `mkdocs serve` often results in "This site can't be reached" or 404 errors because:
1. It might bind to an address/port that is already partially occupied.
2. It enforces a URL structure (based on `site_url`) that doesn't match the root localhost address.
3. It relies on a "live-reload" server that can hang or become unresponsive if the process isn't terminated correctly.
