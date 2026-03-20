# Napa Before The Nuptials — Site UI & Content

## What This Is

A static HTML bachelorette weekend site for Donna's August 6–9, 2026 trip to San Francisco and Napa Valley. The site is live at GitHub Pages and serves as the trip hub — itinerary, RSVP form, hotel info, wayfinding, and Outside Lands add-on details.

## Core Value

Guests land on one beautiful page that tells them everything they need to know, gets excited about the weekend, and collects all the info the organizer needs — no emails back and forth.

## Requirements

### Validated

- ✓ Site renamed to "Napa Before The Nuptials" — all occurrences updated
- ✓ Pink/tie-dye hero redesign — new color variables, layered gradients, animated blobs
- ✓ Itinerary copy updated across all 4 days (Arrival Day, Napa Valley, Reset & Celebrate, Departures)
- ✓ Friday winery order corrected (Winery #1 → Lunch Among the Vines → Winery #2)
- ✓ Sunday "Goodbye Brunch" + Outside Lands clickable link
- ✓ Lineup description updated ("Three days… with my favorite people")
- ✓ Form section heading changed to "A Few More Details"

### Active

- [ ] Remove phone number field from RSVP form
- [ ] Google Form Blueprint — copy-ready question set for organizer to build in Google Forms
- [ ] RSVP section HTML updated to match expanded form (question list, intro copy, iframe height)

### Out of Scope

- Custom form backend — Google Forms handles all data collection
- JavaScript-powered features — vanilla HTML/CSS only
- Major structural redesign — existing layout is working well

## Context

- **Live site**: `https://donz0723.github.io/napa-before-nuptials/`
- **Source**: `/Users/donz23/Napa before Nuptials/index.html` — single-file static HTML, no build system
- **Design system**: Cormorant Garamond + DM Sans, blush/pink/lavender/peach palette, editorial aesthetic
- **Deploy**: git push to `main` → GitHub Pages auto-deploys
- **Event**: August 6–9, 2026 · San Francisco (Westin St. Francis) + Napa Valley day trip (Friday)

## Constraints

- **Tech stack**: Vanilla HTML/CSS only — no JS frameworks, no build tools
- **Single file**: All styles and markup in `index.html`
- **Form backend**: Google Forms only

## Key Decisions

| Decision | Rationale | Outcome |
|----------|-----------|---------|
| GitHub Pages for hosting | Zero-config, free, deploys on push | ✓ Good |
| Pink/tie-dye theme | User requested softer, more feminine aesthetic | ✓ Good |
| Google Form embed | Easiest for organizer to manage responses in Google Sheets | — Pending |
| Remove phone number field | Reduces friction; email sufficient for coordination | — Pending |

---
*Last updated: 2026-03-19 after pivoting scope to UI & content*
