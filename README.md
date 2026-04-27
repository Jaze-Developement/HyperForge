# HyperForge

Evidence-based hypertrophy training — an educational resource on how to build muscle using research-backed principles rather than social media trends.

**GitHub repo:** https://github.com/Jaze-Developement/HyperForge
**Live site:** https://jaze-developement.github.io/HyperForge/

## About

HyperForge is a five-page static website built as a project for CIS 300 (Web Design and Development) at ASU. The goal is to cut through fitness misinformation by distilling resistance-training research into clear, practical guidance.

## Pages

- **Home** (`index.html`) — Landing page with site overview, hero illustration, and feature cards
- **Training Principles** (`principles.html`) — Three drivers of hypertrophy, progressive overload, MV/MEV/MAV/MRV volume landmarks (with bar chart and dose-response curve diagrams)
- **Exercise Selection** (`exercises.html`) — Compound vs isolation, comparison table of training variables across experience levels, six-panel movement patterns infographic, sample movement menu
- **Programming** (`programming.html`) — Training splits, mesocycle design, deload timing, with embedded compound lift demonstration video, weekly split visualization, and mesocycle progression chart
- **Contact** (`contact.html`) — Four-field consultation request form, paper-plane illustration, direct email link, external link to Stronger By Science

## Tech

- Plain HTML5 and CSS3 — no frameworks
- CSS custom properties (`:root` variables) for the color palette and font stack, exported from realtimecolors.com
- 67 CSS selectors, 271 declared properties, 529 lines (`styles.css`)
- CSS Grid for feature-card layout, Flexbox for the nav and form
- Semantic HTML5 tags throughout: `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>`
- Native HTML5 `<video>` tag with controls, poster image, and fallback
- All diagrams generated in matplotlib using the same color hex codes as `styles.css` for visual consistency
- Mobile responsive via single `@media (max-width: 768px)` breakpoint

## Lighthouse audit (desktop preset, run on the home page)

- Performance: 100
- Accessibility: 92
- Best Practices: 96
- SEO: 100

## Folder structure

```
hyperforge/
├── index.html
├── principles.html
├── exercises.html
├── programming.html
├── contact.html
├── styles.css
├── images/
│   ├── hero-barbell.svg          (Home page)
│   ├── three-drivers.png         (Training Principles)
│   ├── volume-landmarks.png      (Training Principles)
│   ├── movement-patterns.png     (Exercise Selection)
│   ├── weekly-split.png          (Programming)
│   ├── mesocycle.png             (Programming)
│   ├── video-poster.jpg          (Programming — video poster)
│   └── contact-illustration.svg  (Contact)
├── videos/
│   └── lift-demo.mp4             (Programming — embedded video)
└── README.md
```

## Running locally

No build step. Just open `index.html` in a browser, or run a simple local server:

```sh
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Author

Joett Ocasio — CIS 300, Spring 2026
