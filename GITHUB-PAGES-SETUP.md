# CyberZone hosting

This repository supports both Netlify (root `/`) and GitHub Pages (`/cyberzone/`).

## GitHub Pages

Repository Settings > Pages > Source: **GitHub Actions**.

The `.github/workflows/deploy.yml` workflow runs `npm ci`, builds with `--base=/cyberzone/`, copies `index.html` to `404.html` for deep-link refreshes, and deploys `dist`.

The site is at https://g7nikhil.github.io/cyberzone/ .

Note: GitHub Pages serves the fallback page with HTTP 404 status for direct deep links even though the app displays the correct content. This is a GitHub Pages limitation.

## Netlify

Keep the existing build command `npm run build` and publish directory `dist`. The `public/_redirects` file handles direct deep links on Netlify.

## Local testing

`npm ci` then `npm run dev`. For production testing, `npm run build` and `npm run preview`.
