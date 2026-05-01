# Haowen Si Personal Website

This repository contains the source for my personal academic website: https://hw-si.github.io.

The site is built with Jekyll and the AcademicPages theme. It presents my current work in high-energy astrophysics, black-hole jet modeling, microquasars, multi-messenger predictions, and previous research experience in dark matter searches, solar-wind MHD, and stellar spectroscopy.

## Site Structure

The public website is intentionally small:

- `_pages/about.md` - home page, research focus, visual context, and blog preview
- `_pages/research.html` - current and previous research project descriptions
- `_pages/blog.html` - blog index for group posts, research notes, and updates
- `_pages/cv.md` - CV summary and PDF link
- `_pages/sitemap.md` - generated sitemap page
- `_pages/tag-archive.html` and `_pages/category-archive.html` - lightweight archives for future blog posts
- `files/CV_HWSI.pdf` - downloadable CV
- `images/` - profile and research images used by the pages

The original AcademicPages demo pages, posts, talks, teaching entries, portfolio entries, and sample publication files have been removed so the repository reflects the actual website rather than the template.

## Editing Content

Use the files in `_pages/` for page content. The main site settings, author profile, social links, and repository metadata live in `_config.yml`. Top navigation is controlled by `_data/navigation.yml`.

Style overrides are kept in `_includes/head/custom.html` so the AcademicPages theme remains easy to update.

## Blog Posts

Add blog posts as Markdown files named like this:

```text
_posts/YYYY-MM-DD-short-title.md
```

A minimal post looks like:

```markdown
---
title: "Post title"
date: 2026-05-01
categories:
  - blog
tags:
  - microquasars
excerpt: "One-sentence summary for the blog index."
---

Post body.
```

## Figures

Current pages use the existing credited research images in `images/`. See `FIGURE_PROMPTS.md` for suggested prompts if you want to generate original schematic-style figures later.

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
