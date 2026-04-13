# Hugo Personal Website

This repository contains a Markdown-managed personal website built for Hugo and ready to deploy on GitHub Pages.

## Structure

- `content/_index.md`: homepage content
- `content/research.md`: research page
- `content/publications.md`: publication list
- `content/cv.md`: CV page
- `layouts/`: custom Hugo templates
- `static/css/site.css`: site styles
- `.github/workflows/hugo.yml`: GitHub Pages deployment workflow

## How To Edit

Most future updates only require editing Markdown files under `content/`.

- Update homepage text in `content/_index.md`
- Add or revise papers in `content/publications.md`
- Update appointments, awards, and funding in `content/cv.md`
- Adjust research directions in `content/research.md`

## GitHub Pages Deployment

1. Create a GitHub repository for this folder.
2. Push the contents to the `main` branch.
3. In GitHub, open `Settings -> Pages`.
4. Set `Source` to `GitHub Actions`.
5. The included workflow will build and deploy the site automatically.

If you want to use a custom domain, add a `static/CNAME` file and update `baseURL` in `hugo.toml`.

## Local Preview

Install Hugo locally, then run:

```bash
hugo server -D
```
