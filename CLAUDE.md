# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a static landing page for Tiny Dictation, a lightweight Windows dictation app. The site is pure HTML/CSS with no build system, bundler, or dependencies.

## Architecture

- **index.html** - Main landing page with product features, comparison chart, API provider list, and feature screenshots
- **pricing.html** - Pricing page with Stripe checkout integration
- **Assets** - PNG screenshots, app icon, and a hero video (webm)

## Development

No build process required. Open HTML files directly in a browser or use any static file server.

## Key Design Patterns

- CSS variables defined in `:root` for consistent theming (colors: `--primary`, `--text`, `--bg`, etc.)
- All styles are inline in `<style>` tags within each HTML file
- Mobile responsiveness via `@media (max-width: 768px)` breakpoints
- CSS-only hamburger menu using checkbox hack (no JavaScript)
- CSS-only lightbox for screenshot zoom using `:target` pseudo-class
- Font: Space Grotesk (Google Fonts) for logo, system fonts for body

## Styling Conventions

- Dark theme with gradient background (`--gradient`)
- Cards/features use glassmorphism effect (`backdrop-filter: blur`, transparent backgrounds)
- Interactive elements have subtle hover transforms and transitions
- Size comparison bars use percentage widths for visual scale
