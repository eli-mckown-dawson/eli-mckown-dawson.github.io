# emckowndawson.com

Personal site of Eli McKown-Dawson, built with [Jekyll](https://jekyllrb.com/) and published to GitHub Pages.

## Updating content

Almost everything on the site comes from four data files in `_data/`. You can edit them on github.com; the site rebuilds and publishes a minute or two after you commit.

| To change…                     | Edit                  |
| ------------------------------ | --------------------- |
| Bylines (Writing page, home)   | `_data/bylines.yml`   |
| Data & models projects, charts | `_data/projects.yml`  |
| Research papers                | `_data/papers.yml`    |
| CV                             | `_data/cv.yml`        |

**Add a byline:** copy an entry to the top of `_data/bylines.yml` and change the title, URL, outlet and date (`YYYY-MM`). Add `featured: true` to show it under "Selected" on the home page.

**Add a project:** put the chart image in `assets/img/charts/` (WebP or PNG, about 1000px wide) and add an entry to `_data/projects.yml`. The first project is the large feature on the home page; the next three are the cards under it.

The bio is in `index.html`, and the contact details and social links are in `_config.yml`.

## Running locally

```bash
bundle install
bundle exec jekyll serve
```

Then open http://localhost:4000.

## Layout

- `_layouts/` and `_includes/` hold the page templates.
- `assets/css/main.css` is the only stylesheet. Colors are defined once at the top.
- `redirects/` keeps old URLs (`/bylines/`, `/academic/`, `/polling/`, `/contact/`) working.
- `.github/workflows/deploy.yml` builds the site and publishes it to the `gh-pages` branch.
