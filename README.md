# shaghaghidev.github.io

This is my portfolio: **[https://shaghaghidev.github.io](https://shaghaghidev.github.io)**

I'm Abolfazl Shaghaghi — a Computer Engineering student focused on **Web
Design & Development**. This site is where that's actually shown: who I
am, what I'm currently building with (WordPress, Figma, HTML, CSS), a
couple of real projects, and how to reach me.

Earlier versions of this repo pulled everything live from the GitHub
API — stats, repo lists, contribution graphs. I pulled all of that back
out. It made the site feel like a GitHub dashboard instead of a personal
portfolio, and it wasn't telling the story I actually wanted to tell. This
version is plain, static, and hand-curated on purpose.

## What's in here

```
index.html              the entire site — every section's content lives directly in here
assets/css/style.css    one stylesheet, no framework
assets/js/app.js        theme toggle, mobile nav, scroll-reveal — that's it, no API calls
assets/images/          real project covers + the Coming Soon teaser for Web Design Showcase
sitemap.xml, robots.txt SEO basics
```

No build step, no framework, no npm install, no bundler, no ES modules.
Open `index.html`, read it top to bottom, and you've seen the whole site.

## Page structure

| Section              | What it is                                                                 |
| --------------------- | --------------------------------------------------------------------------- |
| Hero                  | Name, role, real photo, current focus / next focus                        |
| About                 | Short bio + "Currently Working With" / "Learning Next" + how I use AI-assisted / vibe coding in my workflow |
| Web Design Showcase   | My primary portfolio area — real WordPress/Figma work goes here as I ship it. Currently 3 honest "coming soon" placeholders, not fake projects |
| Vibe Coding Projects  | Supporting proof of previous work (Telegram bots, a C++ course project) — built with AI-assisted development, labeled honestly (`Concept · Direction · AI-Assisted Development` where that's actually true) |
| My Journey            | Four honest stages: Now / Next / Then / Later — "Later" is direction, not current skill |
| Contact               | Email, GitHub, Telegram, Instagram — direct links, no form, no backend |

## Editing content

Everything is hand-written straight into `index.html` — there's no
separate config file to hunt through:

- **Bio / focus** → the `#about` section
- **Projects in Web Design Showcase** → the `#design` section. Replace a
  placeholder `<figure class="showcase-card">` with a real project: swap
  the image in `assets/images/`, update the `figcaption` name/meta, and
  add a real link once there's a live site to point to
- **Vibe Coding Projects** → the `#work` section, one `<article
  class="work-card">` per project. Pinned/shown order is just the order
  they appear in the file
- **Journey stages** → the `<ol class="path">` list in `#journey`
- **Contact links** → the `.contact-row` links in `#contact`

Nothing here is fetched or generated — if it's out of date, it's because
I haven't edited the file yet, not because an API call failed.

## Deploying

Already live at `shaghaghidev/shaghaghidev.github.io`, set to deploy from
`main` / root under Settings → Pages.

```
git add .
git commit -m "update: whatever I changed"
git push
```

GitHub Pages picks it up in a minute or two.

## Running it locally

Just open `index.html` in a browser — no server needed. There are no ES
modules and no API calls, so `file://` works fine.

## If I get a custom domain later

Update these (all currently `https://shaghaghidev.github.io`):

- `index.html` → canonical link, `og:url`, `og:image`, `twitter:image`,
  and the Schema.org `url`/`image` in the JSON-LD block
- `sitemap.xml` → `<loc>`
- `robots.txt` → `Sitemap:`
- Add a `CNAME` file at the repo root
