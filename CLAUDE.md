# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Daven Insurance Agency — a static marketing website for an SMB commercial insurance agency serving NY, NJ, and FL. The entire site lives in a single `index.html` file with no build toolchain.

## Development

No build step required. Serve the file directly with any HTTP server, e.g.:

```bash
python -m http.server 8080
# or
npx serve .
```

## Architecture

**Single-file site**: All HTML, CSS, and JavaScript is in `index.html`. There are no external JS/CSS files, no npm dependencies, and no framework.

**CSS custom properties** define the color palette at the top of the `<style>` block:
- `--navy`, `--gold`, `--cream`, `--stone` are the core brand colors.

**JavaScript** (bottom of `<body>`) handles:
- Mobile hamburger menu toggle
- `handleSubmit()` form handler — currently shows an alert; needs wiring to a CRM (HubSpot/Pipedrive was noted as the intent)

**Cloudflare email obfuscation** script is included for the contact email link.

## Allowed WebFetch Domains

`.claude/settings.local.json` whitelists specific competitor/industry domains for research (Hub International, Alliant, USI, Risk Strategies, etc.). Do not remove these entries.
