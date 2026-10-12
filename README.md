# Arpan Magar: Portfolio Website

A single-page professional portfolio for **Arpan Magar**, founder and CEO of
[Jarghaa Furniture](https://www.facebook.com/jarghaa) (Lalitpur, Nepal).

Plain HTML + CSS, no build step. Deployed to GitHub Pages via the workflow in
`.github/workflows/static.yml`.

## Project structure

```
Jarghaa-portfolio/
├── index.html            # the whole page (content + structured data)
├── assets/
│   ├── theme.css         # all styles (light + dark themes)
│   └── images/           # put photos here (pieces, headshot, og-cover)
├── robots.txt            # search-engine crawl rules
├── sitemap.xml           # sitemap for search engines
└── README.md
```

## What's on the page

1. **Hero** — name, positioning line, and two calls to action.
2. **About / Story** — the narrative arc: IT → property → craft.
3. **By the numbers** — credibility stats.
4. **Jarghaa Furniture** — the workshop, a photo gallery, and CTAs.
5. **What I can help with** — furniture, property/operations, advisory.
6. **Career** — the full timeline.
7. **Strengths** — skills.
8. **In their words** — testimonials.
9. **Let's build something bigger** — partnership/investment band.
10. **Contact** — email, social links, and a contact form.

## Before you publish — fill these in

Search the file for `TODO` (comments) and the visible placeholders:

- [ ] **Photos.** Drop real images into `assets/images/` (gallery pieces,
      an `og-cover.jpg` for link previews, and a headshot). Update the `alt`
      text in `index.html`.
- [ ] **Stats.** Replace the figures in the "By the numbers" section with your
      verified numbers.
- [ ] **Testimonials.** Replace the placeholder quotes with real, attributable
      quotes (ask permission first).
- [ ] **Email.** Change `hello@arpanmagar.com` in the contact section to your
      real address. Add a WhatsApp/phone link if you want enquiries there.
- [ ] **Contact form.** Create a free form endpoint at
      [Formspree](https://formspree.io) or use Netlify Forms, then set the
      `<form action="...">` value (currently `REPLACE_ME`).
- [ ] **URLs.** If you use a custom domain, update the `canonical`, Open Graph
      `og:url`, `sitemap.xml`, and `robots.txt` URLs (currently the GitHub
      Pages URL `https://jarghaa.github.io/Jarghaa-portfolio/`).

## Publish with GitHub Pages

The repo already includes a Pages workflow that deploys on every push to
`main`:

1. Push `main` to GitHub.
2. Repo **Settings → Pages → Build and deployment → Source: GitHub Actions**.
3. The site goes live at `https://jarghaa.github.io/Jarghaa-portfolio/`.

### Custom domain (recommended: `arpanmagar.com`)

1. Add a `CNAME` file containing just your domain (e.g. `arpanmagar.com`).
2. In **Settings → Pages → Custom domain**, enter the same domain.
3. Point DNS (A records to GitHub Pages IPs, or a CNAME for `www`) as GitHub
   instructs. HTTPS is issued automatically.

## Edit the site

- Text lives in `index.html`; styles live in `assets/theme.css`.
- Preview locally:
  ```bash
  python3 -m http.server
  # then open http://localhost:8000
  ```

## Roadmap (next phases)

- Publish 1–2 blog posts / notes for thought leadership and SEO.
- Keep LinkedIn updated to mirror the site.
- Pitch the founder story to Nepali business media for PR.
- Register Jarghaa on Crunchbase/F6S for investor discovery.
- Add a newsletter (Mailchimp) for investor updates.
- Optional: a Nepali-language toggle.
