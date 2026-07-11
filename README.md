# nickconflitti.com

Personal one-page site — bio, contact, and selected work. Static HTML + CSS, no build step.

## Structure
- `index.html` — the entire page
- `styles.css` — all styling (responsive, light/dark aware)
- `CNAME` — custom domain for GitHub Pages (`nickconflitti.com`)

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
