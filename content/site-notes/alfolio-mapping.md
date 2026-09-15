---
title: al-folio Mapping
draft: true
build:
  render: never
  list: never
---

# al-folio Mapping

Use this note when porting the HugoBlox staging content back to the main al-folio site.

- Hero identity, research positioning, institutional profile, and opportunity signal -> `_pages/about.md` and `_data/socials.yml`.
- Research Focus -> a concise expertise section in `_pages/about.md`; preserve the distinction between demonstrated methods and current directions.
- Selected Publications -> `_bibliography/papers.bib`, with four representative entries on Home and the complete record on the publications page.
- Selected Work -> three evidence-led `_projects/*.md` entries on Home; the projects archive retains the complete four-item public set.
- Selected Updates -> `_news/*.md`, limited to three recent milestones on Home.
- Professional Activities -> `_pages/about.md` or `_data/cv.yml`.
- CV/Profile -> keep off the homepage unless a compact CV page is intentionally reintroduced.

The HugoBlox site currently keeps `content/site-notes/homepage-content-source.md` as a framework-neutral source of truth so the research narrative can be reused without copying theme-specific block syntax.
