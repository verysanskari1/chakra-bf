# Hiring a full-time boyfriend — Chakra one-pager

A short, single-file landing page linked from the "Hiring a Boyfriend (via Chakra)" video.

- **`index.html`** — the whole page. No build step, no dependencies. Open it or drop it
  on any static host (GitHub Pages, Netlify, Vercel, S3, …).

## Layout

Two sections, fully dark mode, with muted brand-color gradients in the background:

1. **Hero** — "Hiring a full-time boyfriend 🖼 for Ohshin 🖼" with two inline images and
   the **Apply to be a boyfriend** button (opens the Chakra AI interview).
2. **Chakra** — two-line description that opens with the clickable **Chakra logo** (→
   chakra.sh), then a **Try it for your team** button.

## Font: Kalice

Bundled `fonts/Kalice-Regular.woff2`, loaded via `@font-face`. Regular only — no italics.

## Assets you can swap

- `images/boyfriend.svg` / `images/ohshin.svg` — the two inline hero images
  (placeholders). Replace the files (same name) or repoint the `src` in `index.html`.
  Roughly landscape crops look best.
- `favicon.svg` — Minecraft-style 8-bit pixel heart.
- **Chakra logo** — reproduced inline as an SVG mark + wordmark (the official asset
  couldn't be fetched from this environment). Drop in the real Chakra SVG if you have it.

## Links

- Apply (AI interview): `https://www.chakra.sh/interviewer/onboarding/0/df07gfkmcjp/30de807564929c16e5207bfe8f0be942`
- Chakra: `https://chakra.sh`

## Run locally

```bash
python3 -m http.server 8000   # then open http://localhost:8000
```
