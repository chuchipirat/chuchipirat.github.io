# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is the **chuchipirat Helpcenter** — a Jekyll-based documentation site for the [chuchipirat](https://chuchipirat.ch) web app (a meal planning tool for youth organization camps). It uses the [Just the Docs](https://just-the-docs.com/) theme (v0.12.0, installed as a Ruby gem) and is deployed to GitHub Pages via the `deploy.yml` workflow on pushes to `main`.

All documentation content is written in **German**.

## Common Commands

```bash
# Install dependencies
bundle install
npm install        # first time only, for linters

# Serve locally (with live reload)
bundle exec jekyll serve

# Build the site (output to /tmp/chuchipirat-helpcenter-site, not _site/)
bundle exec jekyll build

# Serve via Docker
docker-compose up

# Lint CSS/SCSS and check formatting
npm test           # runs stylelint + prettier checks in parallel

# Auto-fix formatting
npm run format

# Run accessibility tests (requires Chrome/Chromium)
bundle exec rspec
```

## Architecture

### Build Output

The Jekyll build destination is set to `/tmp/chuchipirat-helpcenter-site` (in `_config.yml`) to avoid iCloud Drive sync conflicts. This means `_site/` is **not** used.

### Theme Customization

The site uses Just the Docs as a gem — most layouts, includes, and SCSS come from the gem. Local overrides:

- **`_layouts/`** — `default.html` and `minimal.html` wrap the theme's layouts; `table_wrappers.html` is a vendor layout for responsive tables
- **`_includes/`** — Customization hooks (`head_custom.html`, `header_custom.html`, `footer_custom.html`, etc.) are mostly empty placeholders; `head.html` adds GA tracking and search
- **`_sass/custom/`** — `custom.scss` and `setup.scss` are empty placeholders for adding custom styles
- **`_includes/vendor/anchor_headings.html`** — Vendored dependency, auto-updated via `.github/workflows/update_jekyll-anchor-heading.yml`

No custom Jekyll plugins exist in `_plugins/`.

### Callouts

Custom callout types are defined in `_config.yml` with German titles:

| Class | Title | Color |
|-------|-------|-------|
| `{: .highlight }` | Beachte | blue |
| `{: .important }` | Wichtig | yellow |
| `{: .new }` | Neu | green |
| `{: .note }` | Hinweis | petrol |
| `{: .warning }` | Achtung! | red |
| `{: .intern }` | ☠️ intern ☠️ | grey-dk |

## Content Structure

All documentation pages live under `docs/` organized by topic area:
- `docs/event/` — Event management (create, settings, menu plan, shopping list, etc.)
- `docs/recipe/` — Recipes (create, edit, publish, print, variants)
- `docs/masterdata/` — Master data (products, units, materials, departments)
- `docs/admin/` — Admin features (user management, system settings, jobs)
- `docs/user/` — User account (profile, password)
- `docs/home/`, `docs/others/`, `docs/request/`, `docs/communityleader/`

## Page Conventions

- Pages use Jekyll front matter with `layout: default` (applied automatically to everything in `docs/` via `_config.yml` defaults)
- Navigation hierarchy is controlled via front matter: `nav_order`, `parent`, `has_children`
- Internal links use Jekyll's `{% link docs/path/file.md %}` syntax — not raw relative paths
- Obsidian-style wiki links appear in HTML comments (`{::comment}[[pagename]]{:/comment}`) for cross-referencing in Obsidian; these are ignored by Jekyll
- Images are stored alongside their docs in `images/` subdirectories (e.g., `docs/event/images/`)

## Documentation Guidelines

### Sprache & Ton
- Alle Texte auf **Deutsch** (Schweizer Kontext, aber Hochdeutsch)
- Immer **du** (informell) — nie Sie
- Ton: freundlich, ermutigend, direkt. Keine Fachsprache ohne Erklärung
- Zielgruppe: Freiwillige in Jugendverbänden, die ein Lager planen. Kein technisches Vorwissen voraussetzen

### Seitenaufbau
Jede Dokumentationsseite folgt dieser Struktur:
1. Front matter mit `layout: default`, `nav_order`, `parent`, ggf. `has_children`
2. H1-Titel, gefolgt von `{: .no_toc }`
3. Einklappbares Inhaltsverzeichnis (`<details>/<summary>`)
4. **Einleitungsabsatz**: Was ist dieses Feature und warum brauche ich es?
5. Schritt-für-Schritt-Anleitung unter H2-Überschriften
6. Callouts für Hinweise/Warnungen
7. Links zu verwandten Seiten

### Callout-Verwendung
- `{: .note }` — Neutrale Zusatzinfo ("Hinweis")
- `{: .highlight }` — Tipps und Best Practices ("Beachte")
- `{: .important }` — Muss man wissen, bevor man weitermacht ("Wichtig")
- `{: .warning }` — Löschaktionen, irreversible Aktionen ("Achtung!")
- `{: .new }` — Neue Features ("Neu")

### Bilder
- Im Ordner `images/` neben den Markdown-Dateien ablegen (z.B. `docs/event/images/`)
- **Absolute Pfade** ab Site-Root verwenden: `![Alt-Text](/docs/event/images/dateiname.png)`
- Relative Pfade funktionieren NICHT korrekt, weil `permalink: pretty` die URL-Tiefe verändert
- Alt-Text soll beschreiben, was auf dem Bild zu sehen ist

### Verlinkung
- Interne Links mit Jekyll-Syntax: `{% link docs/pfad/datei.md %}`
- Obsidian-Links als HTML-Kommentar: `{::comment}[[seitenname]]{:/comment}`

### Vermeiden
- Keine Emojis im Fliesstext (Callout-Titel werden vom Theme gesteuert)
- Keine englischen Fachbegriffe ohne deutsche Erklärung in Klammern
- Keine `//`-Kommentare in Inline-JavaScript (`compress_html` entfernt sie und bricht den Code)

## CI

The CI workflow (`.github/workflows/ci.yml`) runs on PRs and pushes to `main`:
1. Jekyll build across Ruby 3.2/3.3/3.4 × Jekyll 3.9/4.3 on ubuntu/macOS/windows
2. GitHub Pages gem build test (ubuntu, Ruby 3.4)
3. HTML validation (Nu Validator + html-proofer)
4. CSS/JS linting via `npm test`
5. Accessibility testing via axe-core + RSpec + Capybara
