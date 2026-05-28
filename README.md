# weinanhu-site

Personal academic website. Built with [Quarto](https://quarto.org); deployed via Cloudflare Pages from the `gh-pages` branch (produced by GitHub Actions on every push to `main`).

## Local preview

```bash
quarto preview
```

## Manual render

```bash
quarto render
```

Output goes to `_site/`.

## Deploy

Pushing to `main` triggers `.github/workflows/publish.yml`, which renders the site and pushes `_site/` to the `gh-pages` branch. Cloudflare Pages is configured to serve the `gh-pages` branch.

## Structure

```
_quarto.yml             # site config
index.qmd               # home
about.qmd               # about
research/               # listing + per-project qmd files
blog/                   # listing + posts/
assets/                 # cv.pdf, avatar.jpg, ...
styles.css              # minimal overrides
.github/workflows/      # CI render + deploy
```
