# Wenhao Lu — Academic and Technical Portfolio

Personal portfolio for Wenhao Lu, a Research Associate and PhD researcher at the University of Hamburg working across reinforcement learning, robot learning, and agent interpretability.

The site is built with [Hugo](https://gohugo.io/) and [HugoBlox](https://hugoblox.com/). Content is stored as Markdown; local presentation overrides live under `layouts/` and `assets/css/`.

## Local development

Requirements:

- Hugo Extended 0.162.0
- Node.js 22
- pnpm 10
- Go 1.19 or newer

```bash
pnpm install
pnpm run dev
```

The configured GitHub Pages base path is `/hugo-academic-cv/`.

## Production build

```bash
pnpm run build
```

The build renders the static site into `public/` and then creates the Pagefind search index. Generated output, Hugo resources, and dependencies are intentionally ignored by Git.

## Content map

- `content/_index.md` — homepage narrative and calls to action
- `content/publications/` — complete publication record and paper links
- `content/projects/` — contribution-led project pages
- `content/blog/` — concise research updates
- `data/authors/me.yaml` — shared identity and affiliation data
- `assets/media/` — profile and publication imagery

Do not publish draft project pages until their title, status, and public artifacts are verified.
