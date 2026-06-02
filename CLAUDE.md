# mohingu.github.io - Personal Portfolio

Static personal portfolio site (plain HTML/CSS/JS, no build step). Deployed via
GitHub Pages from `main` to https://mohingu.github.io.

## Structure
- `index.html` - single page: Hero, About, Experience, Education, Projects,
  Certificates, YouTube, Contact, Footer.
- `styles/` - modular CSS, one file per section, plus `base.css` (CSS variables
  + theming), `components.css`, `navbar.css`, `responsive.css` (mobile).
- `script.js` - theme toggle, mobile hamburger nav, rotating hero text, scroll
  effects, dynamic footer year.
- `images/profile.jpg` - profile photo (compressed; keep under ~300KB).
- `assets/Mohin_Uddin_CV.pdf` - REDACTED CV (no phone, postcode, or email).
  Never commit the unredacted CV - it exposes personal contact details.

## Previewing locally (IMPORTANT)
- Serve over HTTP, not `file://`. On `file://` the YouTube embeds and CV link
  fail (null origin -> YouTube "Error 153"). Run:
  `python3 -m http.server 8000` then open http://127.0.0.1:8000
- The browser caches CSS/JS aggressively. After editing, **hard refresh
  (Cmd+Shift+R)** or tick "Disable cache" in DevTools > Network. A plain reload
  shows stale styles - this caused repeated "my change isn't showing" confusion.

## Theming & layout
- Dark/light via `[data-theme]` on `<html>`; all colours are CSS variables in
  `styles/base.css`.
- Cards use `--surface` / `--surface-border` so they stay visually distinct from
  section backgrounds (sections alternate `--bg-primary` / `--bg-secondary`).
  Do not give cards `--bg-glass` on a `--bg-primary` section - they vanish.
- Centred hero is intentional (dominant dev-portfolio style); no background photo
  behind the headline (it clashed with the centred text).
- YouTube: DarkMohinxP = landscape 16:9 videos; MohinxP = vertical 9:16 Shorts
  (`.video-grid--shorts` / `.video-embed--short`).

## Conventions
- UK spelling throughout (analyse, specialise, visualisation).
- Work on a feature branch and open a PR into `main`; do not commit to `main`.

## Deploy
- Merging to `main` auto-deploys via GitHub Pages (live in ~1-2 minutes).
