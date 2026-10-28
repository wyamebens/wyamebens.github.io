# Wyame Benslimane — personal website

Source for my academic website: bio, publications, CV, and teaching & service.

Built with [Jekyll](https://jekyllrb.com/) and the [al-folio](https://github.com/alshedivat/al-folio) theme (MIT licensed, see `LICENSE`).

## Structure

| Path | Content |
| --- | --- |
| `_pages/about.md` | Home page: bio and profile photo |
| `_pages/publications.md`, `_bibliography/papers.bib` | Publications list (edit the `.bib` file to add papers) |
| `_pages/cv.md`, `assets/pdf/resume.pdf` | CV page; replace the PDF to update it |
| `_pages/teaching.md` | Teaching & Service: teaching, service, talks, honors |
| `_config.yml`, `_data/socials.yml` | Site settings and social links |

## Run locally

Requires Ruby (3.3+ recommended).

```bash
bundle config set --local path vendor/bundle
bundle install
bundle exec jekyll serve --livereload
```

Then open <http://localhost:4000/>.

## Deploy

Pushing to `main` runs `.github/workflows/deploy.yml`, which builds the site and publishes it to the `gh-pages` branch for GitHub Pages.
