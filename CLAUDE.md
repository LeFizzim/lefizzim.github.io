# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a GitHub Pages personal site (lefizzim.github.io) using Jekyll with the `jekyll-theme-midnight` theme. It serves as a landing page linking to browser games and apps.

## Development Commands

```bash
# Install dependencies
bundle install

# Run local development server
bundle exec jekyll serve

# Build site without serving
bundle exec jekyll build
```

## Architecture

- **Jekyll Site**: Uses GitHub Pages gem with jekyll-theme-midnight
- **Content**: `index.md` is the main page; `README.md` is used as alternate index via jekyll-readme-index plugin
- **Custom Layout**: `_layouts/default.html` overrides the theme's default layout to add logo display, custom styling, and Google site verification
- **Output**: `_site/` contains generated static files (gitignored)
- **Dependencies**: `vendor/bundle/` contains Ruby gems (gitignored)

## Key Files

- `_config.yml` - Site configuration (title, theme, plugins, logo path)
- `index.md` - Main page content with front matter
- `_layouts/default.html` - Custom layout with logo, flexbox styling, and SEO tags
