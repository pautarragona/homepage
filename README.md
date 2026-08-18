# pautarragona.github.io/homepage

Personal site. Plain HTML + CSS + ~30 lines of JS. No build step, no dependencies,
no trackers.

Live at **https://pautarragona.github.io/homepage/**

## Editing

| File | What's in it |
|---|---|
| `index.html` | All the content. Also the SEO tags and the JSON-LD `Person` block. |
| `style.css` | Design tokens are in `:root` at the top — change `--accent` to re-skin the whole site. |
| `sitemap.xml` | Bump `<lastmod>` when you make a meaningful change. |
| `404.html` | Shown for bad URLs. |
| `.nojekyll` | Tells GitHub Pages to serve the files as-is. |

Preview locally with:

```
python -m http.server 8000
```

then open http://localhost:8000

## Still to do

- [ ] Replace `TODO-your-handle` with the real LinkedIn handle (2 places: the
      JSON-LD block in `<head>`, and the contact list).
- [ ] Replace the highlighted `[your subsystem]` in the BSc Thesis entry.
- [ ] Add `cv.pdf` to the repo root, then uncomment the Download CV button in the
      About section.
- [ ] Optional: add a 1200×630 `preview.png` and uncomment the `og:image` tags for
      rich link previews on LinkedIn/WhatsApp/Slack.

## Publishing

Every push to `main` redeploys automatically, roughly a minute later.

```
git add -A
git commit -m "Update"
git push
```

## Notes

Because this is a project repo rather than `pautarragona.github.io`, the site lives
under a `/homepage/` path and a root `robots.txt` isn't possible. Submit
`sitemap.xml` directly in Google Search Console instead.
