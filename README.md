# Ducks In Order v3 — Study Library

GitHub Pages static site. Upload all files to the root of your existing repository, replacing matching files.

## Content
- 9 learning tracks, 52 mapped lessons.
- 21 complete lessons: SQL (9), Python (6), Statistics (6).
- Other subjects remain marked Planned; no empty lesson links.
- Each ready lesson includes concept, example, breakdown, practice, reference solution, takeaways.

## Using
Open Curriculum to select any Ready lesson; use Study Guides to learn and Practice Lab to answer then reveal the reference. Practice responses are not saved or automatically graded.

## Adding a lesson
Create `lessons/<id>.json` with fields `concept`, `example`, `breakdown` (array), `practice`, `answer`, `takeaways` (array); set corresponding catalog status to `ready`.

## Caveats
Code samples are educational examples, not executed by the website. Verify against your own schema and environment. The website is public; do not paste confidential employer data.


## Version 4 additions
- Every ready lesson includes curated, free written resources (no video courses).
- Each of 21 ready lessons includes a one-question, multiple-choice concept check with feedback.
- Mark lessons complete and set a self-assessed 0–4 mastery score.
- Save practice drafts locally; export/import JSON progress backups on Mastery page.
- Progress uses browser localStorage, not GitHub or a backend; it does not sync across devices.
- Concept checks grade predefined answers only. SQL/Python free-response exercises are **not** automatically executed or graded.
- Do not upload a personal progress backup into the public GitHub repository.
- Lesson content lives in lessons/*.json; resources are in each lesson's `resources` list.


## Version 5
- Curriculum is the high-level map, with direct lesson links, progress labels, and inline per-lesson note editors.
- Study Guides retain the full instructional material and now include the same per-lesson note.
- Notes page lists personal notes alongside existing reference notes.
- Personal notes are stored in `localStorage` under `ducks-in-order-lesson-notes-v5` and are browser-specific. Back up important notes manually.
- Version 4 progress is retained in its original key.
