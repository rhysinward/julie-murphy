# Julie Murphy

Professional website built with [Quarto](https://quarto.org), published with GitHub Pages.

## Preview locally

1. Install [Quarto](https://quarto.org/docs/get-started/) 1.5 or later.
2. Run `quarto preview` in this folder. The site opens in your browser and reloads as you edit.

## Where things live

| To change | Edit |
|---|---|
| Headline, introduction, what I do, quote, contact text | `index.qmd` |
| Current roles (the cards) | `roles.yml` |
| Career history | `career.yml` |
| Press, speaking and awards | `news.yml` |
| Colours and fonts | `assets/theme.scss`, the `:root` block |
| Navigation and footer | `_quarto.yml` |

Text in `[square brackets]` shows as a dashed placeholder until it is filled in.

## Publish

1. Create a GitHub repository and push this folder to `main`.
2. Run `quarto publish gh-pages` once, then set Settings → Pages to the `gh-pages` branch.
3. Every push to `main` then republishes the site through `.github/workflows/publish.yml`.
