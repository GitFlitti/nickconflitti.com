# nickconflitti.com

Personal one-page site — bio, contact, and selected work. Static HTML + CSS, no build step.

## Structure
- `index.html` — the entire page (incl. SEO meta + JSON-LD `Person` schema)
- `styles.css` — all styling (responsive, light/dark aware)
- `robots.txt` — crawler directives + sitemap reference
- `sitemap.xml` — single-URL sitemap for search engines
- `og-image.jpg` — 1200×630 social/link preview image (repo root)
- `assets/` — favicons, app icons, and `site.webmanifest`
- `CNAME` — custom domain for GitHub Pages (`nickconflitti.com`)

## SEO notes
- Title, meta description, canonical, Open Graph, and Twitter cards live in `<head>`.
- `Person` structured data (JSON-LD) ties the site to LinkedIn/GitHub via `sameAs`.
- The visually-hidden `<h1>` (`.sr-only`) provides the primary topic signal.
- **To do off-repo:** verify the site in
  [Google Search Console](https://search.google.com/search-console) + Bing
  Webmaster Tools, and submit `sitemap.xml`.

## Editing
Open `index.html` and replace the bracketed `[PLACEHOLDER]` text. Everything is
plain HTML — no framework, no compile step.

To preview locally, just open `index.html` in a browser, or run:

```sh
python3 -m http.server 8000   # then visit http://localhost:8000
```

## Deploying
Hosted on **GitHub Pages** from the `main` branch (root). Every push to `main`
publishes automatically. The `CNAME` file points the site at `nickconflitti.com`.
