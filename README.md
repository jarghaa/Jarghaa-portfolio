# Arpan Magar: Portfolio Website

A single-page portfolio for Arpan Magar, founder of Jarghaa Furniture (Lalitpur, Nepal).
Plain HTML and CSS with no build step, so it works on any static host.

## Project structure

```
arpan-magar-portfolio/
├── index.html          # the whole site (HTML + CSS)
├── assets/images/      # put furniture photos here
├── .nojekyll           # tells GitHub Pages to serve files as-is
├── .gitignore
└── README.md
```

## Publish it live with GitHub Pages

1. Create a new repository on GitHub, for example `arpan-magar-portfolio`. Keep it empty (no README).
2. In a terminal, from inside this folder, run:
   ```bash
   git init
   git add .
   git commit -m "Initial portfolio site"
   git branch -M main
   git remote add origin https://github.com/YOUR-USERNAME/arpan-magar-portfolio.git
   git push -u origin main
   ```
3. On GitHub, open the repository, then **Settings → Pages**.
4. Under **Build and deployment**, set **Source** to **Deploy from a branch**, choose **main** and **/ (root)**, then **Save**.
5. After a minute or two, the site is live at `https://YOUR-USERNAME.github.io/arpan-magar-portfolio/`.

**Tip:** name the repository `YOUR-USERNAME.github.io` to get the shorter address `https://YOUR-USERNAME.github.io/`.

## Edit the site

- Open `index.html` and change the text directly. Roles and dates are in the `Career` section.
- To add photos, put them in `assets/images/` and reference them with `<img src="assets/images/your-photo.jpg" alt="Describe the piece">`.
- Preview locally by double-clicking `index.html`, or run `python3 -m http.server` in this folder and open http://localhost:8000.

## Custom domain (optional)

Add a file named `CNAME` containing your domain (for example `arpanmagar.com`), then set the same domain under **Settings → Pages** and point your DNS to GitHub Pages.
