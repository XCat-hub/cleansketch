# CleanSketch Website

Official marketing site and legal pages for [CleanSketch](https://play.google.com/store/apps/details?id=com.gzll.cleansketch) — a drawing and coloring app for Android.

**Live URL:** https://xcat-hub.github.io/cleansketch/

The Android app opens these paths from Settings and sign-in:

- https://xcat-hub.github.io/cleansketch/PRIVACY_POLICY.html
- https://xcat-hub.github.io/cleansketch/TERMS_OF_SERVICE.html

Google Play Console account deletion URL:

- https://xcat-hub.github.io/cleansketch/delete-account.html

## Pages

| Path | Description |
|------|-------------|
| `/` | Product homepage |
| `/PRIVACY_POLICY.html` | Privacy Policy |
| `/TERMS_OF_SERVICE.html` | Terms of Service |
| `/delete-account.html` | Account & data deletion request |
| `/app-ads.txt` | AdMob `app-ads.txt` (also copied under `public/`) |

## Development

```bash
npm install
npm run dev      # http://localhost:4321/cleansketch/
npm run build    # output to dist/
npm run preview  # preview production build
```

## Deployment

Push to `main` triggers GitHub Actions, which builds Astro and publishes `dist/` to the `gh-pages` branch.

**GitHub Pages settings** (repo → Settings → Pages):

- Source: **Deploy from a branch**
- Branch: **gh-pages** / **/(root)**

## Content sources

- Product copy: `pure-draw` Play listing draft and in-app Pro benefits
- Legal pages: `src/content/legal/*.md`
- Brand colors: CleanSketch MD3 palette (`#5B5FC7`)

## Project structure

```
src/
├── components/     # Hero, Features, FAQ, …
├── content/legal/  # Privacy & Terms markdown
├── layouts/        # BaseLayout
├── pages/          # Routes (index, PRIVACY_POLICY.html, …)
└── styles/         # Global CSS
public/             # favicon, app-ads.txt, robots.txt
```
