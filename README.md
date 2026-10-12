# Arpan Jargha Magar: Portfolio Website

A professional multi-page portfolio for **Arpan Jargha Magar**, founder and CEO of
[Jarghaa Furniture](https://www.facebook.com/jarghaa) (Lalitpur, Nepal).

Plain HTML + CSS, no build step. Deployed to GitHub Pages via
`.github/workflows/static.yml` on every push to `main`.

**Live site:** https://jarghaa.github.io/Jarghaa-portfolio/

## Pages

| Page | Purpose |
| --- | --- |
| `index.html` | Home — story, numbers, Jarghaa showcase, services, career, strengths, testimonials, notes teaser, investment band, contact form |
| `invest.html` | Investors & partners — opportunity, what I'm looking for, traction, meeting request |
| `notes/index.html` | Notes hub — list of essays |
| `notes/why-handmade.html` | First essay: "Why I chose handmade furniture over mass production" |
| `404.html` | Friendly not-found page |

## Project structure

```
Jarghaa-portfolio/
├── index.html            # home page (content + JSON-LD Person schema)
├── invest.html           # investor / partner page
├── notes/
│   ├── index.html        # notes hub
│   └── why-handmade.html # first essay (JSON-LD Article schema)
├── 404.html              # not-found page
├── assets/
│   ├── theme.css         # all styles (light + dark themes)
│   └── images/           # put photos here (pieces, headshot, og-cover)
├── robots.txt            # search-engine crawl rules
├── sitemap.xml           # sitemap for search engines
└── README.md
```

## SEO & sharing built in

- Per-page `<title>`, meta description, canonical URL.
- Open Graph + Twitter card tags for rich link previews.
- JSON-LD structured data (`Person` on home, `Article` on the essay).
- `sitemap.xml` and `robots.txt`.
- Inline SVG favicon and `theme-color`.

## Before you publish — fill these in

Search the code for `TODO` (comments) and the visible placeholders:

- [ ] **Photos.** Drop gallery images into `assets/images/` and add an
      `og-cover.jpg` for link previews. Update the `alt` text in `index.html`.
      (The headshot is already set: `assets/headshot.jpg`.)
- [ ] **Stats.** Replace the figures in the "By the numbers" section on
      `index.html` and the "Traction & financials" section on `invest.html`.
- [ ] **Testimonials.** Replace the placeholder quotes on `index.html` with
      real, attributable quotes (ask permission first).
- [x] **Email.** Set to `jarghaa3314@gmail.com` on the home and investor pages.
- [x] **WhatsApp.** Set to `+977 9818654453` (`https://wa.me/9779818654453`)
      on the home and investor pages. Consider WhatsApp Business for a
      catalogue and auto-replies.
- [x] **Headshot.** Added as `assets/headshot.jpg` and shown in the hero
      (the dovetail graphic is the fallback).
- [ ] **Contact forms.** Create a free form endpoint at
      [Formspree](https://formspree.io) or use Netlify Forms, then set the
      `<form action="...">` value on both forms (currently `REPLACE_ME`).
- [ ] **Pitch deck.** Upload your deck to `assets/jarghaa-pitch.pdf` (linked
      from `invest.html`).
- [ ] **URLs.** If you use a custom domain, update the `canonical`, Open Graph
      `og:url`, `sitemap.xml`, `robots.txt`, and the absolute paths in
      `404.html` (currently the GitHub Pages URL).

## Publish with GitHub Pages

Pages is already enabled for this repo (Source: **GitHub Actions**). Any push
to `main` triggers the workflow in `.github/workflows/static.yml` and deploys
the whole repository.

1. Merge your changes into `main`.
2. Watch the run under the repo's **Actions** tab.
3. The site goes live at https://jarghaa.github.io/Jarghaa-portfolio/.

### Custom domain (recommended: `arpanmagar.com`)

1. Add a `CNAME` file containing just your domain (e.g. `arpanmagar.com`).
2. In **Settings → Pages → Custom domain**, enter the same domain.
3. Point DNS (A records to GitHub Pages IPs, or a CNAME for `www`) as GitHub
   instructs. HTTPS is issued automatically.

## Edit the site

- Content lives in the HTML files; styles live in `assets/theme.css`.
- Preview locally:
  ```bash
  python3 -m http.server
  # then open http://localhost:8000
  ```

## Roadmap (next phases)

- Publish a new note each month for thought leadership and SEO.
- Keep LinkedIn updated to mirror the site.
- Pitch the founder story to Nepali business media for PR.
- Register Jarghaa on Crunchbase/F6S for investor discovery.
- Add a newsletter (Mailchimp) for investor updates.
- Optional: a Nepali-language toggle.

