# Job Market Website (Quarto)

## What's here
- `_quarto.yml` — site config (nav bar, theme)
- `index.qmd` — Home
- `about.qmd` — About Me
- `research.qmd` — Research (job market paper + working papers)
- `teaching.qmd` — Teaching
- `cv.qmd` — CV (links to `cv.pdf`, which you need to add)
- `styles.css` — light custom styling

## Before you publish, fill in:
- Your last name (in `_quarto.yml` and `index.qmd`)
- Real email address, LinkedIn, GitHub links (`_quarto.yml`)
- `headshot.jpg` — add a photo to the project root (or delete the `![](headshot.jpg)` line in `index.qmd`)
- `cv.pdf` — add your CV to the project root
- Bracketed placeholder text in `about.qmd`, `teaching.qmd`, and the two working paper blurbs in `research.qmd`
- Links to actual paper PDFs/drafts in `research.qmd`
- Professors Fleck's and Hanssen's full names/titles and links on `index.qmd` if you want to credit them there

## 1. Install Quarto
Download the CLI from https://quarto.org/docs/get-started/ (free, one-click installer for Mac/Windows/Linux).

## 2. Preview locally
From this folder, run:
```
quarto preview
```
This opens a live-reloading local preview in your browser.

## 3. Publish to GitHub Pages (free hosting)
1. Create a new GitHub repo (e.g. `jobmarket-site`) and push this folder to it.
2. From this folder, run:
```
quarto publish gh-pages
```
This builds the site and pushes it to a `gh-pages` branch automatically.
3. In the repo's Settings → Pages, confirm the source is set to the `gh-pages` branch. Your site will be live at:
```
https://yourusername.github.io/jobmarket-site/
```
4. Update `site-url` in `_quarto.yml` to match, and re-publish.

## Updating the site later
Just edit the relevant `.qmd` file and re-run `quarto publish gh-pages`. No separate hosting dashboard to manage.
