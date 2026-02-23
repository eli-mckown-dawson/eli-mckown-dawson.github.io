# Project Memory: eli-mckown-dawson.github.io

## Overview
Personal website for Eli McKown-Dawson — Senior Elections Analyst at Silver Bulletin.
- Live site: https://emckowndawson.com/
- GitHub: https://github.com/eli-mckown-dawson/eli-mckown-dawson.github.io
- Theme: al-folio (Jekyll static site)
- Hosting: GitHub Pages with custom domain via CNAME

## Current State (as of 2026-02-23)
**Mid-migration** from a previous theme to al-folio. Many placeholders still in place:
- `_pages/about.md`: Bio paragraphs are placeholder text, no profile image set
- `_data/cv.yml`: Education and experience are mostly placeholders
- `_bibliography/papers.bib`: Empty (just `---` front matter)
- `_posts/`, `_projects/`, `_news/`: Still contain al-folio demo content (not yet replaced with real content)
- Blog settings in `_config.yml` still say "al-folio" (demo defaults)

## Key Files
| File | Purpose |
|------|---------|
| `_config.yml` | Main site config — name, URL, features, plugins |
| `_pages/about.md` | Homepage (layout: about, permalink: /) |
| `_pages/cv.md` | CV page (uses rendercv format) |
| `_data/cv.yml` | CV content data |
| `_data/socials.yml` | Social media links |
| `_bibliography/papers.bib` | Publications (BibTeX) |
| `assets/img/prof_pic.jpg` | Profile picture (file exists but not set in about.md) |
| `CNAME` | Custom domain: emckowndawson.com |

## Config Settings of Note
- `url: https://emckowndawson.com`, `baseurl:` (empty) — correct for custom domain
- `scholar.last_name: [McKown-Dawson]`, `first_name: [Eli, E.]` — set correctly
- `cv_format: rendercv` in cv.md
- `enable_darkmode: true`, `enable_math: true`, `enable_masonry: true`
- Nav: only "about" (/) and "CV" (/cv/) are active in navbar

## Social Links (in socials.yml)
- email: eli.inquiries68@gmail.com
- github: eli-mckown-dawson
- x/twitter: emckowndawson
- linkedin: eli-mckown-dawson
- orcid: 0000-0003-4209-6963
- google scholar: -stdPpQAAAAJ

## What Needs Doing (migration TODOs)
- Fill in bio paragraphs in about.md
- Set profile image in about.md (`image: prof_pic.jpg`)
- Complete cv.yml with real education/experience data
- Add publications to papers.bib
- Replace demo _posts, _projects, _news content with real content
- Update blog_name and blog_description in _config.yml
- Add CV PDF path
- Decide which pages to keep in nav (blog, projects, publications, etc.)

## Dev Workflow
- Local dev: Docker (`docker compose up` → http://localhost:8080)
- Pre-commit: `npx prettier . --write`, then verify build
- See AGENTS.md / .github/copilot-instructions.md for full guidelines
