# Quietly Labs Inventory

Workspace checked from `/Users/razzo/Documents/For Codex` on 2026-05-06.

## Strong candidates

### Sheet Doctor CLI

Path: `/Users/razzo/Documents/For Codex/sheet-doctor`

Why it fits:

- Standalone Python package and CLI.
- MIT licensed.
- Local-first positioning is already clear.
- Has tests, schemas, sample data, changelog, production blockers, and a strong README.
- Remote exists at `https://github.com/razzo007/sheet-doctor.git`.

Important boundary:

- Do not copy the active Quietly.tools web UI from `quietly.tools/quietly-tools/src/pages/SheetDoctor.jsx`.
- Labs should link to the CLI repo or include a small project card/case study.

Local cleanup before publishing or linking:

- `sample-data/public/` is untracked.
- `sheet-doctor-output/` is untracked.
- `skills/csv-doctor/scripts/__pycache__/` is untracked.

Recommended Labs status: `stable engine`.

### SalesGPT use-case simulator

Path: `/Users/razzo/Documents/For Codex/Salesgpttest1`

Why it fits:

- Small static prototype.
- Easy to explain as an AI workflow simulator.
- Does not appear to overlap with active Quietly.tools projects.

Recommended Labs status: `prototype`.

## Hold for now

### GST reconciliation / ClearLedger

Path: `/Users/razzo/Documents/For Codex/ClearLedger`

Why it is tempting:

- Clear pain: reconcile GSTR-2A/2B or GST schedules against purchase registers.
- FastAPI backend, React frontend, tests, country configs.
- Strong privacy-first positioning.

Why it should not be copied into Labs right now:

- There is an active Quietly.tools route at `quietly.tools/quietly-tools/src/pages/ClearLedger.jsx`.
- Quietly.tools has active ClearLedger i18n, SEO content, and GST reconciliation guide/template data.
- The local ClearLedger repo has modified files: `frontend/src/components/UploadZone.jsx` and `frontend/src/pages/ClearLedger.jsx`.
- The README points to `quietly.tools/clearledger`, so publishing it inside Labs could confuse product ownership.

Recommended move:

- Keep ClearLedger separate from Labs for now.
- Later, publish either a dedicated `clearledger` repo or a sanitized Labs case study called `How ClearLedger reconciles GST files locally`.
- A tiny related Labs tool is safer: `GST invoice number normalizer` or `GSTR-2B column mapper`.

Recommended Labs status: `hold`.

## Possible archive candidates

### Cinde executive brief prototype

Path: `/Users/razzo/Documents/For Codex/Cinde`

Why it might fit:

- Clear prototype around email-safe HTML plus hosted landing/audio playback.
- Useful public lesson: email clients cannot reliably play inline audio, so route to a landing page.

Risks:

- Mentions specific placeholder assets and external CDN URLs.
- Should be sanitized before publishing.

Recommended Labs status: `case-study` or `prototype`.

### Design Tribe Studio homepage concept

Paths:

- `/Users/razzo/Documents/For Codex/design-tribe-studio-home`
- `/Users/razzo/Documents/For Codex/thedesigncircuit-fordesigntribe`

Why it might fit:

- Design/prototype experiment with local intent matching.

Risks:

- Brand and logo assets may not belong in a public Quietly Labs repo.
- This is more portfolio/client-work adjacent than free-tool adjacent.

Recommended Labs status: `hold unless sanitized`.

