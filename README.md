# Hiring a full-time boyfriend — Chakra one-pager

A short, single-file landing page linked from the "Hiring a Boyfriend (via Chakra)" video.

- **`index.html`** — the whole page. No build step, no dependencies. Open it or drop it
  on any static host (GitHub Pages, Netlify, Vercel, S3, …).

## Layout

Two sections, fully dark mode, in the Chakra aesthetic:

1. **Hero** — "Hiring a *full-time boyfriend* 🖼 for *Ohshin* 🖼" with two inline images and
   the animated **Apply to be a boyfriend** button (opens the Chakra AI interview).
2. **Powered by Chakra** — two-line description + a **Try it for your team** button → https://chakra.sh

## Font: Kalice

Bundled in `fonts/` (Regular + Italic, `.woff2`) and loaded via `@font-face`. Nothing to do.

## Swapping the inline images

The two inline image slots use placeholders in `images/`:

- `images/boyfriend.svg` — the slot after "full-time boyfriend"
- `images/ohshin.svg` — the slot after "Ohshin"

Replace either file (keep the same name), or point the `src` in `index.html` at your own
file (e.g. a `.jpg`/`.png`). They're sized as rounded "pills" and cropped with
`object-fit: cover`, so roughly landscape images look best.

## Links

- Apply (AI interview): `https://www.chakra.sh/interviewer/onboarding/0/df07gfkmcjp/30de807564929c16e5207bfe8f0be942`
- Chakra: `https://chakra.sh`

## Run locally

```bash
python3 -m http.server 8000   # then open http://localhost:8000
```
