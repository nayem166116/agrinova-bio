# Colonize Bio logo assets

Every file here is copied to `assets/brand/` in the built site. The site never
hard-codes the artwork, so **replacing a file here replaces the logo everywhere.**

## Files

| File | Where it is used | Replace with |
| --- | --- | --- |
| `logo-mark.svg` | Header mark on light pages | Square-ish mark, 40x40 viewBox, dark artwork |
| `logo-mark-light.svg` | Header mark over the video hero, footer mark | Same mark, light artwork |
| `logo-badge.svg` | App icon, avatars, OG image | 64x64 viewBox, own background |
| `logo-lockup.svg` | Decks, invoices, email signatures | Mark + wordmark, dark |
| `logo-lockup-light.svg` | Same, on dark backgrounds | Mark + wordmark, light |
| `favicon.svg` | Browser tab | 32x32 viewBox badge |
| `favicon.png` | Fallback favicon | 48x48 PNG |
| `apple-touch-icon.png` | iOS home screen | 180x180 PNG |
| `icon-512.png` | PWA / store listings | 512x512 PNG |
| `favicon.ico` | Legacy browsers | 16+32 ICO |
| `og-image.png` | Link previews (og:image) | 1200x630 PNG |

## How to replace

1. Keep the **same file names**. Nothing else has to change.
2. Keep the same viewBox / pixel dimensions so the header mark stays 28px and the
   favicon stays sharp.
3. Two variants are required: dark artwork for light backgrounds
   (`logo-mark.svg`) and light artwork for the dark video hero and footer
   (`logo-mark-light.svg`). The header swaps between them automatically.
4. If you only have one raster logo, save it as `logo-mark.svg`'s replacement in
   SVG if possible; PNG will blur on high-density screens.

## Design of the current mark

- A root axis with two lateral roots and three colony nodes: the colonisation the
  products actually do, and a graph shape for the AI models.
- The seed node is the accent: pine on light backgrounds, lime on dark.
- Palette is the site's own tokens: forest `#12211E`, pine `#1F6F5C`,
  lime `#C9E265`, mist `#F2F5F1`.
- Stroke weight 2.4 on a 40x40 grid, round caps, matching the site's line art.
