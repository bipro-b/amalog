# Prep Log

A 28-week interview prep tracker — daily routine, DSA log, system/low-level designs, mocks, leadership stories, and a company pipeline. Single static HTML file, no build step, no backend. All data lives in the browser's `localStorage`.

## Deploy

1. Push this folder to a new GitHub repo (branch `main`).
2. Repo **Settings → Pages → Source: GitHub Actions**.
3. The included workflow deploys on every push. Site URL: `https://<username>.github.io/<repo>/`

## Data

- Stored under the `prep-log-v1` key in `localStorage`, scoped to the site's origin.
- Use **Progress → Download backup** regularly. Restore with **Restore backup**.
- Moving from another host (or a different domain) means a new origin — export there, import here.

## Structure

```
index.html                     # the whole app
.nojekyll                      # skip Jekyll processing
.github/workflows/pages.yml    # GitHub Pages deploy
```
