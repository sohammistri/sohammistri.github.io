# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Jekyll-based academic portfolio website hosted on GitHub Pages, built on the [academicpages](https://github.com/academicpages/academicpages.github.io) template (derived from Minimal Mistakes theme).

## Development Commands

```bash
# Install dependencies (first time or after Gemfile changes)
bundle install

# Serve locally with live reload (preferred for development)
bundle exec jekyll liveserve

# Serve locally without live reload
bundle exec jekyll serve

# Build static site only (no server)
bundle exec jekyll build

# Clean build artifacts
bundle clean
```

Local server runs at `http://localhost:4000`. The dev config (`_config.dev.yml`) overrides the production URL and disables analytics automatically when using `liveserve`.

## Architecture

### Content Collections

Content lives in named collection directories and is rendered via layouts:

- `_publications/` — Academic papers with metadata (title, venue, date, paperurl, citation)
- `_talks/` — Conference/seminar talks with location data
- `_teaching/` — Courses taught
- `_portfolio/` — Portfolio projects
- `_posts/` — Blog posts
- `_pages/` — Standalone pages (about, CV, archives)

Each collection item is a Markdown file with YAML front matter. Collections are configured in `_config.yml`.

### Content Generation

`markdown_generator/` contains Python scripts/notebooks to bulk-generate collection Markdown from data files:

- `publications.tsv` + `publications.py` → `_publications/*.md`
- `talks.tsv` + `talks.py` → `_talks/*.md`
- `pubsFromBib.py` — Convert BibTeX to publication Markdown

### Templates

- `_layouts/` — Page templates (`default`, `single`, `archive`, `talk`, `splash`)
- `_includes/` — Reusable fragments (author profile, sidebar, comments, analytics, nav)
- `_sass/` — SCSS stylesheets overriding/extending the Minimal Mistakes theme
- `_data/navigation.yml` — Top navigation menu structure

### Key Config Files

- `_config.yml` — Site title, author info, collections, plugins, analytics
- `_config.dev.yml` — Development overrides (local URL, no analytics, expanded SASS)
- `_data/navigation.yml` — Navigation menu

## Deployment

Pushing to the `master` branch automatically deploys to GitHub Pages at `https://sohammistri.github.io`. No manual build step needed.
