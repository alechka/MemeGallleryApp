# MemeGallery — Landing Page

Marketing landing page for **MemeGallery**, a Windows desktop app for searching memes and images. Static HTML/CSS/JS, designed to be hosted on **GitHub Pages**.

## Files

| File | What it is |
|------|-----------|
| `index.html` | All page content (hero, features, screenshots, demo video, download). |
| `styles.css` | Fluent (Windows 11) light theme. |
| `script.js` | Small enhancements (sticky nav, scroll reveal, lightbox, year). |
| `assets/` | Site images — screenshots, favicon, social preview. |

## Things to fill in

1. **YouTube video** — in `index.html`, the demo `<iframe>` embeds video id `aCALSEO-vu0`;
   replace it with your own (the part after `watch?v=` in the YouTube URL).
2. **Download link** — the download buttons (ids `heroDownload` and `ctaDownload`) point at
   the Microsoft Store listing; update the `href` if your store URL changes.
3. **Screenshots** — the hero and "A closer look" section use the `shot-*.png` files in
   `assets/`; swap them for updated app screenshots as needed.
4. **Copy** — all marketing text is plain English in `index.html`; edit freely.

## Change the accent color

Open `styles.css` and edit the two variables at the top:

```css
--accent:   #0067c0;  /* main brand color  */
--accent-2: #0091ff;  /* lighter gradient tone */
```

## Preview locally

Just open `index.html` in a browser, or run a tiny server:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploy to GitHub Pages

1. Create a repo (e.g. `memegallery.site`) and push these files to the `main` branch.
2. On GitHub: **Settings -�� Pages**.
3. Under **Build and deployment -�� Source**, choose **Deploy from a branch**.
4. Pick branch **`main`** and folder **`/ (root)`**, then **Save**.
5. Your site goes live at `https://<username>.github.io/<repo>/` in a minute or two.

### Custom domain (optional)

If you own `memegallery.site`, add it under **Settings -�� Pages -�� Custom domain**.
GitHub will create a `CNAME` file for you. Then add these DNS records at your registrar:

```
A     @   185.199.108.153
A     @   185.199.109.153
A     @   185.199.110.153
A     @   185.199.111.153
CNAME www <username>.github.io
```
