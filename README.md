# Ducks In Order — GAJ

A personal GitHub Pages learning dashboard built from the visual design of the `home_` portfolio (HTML/CSS/JS, Montserrat, particles.js, duck favicon).

## Publish
1. Create a **public** GitHub repository named `ducks-in-order`.
2. Upload **the contents** of this folder to the repository root (not the enclosing folder).
3. In **Settings → Pages**, choose **Deploy from a branch**, `main`, `/ (root)` and Save.
4. Open `https://ameliameyer.github.io/ducks-in-order/` after deployment.

No changes to your existing `home_` repository are needed. An unlinked public Pages site is **not private**. Do not commit personal or employer-confidential data.

## Updating progress
- `data/skills.json`: change `score` from `null` to 0–4 **only after assessment**. Set `status`, `last_assessed` (YYYY-MM-DD), and optionally `evidence` with objects `{ "label": "SQL diagnostic", "url": "https://..." }`.
- `data/roadmap.json`: update `status` and `completed` when phases are finished.
- `data/notes.json`: add an entry for each new Markdown note with `title`, `category`, `file`, and `description`.
- `notes/*.md`: write notes in Markdown. The lightweight reader supports headings, paragraphs, and fenced code; richer Markdown formatting can be added later.

## Local preview
Run `python -m http.server 8000` in this folder, then visit `http://localhost:8000/`. Opening the HTML directly from disk will not load JSON data because browsers restrict `file://` fetches.

## Version 1 boundaries
This is a read-only dashboard, not a browser-based editor. Updating mastery scores requires editing JSON in GitHub. Search filters note titles, categories, and descriptions, not full note bodies. No quizzes or accounts yet.
