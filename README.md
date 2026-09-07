# DLSU Term 1 AY26-27 — Home

A single-page dashboard for the term: six subjects, a live deadline tracker (tick items off — saved in your browser via `localStorage`), weekly study-hour targets, a collision calendar, and links out to Canvas, the NotebookLM notebooks, and the study guides.

- **Live site:** _(GitHub Pages URL added after first deploy)_
- **Source:** `index.html` — one standalone file, no build step, no dependencies except Google Fonts.

## Editing

It's a plain HTML file. The data lives in `<script>` at the bottom of `index.html`:

- `SUBJECTS` — the six subject cards (name, prof, schedule, status, and the Canvas / Notebook / Guide links).
- `D` — the deadline list: `["CODE", "Task name", "ISO datetime with +08:00"]`. Add a row here and it shows up in the tracker, the countdowns, and the per-subject "next deadline".
- `WK` / `WKDATES` — the 13-week study-hours matrix: `[ACY, STRM, LYTC, MECO, EDEV, COMM, total, "driver note"]`.

The collision calendar and the COBSTRM note are plain HTML in the `#crunch` section.

After any change: commit and push to `main`; GitHub Pages redeploys in ~1 minute.

## Status of the six subjects (as of Sep 7, 2026)

| Subject | State |
|---|---|
| ACYFDR1 · COBSTRM · COBEDEV | Active — deadlines loaded |
| DSILYTC | Module 1 posted, no graded work yet |
| COBMECO | Syllabus only; essay exams; Long Exam + PPT dates pending |
| ACTCOMM | Nothing posted in Canvas |

Local source archive of every Canvas file: `~/Documents/dlsu-notebooklm/`.
