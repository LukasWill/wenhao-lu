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
- Featured Publications -> `_bibliography/papers.bib`, ordered newest first on the homepage.
- Selected Projects -> `_projects/*.md`.
- News -> `_news/*.md`.
- CV/Profile -> keep off the homepage unless a compact CV page is intentionally reintroduced.

The HugoBlox site currently keeps `content/site-notes/homepage-content-source.md` as a framework-neutral source of truth so the research narrative can be reused without copying theme-specific block syntax.
