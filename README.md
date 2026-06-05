# PyPI Version Info Viewer

A simple static HTML site that queries the PyPI JSON API and shows Python version support for **all releases** of a package.

Live site: https://15r10nk.github.io/pypi-version-info/

## Features

- Enter a package name (for example: `requests`)
- Loads all versions from PyPI
- Fetches metadata for each release
- Shows in a table:
  - `Requires-Python`
  - Python classifiers
  - release file `python_version` tags

## Run locally

You can open `index.html` directly in a browser.

## GitHub Pages deployment

This repository includes a GitHub Actions workflow at [.github/workflows/deploy-pages.yml](.github/workflows/deploy-pages.yml) that deploys the site to GitHub Pages.

### Steps to enable

1. Push this repository to GitHub.
2. In GitHub, open **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to **GitHub Actions**.
4. Push to `main` or `master` (or run the workflow manually via **Actions**).

After deployment, your site will be available at:

- `https://<your-user-or-org>.github.io/<your-repo>/`

## API used

- PyPI JSON API: <https://docs.pypi.org/api/json/>
