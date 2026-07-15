# Matrix-Game 3.5 — Project Page

Project homepage for **Matrix-Game 3.5: Enhancing Real-Time Streaming Interactive World Models with Patch Memory** (Riemann Dynamics).

Deployed via GitHub Pages at **https://matrix-game-v3-5.github.io**.

## Structure

- `index.html` — the entire single-page site (inline CSS/JS; fonts & icons via CDN).
- `static/imgs/mg35/` — figures (PRoPE, pose-aware sequence, memory system, distillation), the quantitative table, and the logo.

## Videos (external hosting)

To keep the repo light and stay under the GitHub Pages 1 GB limit, the demo videos are **not** committed. They are loaded from an external host defined by `MEDIA_BASE` in `index.html`:

```js
const MEDIA_BASE = IS_LOCAL
  ? 'static/videos'
  : 'https://REPLACE-WITH-YOUR-MEDIA-HOST/matrix-game-v3-5';   // ← set your external video host
```

Upload the following to that host, preserving the folder names:

- `teaser_mg35_2x3.mp4` (abstract teaser)
- `mg35_1p/fp_01.mp4 … fp_13.mp4` (first-person)
- `mg35_3p/tp_01.mp4 … tp_15.mp4` (third-person)

On `localhost` the page automatically falls back to `static/videos/` for local preview.

## Local preview

```bash
# any static file server works, e.g. the bundled PowerShell one:
powershell -NoProfile -ExecutionPolicy Bypass -File serve.ps1
# then open http://localhost:8321
```
