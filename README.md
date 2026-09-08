# Offline Notes Lab

A small React Progressive Web App based on the supplied practical guide. It saves notes in browser local storage, reports network state, includes an install manifest, and caches the app shell for offline use.

## Run locally

```powershell
cd C:\Users\DELL\Documents\Codex\2026-09-07\he\offline-notes-lab
npm install
npm run dev
```

Open the local URL printed by Vite.

## Verify the production PWA

```powershell
npm run check
npm run build
npm run preview
```

Open the preview URL once while online. In a Chromium browser, inspect Developer Tools > Application to confirm the manifest and service worker. Then use Developer Tools > Network > Offline and reload. A note saved before or after the reload should remain because it is stored in local storage.

## Deploy

Deploy the contents of `dist` to any HTTPS static host such as Netlify, Vercel, or GitHub Pages. Use `npm run build` as the build command and `dist` as the publish directory.
