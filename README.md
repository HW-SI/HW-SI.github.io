# Haowen Si Personal Website

This repository contains the source for my personal academic website: https://hw-si.github.io.

The visible site is now a custom static HTML/CSS GitHub Pages site. It presents my current work in high-energy astrophysics, black-hole jet modeling, microquasars, multi-messenger predictions, and previous research experience in dark matter searches, solar-wind MHD, and stellar spectroscopy.

## Site Structure

The public website is intentionally small:

- `index.html` - home page, research focus, current project, modeling context, and contact
- `research/index.html` - current and previous research project descriptions
- `blog/index.html` - blog landing page for group posts, research notes, and updates
- `cv/index.html` - CV summary and PDF link
- `assets/css/site.css` - custom site styling inspired by compact academic research pages
- `files/CV_HWSI.pdf` - downloadable CV
- `images/` - profile images, research images, and original schematic artwork used by the pages

`.nojekyll` disables Jekyll processing, so GitHub Pages serves the static files directly. Some older AcademicPages files may remain in the repository for reference, but they are no longer part of the active website.

## Editing Content

Use the static HTML files for page content and `assets/css/site.css` for styling. The top navigation is repeated in each page, so update all pages if the navigation changes.

## Blog Posts

For now, the blog page is a static landing page. When posts are ready, add each post as a static HTML file under `blog/` and link it from `blog/index.html` and the homepage blog section.

## Figures

Current pages use original schematic artwork in `images/` for the homepage, research page, and blog header:

- `microquasar-hero.png`
- `jet-medium-interaction.png`
- `multimessenger-pipeline.png`
- `microquasar-smbh-comparison.png`
- `blog-research-notes-header.png`

See `FIGURE_PROMPTS.md` for the prompts and quality criteria used to generate or refine these figures.

## Running Locally

No Ruby or Jekyll build is required. To preview locally, run:

```bash
python3 -m http.server 4000
```

The site will be available at http://localhost:4000.

## Deployment

GitHub Pages builds and deploys the `master` branch automatically. Changes merged into `master` will appear at https://hw-si.github.io after the Pages build finishes.

## Theme Credit

The original repository was based on AcademicPages, a fork of Minimal Mistakes for academic websites. The visible site is now custom static HTML/CSS.
