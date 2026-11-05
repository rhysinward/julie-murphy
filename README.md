# Julie Murphy

Professional website built with [Quarto](https://quarto.org), published with GitHub Pages.

## Preview locally

1. Install [Quarto](https://quarto.org/docs/get-started/) 1.10 or later. The published site is built with 1.10.19.
2. Run `quarto preview` in this folder. It does not always pick up changes to `.yml` or `.scss` files, so if an edit does not appear, stop it, run `quarto render`, and start it again.

## Where things live

| To change | Edit |
|---|---|
| Headline, introduction, profile, quote, impact, contact, short bio | `index.qmd` |
| Career timeline and Board and industry leadership | `career.yml` (instructions at the top of the file) |
| Speaking and press | `news.yml`. `lead: true` shows an item before "Show more" |
| Colours and fonts | `assets/theme.scss`, the `:root` block |
| Navigation and footer | `_quarto.yml` |
| Search engine details (job title, links) | `assets/person.html` |

## Dates

Only enter what is on record. A date known only to the year stays as `"2019"` and never shows a month. A role with no date on record uses `lane: undated` and is listed in words, not drawn on the chart. In `news.yml` use `when`, not `date`, because Quarto rewrites `date` and invents a day.

The timeline works out "today" when the page loads, so the years count and current roles stay correct without a rebuild.

## Publish

1. Create a GitHub repository and push this folder to `main`.
2. Run `quarto publish gh-pages` once, then set Settings → Pages to the `gh-pages` branch.
3. Every push to `main` then republishes the site through `.github/workflows/publish.yml`.
