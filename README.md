# Haowen Si Personal Website

This repository contains the source for my personal academic website: https://hw-si.github.io.

The site is built with Jekyll and the AcademicPages theme. It presents my current work in high-energy astrophysics, black-hole jet modeling, microquasars, multi-messenger predictions, and previous research experience in dark matter searches, solar-wind MHD, and stellar spectroscopy.

## Site Structure

The public website is intentionally small:

- `_pages/about.md` - home page and research overview
- `_pages/cv.md` - CV summary and PDF link
- `_pages/research.html` - research project descriptions
- `_pages/sitemap.md` - generated sitemap page
- `files/CV_HWSI.pdf` - downloadable CV
- `images/` - profile and research images used by the pages

Most of the original AcademicPages demo pages, posts, talks, teaching entries, portfolio entries, and sample publication files have been removed so the repository reflects the actual website rather than the template.

## Editing Content

Use the files in `_pages/` for page content. The main site settings, author profile, social links, and repository metadata live in `_config.yml`. Top navigation is controlled by `_data/navigation.yml`.

After changing `_config.yml`, restart the local Jekyll server because Jekyll does not reload config changes automatically.

## Running Locally

Install Ruby and Bundler, then run:

```bash
bundle install
bundle exec jekyll serve -l -H localhost
```

The site will be available at http://localhost:4000.

## Deployment

GitHub Pages builds and deploys the `master` branch automatically. Changes merged into `master` will appear at https://hw-si.github.io after the Pages build finishes.

## Theme Credit

This site uses AcademicPages, a fork of Minimal Mistakes for academic websites. The theme code remains under the original license in `LICENSE`.
