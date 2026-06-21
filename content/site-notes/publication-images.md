---
title: Publication Image Maintenance
draft: true
build:
  render: never
  list: never
---

# Publication Image Maintenance

Publication illustrations use Hugo page bundles. Each publication directory contains its Markdown page and a replaceable image:

```text
content/publications/<publication-slug>/
|-- index.md
`-- featured.png
```

HugoBlox automatically selects an image whose filename contains `featured`. No image path needs to be added to the front matter.

## Replacing a Placeholder

1. Prepare a 16:9 PNG, JPEG, or WebP image. A width of at least 1200 pixels is recommended.
2. Replace that publication's `featured.png` while keeping the filename.
3. Keep `image.preview_only: true` in `index.md` to show the image in publication lists without adding a large image to the publication page.
4. Run `hugo --cleanDestinationDir --minify` and inspect the homepage and Publications page.

Use figures that remain legible at thumbnail size. Prefer a visual overview or representative result over a dense full-page screenshot. Avoid adding text that duplicates the paper title already displayed beside the image.

## Adding a New Publication

Create a new page bundle under `content/publications/`, add `featured.png`, and include:

```yaml
image:
  preview_only: true
```

The illustrated list layout is selected in:

- `content/_index.md` for the homepage Featured Publications block.
- `content/publications/_index.md` for the Publications page.

The local view implementation is under `layouts/_partials/views/publication-illustrated*.html`. It does not modify the HugoBlox module.

## al-folio Equivalent

The main al-folio site uses the BibTeX `preview` field and stores thumbnails in `assets/img/publication_preview/`. When porting an image back, copy it there and set `preview = {filename.png}` on the corresponding entry in `_bibliography/papers.bib`.
