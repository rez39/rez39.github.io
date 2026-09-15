# rez39.github.io

Personal / academic website for C. Rajashekar Reddy, built on the [al-folio](https://github.com/alshedivat/al-folio) Jekyll theme. Deployed automatically to GitHub Pages via `.github/workflows/deploy.yml` on every push to `main`.

## Updating content

- **New publication:** add a BibTeX entry to `_bibliography/papers.bib`. Set `selected: true` to feature it on the home page, and `abbr` to show a short venue tag.
- **News item:** add a file to `_news/`, named `YYYY-MM-DD-slug.md`, with `inline: true` for a one-line item (see existing files for the format).
- **Project page:** add a file to `_projects/`.
- **Bio / CV / contact info:** `_pages/about.md`, `_data/cv.yml`, `_data/socials.yml`.

## Local preview

```bash
bundle install
bundle exec jekyll serve
```

Requires Ruby and Bundler; see [al-folio's install docs](https://github.com/alshedivat/al-folio/blob/master/docs/INSTALL.md) for details.
