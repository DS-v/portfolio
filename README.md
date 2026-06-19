# Divyanshu Shukla — PM Portfolio

Static portfolio site (plain HTML/CSS, no build step). Designed to be hosted on **GitHub Pages**.

## Structure

```
index.html                              ← homepage
artifact-1-why-platforms-break.html     ← 01 · Why Cross-Border Procurement Platforms Break
artifact-2-system-design.html           ← 02 · End-to-End Procurement System Design
artifact-3-ai-matching.html             ← 03 · AI Matching: Reality vs Expectation
artifact-4-decision-tradeoffs.html      ← 04 · Decision Tradeoffs Under Founder-Led Strategy
artifact-5-granola-teardown.html        ← 05 · The Discipline of Subtraction (Granola teardown)
artifact-6-lecturesnap.html             ← 06 · LectureSnap — AI Build & Evaluation
assets/
  pf-chrome.css                         ← shared nav + prev/next pager styling
  Divyanshu_Shukla_PM_Resume.pdf        ← downloadable résumé
.nojekyll                               ← tells GitHub Pages to serve files as-is
```

All pages share one design system: **Archivo** headings, **Spectral** body, **JetBrains Mono** labels,
on the warm paper / ink / amber palette. Navigation (top nav + prev/next pager) is identical everywhere
and lives in `assets/pf-chrome.css`.

## Before you publish — fill in these placeholders

Search the repo for `REPLACE_` and swap in real URLs:

| Placeholder | Where | What to put |
|---|---|---|
| `REPLACE_LINKEDIN_URL` | `index.html` (contact) | Your LinkedIn profile URL |
| `REPLACE_PRD_URL` | `artifact-6-lecturesnap.html` ×2 | Public link to the LectureSnap PRD |
| `REPLACE_CATALOGUE_URL` | `artifact-6-lecturesnap.html` ×3 | Public link to the 106-mode failure catalogue |
| `REPLACE_EVAL_XLSX_URL` | `artifact-6-lecturesnap.html` ×2 | Public link to the six-lecture eval results (xlsx) |

Already working: the Figma board link (artifact 2) and the LectureSnap GitHub link (artifact 6).
The personal GitHub link in `index.html` points to `https://github.com/DS-v` — change if needed.

## Deploy to GitHub Pages

**Option A — user site (`username.github.io`):**
1. Create a repo named `DS-v.github.io` (use your exact GitHub username).
2. From this folder:
   ```bash
   git init
   git add .
   git commit -m "Portfolio site"
   git branch -M main
   git remote add origin https://github.com/DS-v/DS-v.github.io.git
   git push -u origin main
   ```
3. Live at `https://DS-v.github.io` within a minute or two.

**Option B — project site (any repo name, e.g. `portfolio`):**
1. Push this folder to a repo (same steps, different remote URL).
2. Repo → **Settings → Pages → Build and deployment** → Source: *Deploy from a branch* → Branch: `main` / `/ (root)`.
3. Live at `https://DS-v.github.io/portfolio/`.

All internal links are relative, so both options work without changes.
