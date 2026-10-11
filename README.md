# dateme

Shay's date-me page: a single static page served by GitHub Pages at
<https://shaywei.github.io/dateme/>.

## What is here

- `index.html` – the whole profile. Edit the text directly; each section is a plain `<section>`.
- `style.css` – all styling. Colours and fonts are CSS variables at the top of the file, with a
  dark theme that follows the visitor's system setting.
- `images/` – photos resized for the web with metadata stripped. Each has a 1600px version and an
  800px version for phones; `og.jpg` is the picture shown when the link is shared.
- `favicon.svg` – the tab icon.
- `.github/workflows/pages.yml` – deploys the repository root to GitHub Pages on every push to `main`.

## Publishing

Pages is configured with **Settings → Pages → Build and deployment → Source: GitHub Actions**.
After that one-time setting, every push to `main` runs the workflow and the site updates within a
minute or two. Nothing needs building locally.

## Search engines

`index.html` carries `<meta name="robots" content="noindex">`, so the page is reachable by anyone
with the link but is not meant to show up in search results. Delete that line to allow indexing.
