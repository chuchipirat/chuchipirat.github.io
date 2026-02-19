# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is the **chuchipirat Helpcenter** — a Jekyll-based documentation site for the [chuchipirat](https://chuchipirat.ch) web app (a meal planning tool for youth organization camps). It uses the [Just the Docs](https://just-the-docs.com/) theme (v0.10.0) and is deployed to GitHub Pages via the `deploy.yml` workflow on pushes to `main`.

All documentation content is written in **German**.

## Common Commands

```bash
# Install Ruby dependencies
bundle install

# Serve locally (with live reload)
bundle exec jekyll serve

# Build the site (output to _site/)
bundle exec jekyll build

# Serve via Docker
docker-compose up

# Lint CSS/SCSS and formatting
npm install   # first time only
npm test      # runs stylelint + prettier checks
npm run format  # auto-fix formatting
```

## Content Structure

All documentation pages live under `docs/` organized by topic area:
- `docs/event/` — Event management (create, settings, menu plan, shopping list, etc.)
- `docs/recipe/` — Recipes (create, edit, publish, print, variants)
- `docs/masterdata/` — Master data (products, units, materials, departments)
- `docs/admin/` — Admin features (user management, system settings, jobs)
- `docs/user/` — User account (profile, password)
- `docs/home/`, `docs/others/`, `docs/request/`, `docs/communityleader/`

## Page Conventions

- Pages use Jekyll front matter with `layout: default` (applied automatically to everything in `docs/`)
- Navigation hierarchy is controlled via front matter: `nav_order`, `parent`, `has_children`
- Internal links use Jekyll's `{% link docs/path/file.md %}` syntax — not raw relative paths
- Obsidian-style wiki links appear in HTML comments (`{::comment}[[pagename]]{:/comment}`) for cross-referencing in Obsidian; these are ignored by Jekyll
- Callout blocks use the custom syntax: `{: .highlight }`, `{: .important }`, `{: .new }`, `{: .note }`, `{: .warning }`
- Images are stored alongside their docs in `_images/` subdirectories (e.g., `docs/event/_images/`)

## CI

The CI workflow (`.github/workflows/ci.yml`) runs on PRs and pushes to `main`:
1. Jekyll build across multiple Ruby/Jekyll version combinations
2. HTML validation (Nu Validator + html-proofer)
3. CSS/JS linting via `npm test`
