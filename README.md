# IPOFINDS

Standalone IPO tracking website. This project does not modify or depend on Yoqart.

## Pages
- `/index.html` — dashboard + home calendar
- `/ipos.html` — IPO directory
- `/gmp.html` — GMP tracker
- `/calendar.html` — full calendar
- `/ipo/*.html` — dedicated IPO pages

## Current mode
Demo data is embedded for testing navigation and UI. The data layer is designed to be replaced by a Cloudflare Worker endpoint without exposing an API key.

## Cloudflare Pages
Repository root must contain `index.html`. Framework: None. Build command: blank. Build output directory: blank.

## Live API
See `worker/index.js`. Configure the provider URL and API key as Worker secrets/environment variables; never put the key in `assets/app.js` or GitHub.
