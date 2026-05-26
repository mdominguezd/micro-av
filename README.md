# quarto-site

A minimal website built with [Quarto](https://quarto.org), deployed automatically to GitHub Pages via GitHub Actions.

## Repo structure

```
.
├── _quarto.yml                  # Project config (theme, navbar, output dir)
├── index.qmd                    # Home page
├── about.qmd                    # About page
├── styles.css                   # Custom CSS overrides
└── .github/workflows/publish.yml  # CI/CD: renders & deploys on push to main
```

## Deploy in 3 steps

1. **Push this repo to GitHub.**

2. **Enable GitHub Pages** in your repo settings:  
   `Settings → Pages → Source → GitHub Actions`

3. **Push any commit to `main`** — the workflow builds the site with Quarto and deploys it automatically.

Your site will be live at `https://<your-username>.github.io/<repo-name>/`.

## Local preview

```bash
# Install Quarto: https://quarto.org/docs/get-started/
quarto preview
```

## Adding pages

1. Create a new `.qmd` file (e.g. `blog.qmd`).
2. Add it to the `navbar` section of `_quarto.yml`.
