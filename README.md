# shaghaghi-portfolio

This repository contains my personal portfolio source code.

**Production:** https://shaghaghidev.ir  
**GitHub:** https://github.com/shaghaghidev

I'm **Abolfazl Shaghaghi**, a Computer Engineering student focused on **Web Design & Development**. My current focus is WordPress, Figma, HTML and CSS, followed by JavaScript, PHP and deeper WordPress development.

## What this repository contains

- `index.html` — complete portfolio markup and content
- `assets/css/style.css` — site styles
- `assets/js/app.js` — theme toggle, mobile navigation and small UI interactions
- `assets/images/` — profile, project covers and showcase placeholders
- `assets/icons/` — favicon and social preview assets
- `robots.txt` / `sitemap.xml` — SEO basics

The site is intentionally **static and hand-curated**. It does not use a GitHub API dashboard or dynamically generate portfolio content from repositories.

## Portfolio structure

- **Hero** — name, role, photo and current/next focus
- **About** — current learning direction and AI-assisted / vibe coding workflow
- **Web Design Showcase** — reserved for real WordPress/Figma work; no fake projects
- **Vibe Coding Projects** — selected previous work, labeled honestly
- **My Journey** — Now / Next / Then / Later
- **Contact** — Email, GitHub, Telegram and Instagram

## Source vs. production

GitHub is the **source code and version history** for the portfolio.

The production website is hosted separately on cPanel at **https://shaghaghidev.ir**.

GitHub Pages is not the production host and should remain disabled once the custom-domain deployment is confirmed.

## Editing

Most content lives directly in `index.html`.

- Update the About section for bio/focus changes.
- Replace showcase placeholders only when real web projects are available.
- Add/update selected projects in the Work section.
- Update Journey stages as the learning path changes.
- Update contact links when needed.

No fake clients, certificates, testimonials, ratings or professional claims should be added.

## Local use

No build step or package installation is required. Open `index.html` directly in a browser or serve the folder with any simple local HTTP server.

## Deployment

Production deployment is handled separately through cPanel.

For source changes:

```bash
git add .
git commit -m "update: describe the change"
git push
```

Keep the repository even though GitHub Pages is not used for production.
