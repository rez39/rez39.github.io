# Site conventions for rez39.github.io

This is Raj's personal/academic site, built on the al-folio Jekyll theme (v1.x, gem-based runtime — layouts/includes live in the `al_folio_core` gem, not in this repo).

## Where content lives

- **Publications** — `_bibliography/papers.bib`. One BibTeX entry per paper. Use `abbr` for the short venue tag, `selected: true` to feature it on the home page, `pdf: <filename>` for a PDF under `assets/pdf/`, `preview: <filename>` for a thumbnail under `assets/img/publication_preview/`. Posters/demos go in the same file, just without `selected`.
- **News** — one file per item under `_news/`, named `YYYY-MM-DD-slug.md`. Use `inline: true` in the front matter for a short one-liner (body text becomes the item). Sort order is by the `date` field, not filename.
- **Projects** — one file per project under `_projects/`, `layout: page`, with `related_publications: true` and a `{% cite bibkey %}` tag to link back to the matching `_bibliography` entry.
- **Bio / timeline / academic service** — `_pages/about.md`.
- **CV** — `_data/cv.yml` (structured, rendered on `/cv/`) plus the actual PDF at `assets/pdf/Rajashekar_CV.pdf`, referenced from `_pages/cv.md`.
- **Contact / social links** — `_data/socials.yml` (email, github_username, linkedin_username, scholar_userid, cv_pdf).

## Working conventions

- Never commit straight to `main`. Make changes on a branch and push it; Raj opens/merges the PR himself (or asks for one to be opened).
- Only add facts Raj has actually provided or that are independently verifiable (e.g. from a co-author's site, a DOI, an official acceptance notice) — never invent bibliographic details, dates, or award names.
- The deploy workflow (`.github/workflows/deploy.yml`) builds via Jekyll + GitHub Actions using the existing "Actions" Pages source — don't switch it to a gh-pages-branch deploy method without checking the repo's Pages settings first, since that needs a manual settings change on GitHub.
- Ruby gem installs (`bundle install`) require rubygems.org, which is not reachable from this sandbox — the real build only happens in GitHub Actions after pushing. Validate YAML/BibTeX syntax locally where possible before pushing.
