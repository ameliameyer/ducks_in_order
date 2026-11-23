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


## Version 6 — lesson notebook
Each lesson has Existing Notes and Add a New Note. Entries append rather than replace earlier notes. Previous v5 notes migrate automatically in the same browser. Notes page offers JSON export and import (merging without duplicates). Upload exported `ducks-in-order-notes.json` to GitHub for backup; to restore, download and import it on Notes. Uploading alone does not sync the website automatically. Avoid private information in public repositories.


## Version 7
- Updated site-wide hero to My Learning Lab and removed GAJ.
- Dashboard title and description updated.
- Curriculum page explicitly titled Full Curriculum; Study Guides remains a separate lesson reader.
- Bumped CSS/JS cache version to 7.


## Version 8 — Curriculum audit, deeper study guides, Projects

- Expanded the curriculum from 52 to 155 mapped topics across 18 tracks; 21 existing study guides remain Ready, 134 are honestly marked Planned. Audit counts and gap list: `data/curriculum-audit.json`.
- All 21 existing SQL, Python and Statistics lessons now have explicit objectives, common mistakes and transfer exercises; five key lessons have additional authored deep-dive explanations and examples. The original lesson content and existing notes/mastery storage are preserved.
- New `projects.html`: add projects, choose any number of curriculum topic tags, update status, edit or delete projects, and export/import JSON. Data lives in browser localStorage until exported; committing an export to GitHub is manual.
- Project backups are separate from notes and mastery backups. Existing v6 notes continue to use the same storage key.


## Version 10 — Depth and cumulative assessments
- Eight existing SQL, Python, and Statistics lessons gained expanded deep dives, practical code where appropriate, and diagnostic questions.
- New Assessments page includes three realistic cross-topic scenarios with local draft autosave and revealable reference solutions. Assessments are self-reviewed; no execution or automatic grading.
- Existing notes, projects, and mastery storage formats are unchanged. Export backups before updating.
