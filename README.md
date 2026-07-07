# PLE Kit — Batch Masikhay 2026

Guide to the October 2026 Physician Licensure Examination for the UP-PGH Batch
Masikhay 2026 graduation kit: PRC/LERIS application steps, documentary
requirements, key dates with a live countdown, exam coverage, and review tips.

Static site — a single `index.html`, no build step, no dependencies.

## Deploy to Vercel

**Option A — Dashboard (fastest)**
1. Push this repo to GitHub (see below).
2. On [vercel.com](https://vercel.com) → **Add New → Project** → import the repo.
3. Framework preset: **Other**. Leave build command and output directory empty.
4. Deploy. Done.

**Option B — CLI**
```bash
npm i -g vercel
vercel --prod
```

## Push to GitHub

```bash
git remote add origin https://github.com/<your-username>/ple-kit-masikhay-2026.git
git branch -M main
git push -u origin main
```

## Generate the QR code

Once deployed, point any QR generator at the production URL
(e.g. `https://ple-kit-masikhay-2026.vercel.app`). For print in the kit cards,
export the QR as **SVG or ≥600×600 px PNG** with a quiet zone, and test-scan
from a printed proof before the full print run.

## Updating for March 2027

The countdown dates live in one block at the top of the inline `<script>` in
`index.html` (`open`, `deadline`, `examStart`, `examEnd`, `results`). When PRC
releases the 2027 exam calendar (usually November), update those five dates and
the corresponding text in the timeline cards and hero.

## Sources

Content is based on official PRC issuances as of July 2026, primarily the
[2026 Schedule of Examinations](https://www.prc.gov.ph/2026-schedule-examination)
(Resolution No. 2113, s. 2025) and the
[PRC List of Requirements](https://www.prc.gov.ph/list-of-requirements).
Always cross-check against [prc.gov.ph](https://www.prc.gov.ph) before acting.
