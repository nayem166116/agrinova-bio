# Colonize Bio website

Static multi-page site: HTML, vanilla CSS, vanilla JS. No build step.

## Preview

`python3 -m http.server 8080 --directory .` then open http://localhost:8080

## Deploy

Upload the folder to Vercel, Netlify, Cloudflare Pages or any static host. `vercel.json` sets clean URLs.

## Hero background video

`assets/media/hero-field.mp4` with poster `assets/media/hero-field.jpg`. Replace both with real product footage using the same filenames and no code changes are needed. Keep the file under ~3 MB and encode with `-movflags +faststart`.

## Home page order

Minimal video hero, then the standalone product line index (#product-line), then the full label specifications (#products), then evidence and programme sections.

## Notes

- No dashboard, no internal route, and no authentication anywhere on the site.
- This is a business-to-business information site: the only conversion is the contact page.
- Cookie preferences are stored in the browser only.
- Logo assets live in `assets/brand/`. Replace any file there (same file name) to change the logo across the whole site; see `assets/brand/README.md`.

## IMPORTANT: how to deploy

The files in THIS folder (index.html, vercel.json, assets/) must sit at the ROOT of the deployment.

If you get a `404: NOT_FOUND` on Vercel, it is because the project root contains an `colonize-bio` folder instead of `index.html` directly.

### Vercel drag-and-drop

Drag the `colonize-bio` FOLDER itself onto Vercel (not a zip containing it). Vercel then uses the folder contents as the root.

### Vercel via Git

Commit the CONTENTS of this folder at the repository root, so `index.html` sits next to `vercel.json`. Framework preset: Other. Build command: none. Output directory: leave empty.

### Netlify / Cloudflare Pages

Set the publish directory to the folder that contains `index.html`. No build command.

Note: there is deliberately no folder named `public` here, because some hosts treat `public` as the output directory and would serve that instead of the site.
