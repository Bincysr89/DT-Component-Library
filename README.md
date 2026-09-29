# DT Component Library

Typography, design tokens and UI component reference for the Dubai Trade platform.

Built as a Figma Make project (React + Vite). The component reference itself is a
single static page under `public/` — it has no build step and can be opened directly.

## Contents

| Path | What it is |
| --- | --- |
| `public/dt-component-directory.html` | The component library page (also served as `index.html`) |
| `public/assets/`, `public/lpi-images/` | Icons and screenshots used by the page |
| `public/dubai-font.zip` | Dubai typeface (Bold / Medium / Regular / Light) |
| `src/` | Figma Make React scaffold |
| `src/imports/` | Source material the page was built from |

## What the page covers

Dubai font and icon set; typography scale (H1–H3, body, button/tag text); colour and
elevation tokens; the Dirham symbol; form controls (checkbox, radio, toggle, phone,
date/time, dropdown, search, uploader); and larger patterns — data tables, pagination,
stepper, tabs, side panel, dialogs, notifications, charts, card/list views and the
listing-page interaction spec.

## Viewing it

Open `public/dt-component-directory.html` in a browser, or serve the folder:

```bash
python3 -m http.server 4211 --directory public
```

## Development

```bash
npm install
npm run dev
```

## Notes

- The page falls back to Arial when the Dubai font is not installed. Add `@font-face`
  declarations pointing at your hosted font files before using these styles in production.
- "View in Figma" links point at the DT Component Library Figma file and need access to it.
