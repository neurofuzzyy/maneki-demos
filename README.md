# maneki-demos

Speculative website demos for Maneki Studio outreach. Deployed automatically by Cloudflare Pages on every push to `main`.

## Structure

Each prospect gets one folder at the repo root. The folder name is the URL path.

```
senn-landscaping/      -> /senn-landscaping/
  index.html
  img/
```

The root `index.html` redirects to maneki.studio so prospects can't browse each other's demos.

## Rules for every demo

- Self-contained static files: `index.html` plus local assets. No build step.
- Relative asset paths (`img/photo.jpg`), so the folder works at any path.
- `noindex` meta tag on the page. `_headers` and `robots.txt` at the root also block indexing site-wide.
- Footer credit: `Speculative redesign concept by Maneki Studio · Not affiliated with [Business]`
- Open Graph image and URL point at the demo's own path, so text and email link previews show the hero photo.

## Cloudflare Pages settings

Framework preset: None · Build command: (empty) · Output directory: (empty, repo root)
