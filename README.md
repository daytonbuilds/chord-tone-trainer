# 1·3·5·7 Chord Tone Trainer

Installable, offline-capable trainer for seventh-chord spelling, degrees, and ear recognition.
Static site, no build step. Deployed with GitHub Pages (Settings → Pages → Deploy from a branch → `main` / root).

- `index.html`: the whole app (markup, styles, script)
- `sw.js`: service worker. The page is network-first (deploys show up on the next online launch); fonts and icons are cache-first. Bump `CACHE` only if you rename or remove a precached asset.
- `fonts/`: self-hosted latin subsets of Fraunces, Inter, JetBrains Mono (SIL OFL, via Fontsource)
- Progress is stored in `localStorage` on the deployed origin.

Local preview: `npx serve .` (service workers need http://localhost or https).
