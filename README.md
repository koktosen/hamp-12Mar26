# Digital Shield — Private Security Briefing (12 Mar 26)

Static HTML landing page for the **Digital Shield** private security briefing event (Hampton, 12 March 2026).

## Contents

- **index.html** — Main page (served at site root on Netlify)
- **hampton-event-12mar26.html** — Same content, named copy

No build step or dependencies. Uses Google Fonts (loaded from CDN).

## Deploy on Netlify

1. Push this repo to GitHub: [koktosen/hamp-12Mar26](https://github.com/koktosen/hamp-12Mar26)
2. In [Netlify](https://app.netlify.com): **Add new site** → **Import an existing project** → choose **GitHub** and `koktosen/hamp-12Mar26`
3. Netlify will use the repo root as publish directory (no build command). Click **Deploy**.

Your site will be live at `https://<random>.netlify.app` (you can set a custom domain later).

## Run locally

Open `index.html` in a browser, or use a simple server:

```bash
# Python
python3 -m http.server 8000

# Node (npx)
npx serve .
```

Then visit `http://localhost:8000`.

## Push to GitHub

From the project folder, run:

```bash
git init
git add .
git commit -m "Initial commit: Digital Shield briefing page + Netlify config"
git branch -M main
git remote add origin https://github.com/koktosen/hamp-12Mar26.git
git push -u origin main
```

If the repo already has content (e.g. a README created on GitHub), use:

```bash
git pull origin main --allow-unrelated-histories
# resolve any conflicts, then:
git push -u origin main
```
