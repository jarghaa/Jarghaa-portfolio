# Arpan Jargha Magar: Portfolio Website

A professional multi-page portfolio for **Arpan Jargha Magar**, founder and CEO of
[Jarghaa Furniture](https://www.facebook.com/jarghaa) (Lalitpur, Nepal).

Plain HTML + CSS, no build step. Deployed to GitHub Pages via
`.github/workflows/static.yml` on every push to `main`.

**Live site:** https://jarghaa.github.io/Jarghaa-portfolio/

## Design

- **Palette:** Navy Blue · Crisp White · Gold hardware (with a deep-navy dark mode).
- **Type:** Young Serif for headings, Instrument Sans for body.
- **Motif:** a dovetail-joint brand mark, used small and centred in the footer.

## Pages

| Page | Purpose |
| --- | --- |
| `index.html` | Home — story, numbers, Jarghaa showcase, services, career, strengths, testimonials, Liverpool section, notes, investment band, contact |
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
│   ├── theme.css         # all styles (navy/white/gold, light + dark)
│   └── images/
│       └── headshot.jpg  # portrait used in the hero and link previews
├── robots.txt            # search-engine crawl rules
├── sitemap.xml           # sitemap for search engines
└── README.md
```

## Email privacy (spam protection)

The email address is **not** written anywhere in the HTML. It is split into
character codes in a small script and rebuilt in the browser, so:

- **People can still email you** — the "Email me" button and the contact form
  both open the visitor's mail app with the message ready to send.
- **Harvesting bots can't read it** — scrapers that only read HTML (no
  JavaScript) never see the address.

This replaced the earlier Formspree form, so no third-party signup is needed.

## SEO & sharing built in

- Per-page `<title>`, meta description, canonical URL.
- Open Graph + Twitter card tags (share image = your headshot).
- JSON-LD structured data (`Person` on home, `Article` on the essay).
- `sitemap.xml` and `robots.txt`.
- Inline SVG favicon and `theme-color`.

## Before you publish — remaining placeholders

Search the code for `TODO` (comments) and the visible placeholders:

- [ ] **Photos.** Drop gallery images into `assets/images/` and add an
      `og-cover.jpg` (1200×630) for even better link previews. Update the `alt`
      text in `index.html`.
- [ ] **Stats.** Figures (180+ pieces, 130+ clients) are plausible placeholders —
      replace with your real numbers on `index.html` and `invest.html`.
- [ ] **Testimonials.** Three quotes are drafted with placeholder Nepali names
      (Prarambha Shakya, Nischal Tuladhar, Dikshya Amatya) — swap in real,
      attributable quotes with permission before publishing.
- [ ] **Pitch deck.** Upload your deck to `assets/jarghaa-pitch.pdf` (linked
      from `invest.html`).
- [ ] **URLs.** If you use a custom domain, update the `canonical`, Open Graph
      `og:url`, `sitemap.xml`, `robots.txt`, and the absolute paths in
      `404.html` (currently the GitHub Pages URL).

Done already:

- [x] **Headshot** — `assets/images/headshot.jpg` in the hero and link previews.
- [x] **WhatsApp** — `https://wa.me/9779818654453` on home + investor pages.
- [x] **Email** — hidden from scrapers, usable via button and form.
- [x] **Theme** — navy / white / gold.

## Publish with GitHub Pages

Pages is already enabled for this repo (Source: **GitHub Actions**). Any push
to `main` triggers the workflow in `.github/workflows/static.yml` and deploys
the whole repository.

1. Merge your changes into `main`.
2. Watch the run under the repo's **Actions** tab.
3. The site goes live at https://jarghaa.github.io/Jarghaa-portfolio/.

### Custom domain (recommended)

1. Add a `CNAME` file containing just your domain (e.g. `arpanmagar.com`).
2. In **Settings → Pages → Custom domain**, enter the same domain.
3. Point DNS (A records to GitHub Pages IPs, or a CNAME for `www`) as GitHub
   instructs. HTTPS is issued automatically.

## Edit the site

- Content lives in the HTML files; styles live in `assets/theme.css`.
- Colours are CSS variables at the top of `theme.css` — change them in one
  place to re-skin the whole site.
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

