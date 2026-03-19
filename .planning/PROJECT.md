# Napa Before Nuptials — RSVP Form Expansion

## What This Is

A static HTML bachelorette weekend site for Donna's August 6–9, 2026 trip to San Francisco and Napa Valley. The site is already designed and deployed — this work expands the RSVP section to collect comprehensive guest preference data so the organizer can plan every detail of the weekend: hotel rooms, activities, spa, and Napa logistics.

## Core Value

Guests submit one form that gives the organizer everything needed to plan the full weekend — no follow-up emails, no guesswork.

## Requirements

### Validated

(None yet — ship to validate)

### Active

- [ ] Update the RSVP section's left-side question preview list to reflect all new questions
- [ ] Provide a complete, copy-ready Google Form question set with all fields, options, and question types
- [ ] Include Saturday activity preference (yoga class / hike / spa treatments / city free time)
- [ ] Include spa interest gauge (yes / maybe / no)
- [ ] Include wine preference for Napa day (reds / whites / rosé / sparkling / non-drinker) — helps with winery selection
- [ ] Include a message to the bride field
- [ ] Include "anything to celebrate this weekend?" field (birthdays, milestones)
- [ ] Retain all existing fields: name, email, dietary restrictions, hotel room type, roommate preference, arrival time, Outside Lands interest, t-shirt size, open notes

### Out of Scope

- Custom backend / database — Google Forms handles all data collection
- Building the actual Google Form — user creates it in Google Forms; we provide the question blueprint
- Major redesign of the RSVP section layout — keep existing structure, expand the preview list

## Context

- **Existing site**: `/Users/donz23/Napa before Nuptials/index.html` — single-file static HTML, no build system
- **Design system**: Cormorant Garamond + DM Sans, ivory/gold/terra/sage palette, editorial aesthetic
- **RSVP mechanism**: Google Form iframe embed (src URL is a placeholder — user will paste real URL after building the form)
- **Event**: August 6–9, 2026 · San Francisco (Westin St. Francis) + Napa Valley day trip (Friday)
- **Saturday activities**: Yoga, hike, spa treatments, or city free time — guests pick preference
- **Organizer**: Donna (dlyakhov23@gmail.com)

## Constraints

- **Tech stack**: Vanilla HTML/CSS only — no JS frameworks, no build tools
- **Form backend**: Google Forms only — no Formspree, no custom backend
- **Scope**: Minimal — touch only the RSVP section HTML; preserve all design tokens and layout

## Key Decisions

| Decision | Rationale | Outcome |
|----------|-----------|---------|
| Keep Google Form embed | Easiest for organizer to manage responses in Google Sheets | — Pending |
| Include wine preferences | Napa winery selection depends on group's taste profile | — Pending |
| Include fun extras (bride message, celebrations) | Standard for bachelorette; adds warmth without complexity | — Pending |

---
*Last updated: 2026-03-19 after initialization*
