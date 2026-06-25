# Artizen — Art Studio Website

A warm, mobile‑first website for **Artizen**, a cozy art studio in Amman, Jordan offering canvas, pottery, fabric and clay sessions, music lessons, and private events.

## What's here

| File | Description |
|------|-------------|
| `Artizen-Website-Standalone.html` | **The main site** — a single self‑contained page (hero, "pick your craft" paint‑journey section, weekly session calendar with reservations, occasions, about, FAQ, footer, and a booking modal). |
| `paint-journey.html` | Standalone version of the scroll‑driven "paint journey" section (a paintbrush draws a winding line that threads past the craft photos). |
| `assets/` | Fonts (`Alta`, `Feeling Passionate`) and images used across the site. |
| `ref/` | Reference images and source SVGs (e.g. the paintbrush icon). |
| `index.html`, `category-test*.html`, `collage.html`, `animated-cards.html` | Earlier explorations / prototypes kept for reference. |

## The paint‑journey section

The signature element: a winding light‑yellow line runs down the page in a regular zigzag (photos step right → centre → left → centre). A green‑handled **paintbrush** rides the leading tip of the line and rotates to follow it, smoothly easing as you scroll — so it looks like the brush is drawing the line. Short hand‑lettered notes ("made by hand", "find your rhythm", "celebrate the moment") sit along the line between sections. Fully responsive, with a tuned mobile layout.

## Tech

- Plain **HTML + CSS**, no build step.
- The main site renders with **React 18 + Babel Standalone** loaded from CDN (so it must be opened with an internet connection).
- Fonts: **Alta** (local), **Feeling Passionate** (local script), **Caveat** (Google Fonts).
- The brand palette (terracotta, olive‑green, rust, mauve‑brown, cream, dark‑brown) is defined as CSS variables.

## Brand / copy rules

- **English only**, no Arabic.
- **No emoji** in copy — decorative icons are SVG vectors.
- **No `&`** in visible text (use "and").
- **No em dash (—)** — use commas, colons, or periods.
- The script font (`Feeling Passionate`) never renders **numbers or commas** (they fall back to a plain font).

## Running it

Open `Artizen-Website-Standalone.html` in a browser (needs internet for the CDN fonts/scripts). No server or build required.
