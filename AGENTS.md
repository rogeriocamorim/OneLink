# AGENTS.md

## Project

Static "link-in-bio" page for Maple Designs Creations. Single `index.html` with inline CSS/JS — no framework, no build step, no dependencies.

## Structure

- `index.html` — entire app (HTML + inline styles + inline JS)
- `.github/workflows/deploy.yml` — deploys repo root to GitHub Pages on push to `main`

## Development

Open `index.html` in a browser. There is no dev server, build, or install step.

## Deployment

Push to `main` triggers GitHub Pages deploy via Actions. The repo root is served as-is — no build artifact.

## Conventions

- All styles and scripts are inline in `index.html` (no external CSS/JS files)
- CSS uses custom properties defined in `:root` (maple/autumn color theme)
- External dependency: Google Fonts (`Playfair Display`, `Inter`) loaded via CDN
- No linter, formatter, or tests are configured
