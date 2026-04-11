# lotta-lorette kalmaru · issue 01

Personal portfolio page. Single-file static site. Dark 90s editorial.

**Live:** _(fill in after Vercel deploy)_

## Stack
- Plain HTML + embedded CSS + ~10 lines of vanilla JS
- Google Fonts: Playfair Display, Inter, JetBrains Mono
- Assets: `images/` (jpeg) + `video/` (mp4)
- No build step
- Host: Vercel

## Local preview
```bash
# any static server works
python3 -m http.server 8000
# then open http://localhost:8000
```

## Deploy to Vercel
```bash
npx vercel          # first time — it'll link the project
npx vercel --prod   # subsequent deploys
```
Or: connect this GitHub repo to Vercel and every push to `main` auto-deploys.

## Editing copy
Everything is in `index.html`. Sections are clearly commented (00 cover, 01 eha, 02 stacc, 03 ecb, 04 research, 05 about, 06 back page). Design tokens (colors, fonts, spacing) live in the `:root {}` CSS variables at the top of the `<style>` block.

## Locked design decisions
See [`DESIGN.md`](./DESIGN.md) for the full locked creative direction — palette, type, section-by-section layout, copy rules.
