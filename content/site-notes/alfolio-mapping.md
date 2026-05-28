---
title: al-folio Mapping
draft: true
build:
  render: never
  list: never
---

# al-folio Mapping

Use this note when porting the HugoBlox staging content back to the main al-folio site.

- Hero/profile -> `_pages/about.md` and `_data/socials.yml`.
- Research Themes -> a custom include or Markdown section on `_pages/about.md`.
- Selected Projects -> `_projects/*.md`.
- Featured Publications -> `_bibliography/papers.bib` with selected/featured entries.
- News -> `_news/*.md`.
- CV/Profile -> `_data/cv.yml` or `assets/json/resume.json`.
- Technical Capabilities -> `_pages/about.md`, `_pages/cv.md`, or a reusable include.

The HugoBlox site currently keeps `content/site-notes/homepage-content-source.md` as a framework-neutral source of truth so the research narrative can be reused without copying theme-specific block syntax.
