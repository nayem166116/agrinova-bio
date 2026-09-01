# AgriNova Bio website

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

- No dashboard or internal route exists.
- Account actions route only to /login or /register.
- Cookie preferences are stored in the browser only.
- Add public/logo.png and public/icon.png before launch.
