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

## Assets you upload (recommended dimensions)

Replace these files (keep the same name), or repoint the `src` in `index.html`.
All three are center-cropped/scaled with CSS, so exact pixels aren't critical — just
match the aspect ratio.

| File | What | Recommended | Notes |
|------|------|-------------|-------|
| `images/boyfriend.webp` | hero photo after "full-time boyfriend" | **~600 × 320 px (≈1.9:1 landscape)** | shown as a small capsule; keep the subject centered. JPG/PNG fine — if so, update the `src` extension. |
| `images/ohshin.webp` | hero photo after "Ohshin" | **~600 × 320 px (≈1.9:1 landscape)** | same as above. |
| `images/chakra_logo.svg` | the full Chakra logo (clickable → chakra.sh) | **SVG preferred**; or transparent PNG **~360 × 96 px** | horizontal lockup, transparent background, light/white so it reads on the dark bg. Scales with the text. |
| `favicon.svg` | Minecraft-style 8-bit pixel heart | — | already done. |

> **Heads up on filenames:** the `src` attributes must match the file names exactly.
> The logo is wired to `images/chakra_logo.svg` (underscore). If you swap any asset for a
> different format/name, update the matching `src` in `index.html` and hard-refresh
> (**Cmd/Ctrl + Shift + R**) to clear the cached version.

## Links

- Apply (AI interview): `https://www.chakra.sh/interviewer/onboarding/0/df07gfkmcjp/30de807564929c16e5207bfe8f0be942`
- Chakra: `https://chakra.sh`

## Run locally

```bash
python3 -m http.server 8000   # then open http://localhost:8000
```
