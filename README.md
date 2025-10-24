# Vansh Ahuja — Interactive Portfolio

A single-file, responsive portfolio website showcasing projects, skills, and achievements with two presentation modes: a polished "Developer" view and an interactive "Designer" 3D scene.

Live preview: open [`index.html`](index.html).

## Key Features

- Responsive, single-page layout optimized for mobile and desktop.
- Dual-mode interface:
  - Developer Mode: clean, information-first UI built with Tailwind CSS.
  - Designer Mode: interactive 3D canvas powered by three.js.
- Sticky header with quick navigation and a mobile slide-out menu.
- Image marquees for personal intro photos and achievement visuals.
- Lightweight custom UI: search field, toggle switch, animated trophy list.
- Graceful fallbacks for missing images (uses placeholder images).

## Tech Stack

- HTML5, vanilla JavaScript
- Tailwind CSS (CDN)
- three.js (CDN) for the Designer mode 3D scene
- Font Awesome for icons

## Files & Assets

- Core file: [`index.html`](index.html)
- Assets:
  - `assets/intro/` — personal photos used in marquees ([assets/intro/](assets/intro/))
  - `assets/achievements/` — award images used in the achievements marquee ([assets/achievements/](assets/achievements/))

Project root:
```
index.html
README.md
assets/
  ├─ intro/
  └─ achievements/
```

## How to run locally

1. Clone or copy the repository to your machine.
2. Open the project folder and launch the site by opening [`index.html`](index.html) in your browser (double-click or use the editor's Live Preview).
3. Toggle the "Designer" mode in the header to enable the three.js 3D canvas.

No build step or server required — everything runs client-side.

## Notes for development

- The Designer mode uses three.js and appends a WebGL canvas to the fixed `#designer-canvas-container`.
- Toggle sync: `#mode-toggle` (desktop) and `#mobile-mode-toggle` (mobile) keep both modes synchronized.
- Marquee loops duplicate image sets for a seamless scroll; placeholders are used via `onerror` handlers.

## Suggested improvements

- Make the marquee animation pausable on hover for accessibility.
- Add keyboard navigation and ARIA roles for the mobile menu and toggles.
- Extract repeated CSS into a small stylesheet for maintainability.
- Add lazy-loading for images (`loading="lazy"`) to improve initial loading performance.

## Contact

- Email: ahujavansh076@gmail.com
- LinkedIn: https://www.linkedin.com/in/vansh-ahuja-8b5673259

---

Designed & built by Vansh Ahuja.
