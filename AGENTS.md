# AGENTS.md

## Architecture

Static single-page site with no build step. Netlify publishes the `public/` directory directly (see `netlify.toml`).

## Key files

- `public/index.html` — the entire site: markup, inline `<style>`, and inline `<script>` for the countdown/redirect.
- `netlify.toml` — sets the publish directory.

## Conventions and notes

- Keep everything self-contained in `index.html` unless the site grows; the owner supplied this page as finished HTML, so preserve its design and copy unless asked to change them.
- The Telegram invite URL appears twice (button `href` and `TELEGRAM_URL` constant) — keep them in sync.
- The countdown ring uses an SVG circle with `r=26`; `stroke-dasharray` in CSS (163.36) must match `2πr` if the radius changes.
- External assets (fonts, Font Awesome, Unsplash profile image) load from CDNs.
