# Agent guidelines

This is Eli McKown-Dawson's personal site: a small, plugin-light Jekyll site (no theme gem) deployed by `.github/workflows/deploy.yml` to the `gh-pages` branch, which serves emckowndawson.com (see `CNAME`).

- Content lives in `_data/*.yml` (bylines, projects, papers, cv). Prefer editing data over templates.
- Templates: `_layouts/` and `_includes/`. Styles: `assets/css/main.css` only, with color tokens at the top (Ink navy palette, light and dark).
- Fonts: Newsreader (body/headings), Public Sans (UI), IBM Plex Mono (dates, labels), loaded from Google Fonts in `_layouts/default.html`.
- Keep it lean: no JavaScript frameworks, no new plugins unless GitHub Pages-safe and clearly needed.
- Before committing, run `bundle exec jekyll build` and check the pages at desktop and phone widths in light and dark mode.
- Old URLs must keep working; add a file in `redirects/` when moving a page.
