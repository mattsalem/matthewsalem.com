# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Personal resume website for Matthew Salem (matthewsalem.com) - a static HTML/CSS/JS site styled as a MySpace/SpaceHey tribute page.

## Development

**Local Preview:**
```bash
python3 -m http.server 8080
```
Then open http://localhost:8080

**Deployment:**
- Hosted on Vercel with GitHub auto-deploy
- Push to `main` branch triggers automatic deployment
- Live at: https://matthewsalem.com

## Architecture

This is a single-page static site with no build process:

- `index.html` - Main resume page (all HTML, CSS, and JS inline)
- `option-*.html` - Alternative design explorations (not deployed)
- Image assets (`.png`, `.jpg`) - Logos, headshot, friend avatars
- `favicon.svg` - Site favicon
- `matthew-salem-resume.pdf` - Downloadable resume

## Key Features

- **SpaceHey/MySpace aesthetic** - Blue color scheme, table layouts, "Friend Space" section
- **Retro terminal stats panel** - DOS-style career metrics display
- **Collapsible experience section** - LinkedIn job hidden by default with toggle
- **Resume search** - Client-side text search with highlighting

## CSS Variables

Site uses CSS custom properties defined in `:root`:
- `--logo-blue`, `--darker-blue`, `--lighter-blue` - Primary blues
- `--light-orange`, `--dark-orange` - Accent colors for blurbs/friends sections
- `--gray`, `--dark-gray` - Neutral backgrounds
