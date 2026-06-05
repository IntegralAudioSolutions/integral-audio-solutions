# Integral Audio Solutions Ltd — Business Website

Professional business website for Integral Audio Solutions Ltd, hosted on GitHub Pages.

## Tech Stack

Plain HTML, CSS, and vanilla JavaScript — no frameworks, no build tools.
Designed to be clean, fast, and easy to iterate on.

## Structure

```
integral-audio-solutions/
├── index.html              ← Landing page
├── README.md
├── pages/
│   ├── services.html       ← Services overview
│   ├── projects.html       ← Published credits
│   ├── about.html          ← Company background
│   └── contact.html        ← Business enquiry form
└── assets/
    └── images/             ← Key art and logo assets
```

## Pages

| Page | Description |
|------|-------------|
| `index.html` | Hero logo, credits grid, about summary, services snapshot, CTA |
| `pages/services.html` | Seven service cards with descriptions, how-we-work process strip |
| `pages/projects.html` | All 14 published credits with filterable grid |
| `pages/about.html` | Company overview, Epic Games feature, ethos, client list |
| `pages/contact.html` | Business enquiry form with thank you state |

## Logo

The animated oscilloscope logo is rendered via HTML Canvas with a JavaScript animation loop. It animates for 5 seconds, then a laser traces the waveform left to right and freezes on a target frame. Parameters are in the `<script>` block at the bottom of `index.html`.

Key constants:
- `FREQ` — wave frequency (1.25 = slightly more than half a cycle visible)
- `TARGET_T_MOD` — phase value at which the wave freezes (PI * 0.75)
- `FREEZE_AFTER` — milliseconds before freeze is allowed (5000)
- `LEFT_F / RIGHT_F` — horizontal extent of wave as fraction of canvas width (0.24 / 0.73)

## Deploying to GitHub Pages

1. Push to the `main` branch
2. Go to **Settings → Pages**
3. Set source to `main` branch, root folder
4. Site goes live at `https://yourusername.github.io/integral-audio-solutions`

## Assets

All key art images live in `assets/images/`. Filenames follow the pattern `[title-slug]-keyart.png`.

For the best result on the projects page, replace the current cropped versions with the original high-resolution source images — the projects grid displays them at 340×180px so anything 680px wide or above will look sharp.

## Colour Palette

| Token | Value | Usage |
|-------|-------|-------|
| `--bg` | `#0a0e14` | Page background |
| `--surface` | `#111827` | Card / section surface |
| `--surface-2` | `#1a2332` | Hover state surface |
| `--cyan` | `#00d4ff` | Primary accent |
| `--violet` | `#7c3aed` | Secondary accent |
| `--text` | `#e2e8f0` | Body text |
| `--muted` | `#64748b` | Secondary text |

## Typography

Orbitron (Google Fonts) for all headings and UI text. Falls back to `'Courier New', monospace`.
Font import is included in the `<head>` of every page.

---

Integral Audio Solutions Ltd · Registered in England & Wales · Est. 2023
