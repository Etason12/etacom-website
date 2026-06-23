# Etacom Technology Website

Modern corporate website for Etacom Technology — a software, AI, data, and ICT solutions company based in Mekelle, Ethiopia.

## Tech Stack

- [Astro](https://astro.build) — Static site generator
- Vanilla CSS — Custom properties, responsive design
- Vanilla JavaScript — No frameworks, no dependencies

## Project Structure

```text
etacom-website/
├── public/
│   ├── styles.css          # All styles (nav, cards, responsive)
│   ├── script.js           # Nav, dropdown, form, counters
│   └── services.js         # Service detail data (9 services)
├── src/
│   ├── layouts/
│   │   └── Layout.astro    # Shared head, fonts, scripts
│   ├── components/
│   │   ├── Header.astro    # Nav bar, hamburger, dropdown
│   │   └── Footer.astro    # Footer with links, contact
│   └── pages/
│       ├── index.astro     # Homepage
│       └── service.astro   # Dynamic service detail page
└── package.json
```

## Commands

| Command | Action |
|:---|:---|
| `npm install` | Install dependencies |
| `npm run dev` | Start dev server at `localhost:4321` |
| `npm run build` | Build to `./dist/` |
| `npm run preview` | Preview production build |

## Features

- Mobile-first responsive design
- Animated hamburger menu with slide-down dropdown
- 9 service detail pages via `?slug=` parameter
- Contact form with Formspree integration
- Animated stat counters on scroll
- Sticky header with scroll effect

## Deployment (Netlify)

1. Push to GitHub
2. Connect repo to Netlify
3. Build command: `npm run build`
4. Publish directory: `dist/`

## Contact Form Setup

Replace the placeholder in `src/pages/index.astro`:

```
action="https://formspree.io/f/YOUR_FORM_ID_HERE"
```

Get your form ID at [formspree.io](https://formspree.io).

## License

Private — Etacom Technology
