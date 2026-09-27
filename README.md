# Hin Chu Group website

An HKUMed research group website based on the [HugoBlox Developer Portfolio](https://github.com/HugoBlox/hugo-theme-developer-portfolio) template (MIT license). It is adapted for research themes, publications, news, and a dedicated People page.

## Current content

- **Home:** group introduction, three research themes, recent highlights, and contact information.
- **People:** Professor Hin Chu and Tianrenzheng Zhu, the first PhD student profile supplied by the group.
- **Publications:** a short sourced selection, with links to the official profile and papers.
- **News:** three sourced HKU research highlights.

Factual sources and follow-up content items are in [CONTENT_SOURCES.md](CONTENT_SOURCES.md). The public site is published at [hin-chu-group.github.io](https://hin-chu-group.github.io/).

## Preview locally

Use Hugo Extended **0.162.0**, Go, Node.js, and pnpm 10.14.0. The template's GitHub Actions workflow installs the exact Hugo version listed in `hugoblox.yaml`.

```sh
pnpm install
ln -sf ../@tailwindcss/cli/dist/index.mjs node_modules/.bin/tailwindcss
hugo server --disableFastRender
```

Open `http://localhost:1313/`. The symlink lets Hugo call Tailwind's Node entry point; the deployment workflow applies the same fix.

## Edit content

| What | File or folder |
| --- | --- |
| Home sections | `content/_index.md` |
| Navigation | `config/_default/menus.yaml` |
| Site identity and colors | `config/_default/params.yaml` |
| People page layout | `content/people/_index.md` |
| Member profiles | `data/authors/*.yaml` |
| Member photos | `assets/media/authors/` |
| Research themes | `content/projects/` |
| News | `content/blog/` |
| Selected publications | `content/publications/index.md` |

The local `team-showcase` and author-card overrides in `layouts/_partials/` keep profile links correct when GitHub Pages serves the site below a repository path.

## Publish to GitHub Pages

Push this site to the `main` branch of [`hin-chu-group/hin-chu-group.github.io`](https://github.com/hin-chu-group/hin-chu-group.github.io). In **Settings → Pages**, select **GitHub Actions** as the source. The included workflow builds and deploys the site.

The HugoBlox source remote is named `template`; the group's repository is named `origin`.
