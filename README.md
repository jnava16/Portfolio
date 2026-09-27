# Joshua Nava — Portfolio

A clean, editorial-style portfolio built with plain HTML, CSS, and JavaScript — no build step, no frameworks.

## Structure

```
portfolio/
├── index.html          Page structure and content
├── css/
│   └── style.css        All styling, using CSS custom properties for the design system
├── js/
│   └── script.js         Mobile nav toggle only — everything else is plain CSS
├── images/
│   ├── joshua-photo.jpg   Hero portrait
│   ├── case-nia.jpg       National Irrigation Administration screenshot
│   ├── case-tpb.jpg       Tourism Promotions Board Philippines screenshot
│   └── case-rtf.jpg       Regional Travel Fair screenshot
└── README.md
```

## Running it locally

No build tools needed. Either:
- Double-click `index.html` to open it directly in a browser, or
- Serve the folder locally, e.g. `python3 -m http.server` from inside `portfolio/`, then visit `http://localhost:8000`.

## Editing content

All page copy lives directly in `index.html` — no CMS or template engine. To update a case study, edit the relevant `<article class="case">` block. To add a new one, copy an existing `<article class="case">...</article>` block, update its image, role, overview, responsibilities list, outcome, and link, and add a new image to `images/`.

## Design system

Colors, fonts, spacing, and border-radius are defined once as CSS custom properties at the top of `css/style.css` (under `:root`). Change a value there to update it site-wide — for example, `--accent` controls the single accent color used for links, tags, and buttons throughout.

## Notes on content accuracy

Every project, skill, service, and credential listed reflects what was provided in your resume and Canva portfolio. Nothing has been invented — no fabricated testimonials, stats, or client names. If you add new projects or claims later, keep the same principle: specific, verifiable detail over generic claims.

## Deploying

This is a static site — it can be hosted as-is on GitHub Pages, Netlify, Vercel, or any standard web host. Just upload the whole `portfolio/` folder (or its contents) to your host of choice.
