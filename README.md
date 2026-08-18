# pautarragona.github.io/homepage

Personal site. Plain HTML + CSS, no build step, no dependencies.

Live at **https://pautarragona.github.io/homepage/**

## Editing

| File | What's in it |
|---|---|
| `index.html` | All the content. Search for `TODO` — that's everything to fill in. |
| `style.css` | Colours live in `:root` at the top. Change `--accent` to re-skin the site. |
| `sitemap.xml` | Update `<lastmod>` when you make a meaningful change. |
| `404.html` | Shown for bad URLs. |
| `.nojekyll` | Tells GitHub Pages to serve files as-is. |

To preview locally, open `index.html` in a browser, or run:

```
python -m http.server 8000
```

and visit http://localhost:8000

## Publishing

Every push to `main` redeploys automatically (takes ~1 minute).

```
git add -A
git commit -m "Update"
git push
```

## Notes

- `index.html` references `preview.png` (link-preview image, 1200×630) and
  `cv.pdf`. Drop those files in this folder, or remove the references.
- Because this is a project repo rather than `pautarragona.github.io`, the site
  lives under a `/homepage/` path and a root `robots.txt` isn't possible.
  Submit `sitemap.xml` directly in Google Search Console instead.
