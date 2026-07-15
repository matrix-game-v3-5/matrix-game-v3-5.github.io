# Matrix-Game 3.5 — Project Page

Project homepage for **Matrix-Game 3.5: Enhancing Real-Time Streaming Interactive World Models with Patch Memory** (Riemann Dynamics).

Deployed via GitHub Pages at **https://matrix-game-v3-5.github.io**.

## Structure

- `index.html` — the entire single-page site (inline CSS/JS; fonts & icons via CDN).
- `static/imgs/mg35/` — figures (PRoPE, pose-aware sequence, memory system, distillation), the quantitative table, and the logo.
- `static/videos/` — demo videos, H.264-compressed and bundled in the repo (~300 MB total):
  - `teaser_mg35_2x3.mp4` — abstract teaser (1280×480)
  - `mg35_1p/fp_01.mp4 … fp_13.mp4` — first-person (1280×704)
  - `mg35_3p/tp_01.mp4 … tp_15.mp4` — third-person (1280×704)

All video paths are prefixed by `MEDIA_BASE = 'static/videos'` in `index.html`.

## Local preview

```bash
# any static file server works, e.g. the bundled PowerShell one:
powershell -NoProfile -ExecutionPolicy Bypass -File serve.ps1
# then open http://localhost:8321
```
