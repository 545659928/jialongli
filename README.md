# Hugo Personal Website

This repository contains a Hugo-based personal website managed with Markdown and deployed with GitHub Pages.

## Project Structure

- `content/_index.md`: homepage
- `content/01-research.md`: research page
- `content/02-publications.md`: publications page
- `content/03-students.md`: students page
- `content/04-cv.md`: CV page
- `content/05-jp.md`: Japanese page
- `layouts/`: Hugo templates
- `static/css/site.css`: site styles
- `hugo.toml`: site configuration
- `.github/workflows/hugo.yml`: GitHub Pages deployment workflow

## How To Update Content

Most edits only require changing Markdown files in `content/`.

- Update the homepage in `content/_index.md`
- Update research information in `content/01-research.md`
- Add or revise publications in `content/02-publications.md`
- Update students information in `content/03-students.md`
- Update CV information in `content/04-cv.md`
- Update Japanese content in `content/05-jp.md`

## How To Update The Sidebar Or Navigation

- Edit `hugo.toml` for site-wide settings such as title, menu items, and profile links
- Edit `layouts/partials/sidebar.html` for the left sidebar
- Edit `layouts/_default/baseof.html` for the shared page layout

## Local Preview

If Hugo is installed locally, run:

```bash
hugo server -D
```

Then open the local preview URL shown in the terminal.

## How To Publish Updates

After editing files, publish changes with:

```bash
git add .
git commit -m "Update website content"
git push
```

GitHub Actions will automatically rebuild and deploy the site after the push.

## GitHub Pages Setup

1. Push this repository to the `main` branch.
2. Open `Settings -> Pages` in GitHub.
3. Set `Source` to `GitHub Actions`.
4. Wait for the workflow in `Actions` to finish successfully.

## Notes

- Keep this repository public-safe: do not place private notes, unpublished documents, or sensitive personal information here.
- If using a custom domain, add `static/CNAME` and update `baseURL` in `hugo.toml`.
