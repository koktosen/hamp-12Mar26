# Assets folder — images and favicons

## For images to show

1. **Keep this structure**
   - `index.html` and `hampton-event-12mar26.html` must sit in the **same folder** as this `assets` folder (sibling, not inside assets).
   - Reference images as: `assets/filename.png` (no leading slash).

2. **Local testing**
   - Opening the HTML file directly (`file://...`) can block images in some browsers. Use a local server instead:
     - `npx serve .` then open `http://localhost:3000`
     - or `python3 -m http.server 8000` then `http://localhost:8000`

3. **Netlify**
   - Push the whole project (including `assets/`) to GitHub. Netlify will serve `assets/` at `https://yoursite.netlify.app/assets/...`.

4. **File names**
   - Use lowercase and hyphens (e.g. `hero-banner.png`). Some hosts are case-sensitive.

## What’s here

| File | Used for |
|------|----------|
| `favicon.ico`, `favicon-16x16.png`, `favicon-32x32.png` | Browser tab icon |
| `apple-touch-icon.png` | iOS home screen |
| `android-chrome-192x192.png`, `android-chrome-512x512.png` | Android / PWA (via manifest) |
| `site.webmanifest` | PWA manifest (name, icons) |
| `hero-banner.png` | Hero image at top of page |

Add any other images (e.g. `your-image.png`) here and reference them in the HTML as `src="assets/your-image.png"`.
