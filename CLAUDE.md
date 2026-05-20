# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Static HTML/CSS landing page — no build system, package manager, or backend. Open `index.html` directly in a browser or serve with any static file server.

## Development

To preview locally, run a simple HTTP server from the project root:

```powershell
# Python (if available)
python -m http.server 8080

# Node.js (if available)
npx serve .
```

## Architecture

Two files:

- `index.html` — single-page layout with a fixed navbar, full-height hero section, and a 3-column features grid
- `styles.css` — all styles; uses CSS Grid/Flexbox, `clamp()` for responsive typography, and `backdrop-filter` for the navbar glassmorphism effect

No JavaScript, no preprocessors, no external dependencies (all styles are hand-written CSS).
