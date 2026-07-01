# wenyin-portfolio

## Cursor Cloud specific instructions

This repo is a **zero-build, dependency-free static website** (a personal design portfolio). It is plain HTML/CSS/vanilla-JS with inline `<style>`/`<script>`, plus image assets under `images/`. There is no package manager, no build step, no tests, no lint config, and no backend/database.

- **Pages:** `index.html` (landing), `loans-onboarding.html`, `lions-share-loyalty.html`.
- **Run (dev):** serve the repo root over HTTP, e.g. `python3 -m http.server 8000`, then open `http://localhost:8000/`. Opening files via `file://` also works but HTTP is preferred so relative asset paths resolve cleanly.
- **Build / lint / test:** none exist. There is nothing to install or compile.
- **External dependency:** the only remote asset is the Google Fonts "DM Sans" webfont loaded via CDN in each page's `<head>`. It is non-blocking — pages fall back to a system sans-serif if the CDN is unreachable.
