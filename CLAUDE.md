# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Static website for **The Shchepinova Lab**, an academic research group at the University of Bath, UK. Built with plain HTML and CSS — no frameworks, no build tools, no JavaScript dependencies.

## Architecture

- **Pages**: `index.html` (home), `about.html` (lab info + team), `news.html` (updates), `contact.html` (address + map)
- **Styling**: Single shared stylesheet at `css/style.css` using CSS custom properties (variables in `:root`)
- **Assets**: `images/` directory for logo, team photos, and other media
- **Navigation & footer**: Duplicated in each HTML file (no templating system). When modifying nav or footer, update all four pages.

## Development

Open `index.html` directly in a browser — no server required. Refresh to see changes.

## Key Conventions

- University of Bath brand blue: `#003E74` (stored as `--bath-blue` CSS variable)
- All placeholder content is marked with `<!-- TODO: ... -->` HTML comments
- Responsive design via media queries at 768px breakpoint
- Mobile nav uses a simple JS toggle (`.nav-links.open` class)
- No external font or icon dependencies — uses system font stack
