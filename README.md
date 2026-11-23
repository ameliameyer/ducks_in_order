# Ducks In Order — v2

A GitHub Pages learning hub reusing the portfolio visual theme.

## Publish / upgrade

Upload **all contents** of this ZIP to the root of the existing `ducks-in-order` repository, replacing same-named files and adding new ones. Do **not** create a second repository. GitHub Pages should remain set to `main` / `(root)`.

## What's available

- Dashboard, roadmap, curriculum catalog, study guides, practice lab, notes, mastery tracker.
- 9 learning tracks and a complete concept-level catalog.
- Three fully written SQL lessons with examples, explanations, exercises, and reference answers. Other topics are **clearly labeled Planned**, not presented as finished lessons.
- Lessons follow Concept → Example → Breakdown → Practice → Takeaways.
- Existing skill scores remain unassessed.

## Update content

- `data/catalog.json`: all lesson titles and readiness flags.
- `lessons/*.json`: fully written lesson content; add a new JSON file and change the matching catalog item from `planned` to `ready`.
- `data/skills.json`: verified mastery scores (null means unassessed).
- `data/roadmap.json`: curriculum phases.
- `data/notes.json` and `notes/*.md`: personal notes.

## Limitations

This is a static website. Exercises are self-checked, not executed or graded. Text entered into the practice area is not saved to GitHub. There is no authentication; all content in a public repository and public GitHub Pages site is publicly accessible even if not linked from your portfolio. Never publish work/customer data or personal secrets.

## Local preview

Run `python -m http.server 8000` from this directory, then visit `http://localhost:8000`. Opening HTML directly as `file://` may block JSON loading.
