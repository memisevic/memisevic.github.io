# Personal website — Roland Memisevic

Static site (plain HTML + CSS, no build step).

## Files

- `index.html`, `style.css` — the site itself
- `assets/portrait.jpg`, `assets/cv.pdf` — hero image and CV linked from the site
- `cv/` — LaTeX source for the CV; run `make` in this directory to rebuild `cv.pdf`, then copy it to `assets/cv.pdf`

## Local preview

Any of the following works:

```
python3 -m http.server 8000
# then open http://localhost:8000
```

Or just open `index.html` directly in a browser.

## Deploy (GitHub Pages)

The repo is set up to be served as-is:

1. Push to a repo named `<your-github-username>.github.io`
2. Repo Settings → Pages → source: `main` branch, root folder
3. Live at `https://<your-github-username>.github.io/`
