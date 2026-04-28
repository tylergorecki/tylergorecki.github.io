# tylergorecki.github.io

Personal portfolio website for Tyler Gorecki, Data Science professional.
Live at: https://tylergorecki.github.io | LinkedIn: https://linkedin.com/in/tylergorecki

## Project Overview

Static single-page portfolio deployed via GitHub Pages (auto-deploy from `main` branch). No build process, no framework, no npm.

## Tech Stack

- **Markup:** `index.html` — single page, all sections inline
- **Styles:** `assets/css/custom.css` (primary, 600+ lines) + `assets/css/main.css` (template base)
- **SASS source:** `assets/sass/` — compiled into `main.css`; exists for reference only
- **JS:** Vanilla JS + jQuery (minimal — gallery modal only)
- **Icons:** FontAwesome 6.0.0 (CDN)
- **Fonts:** Google Fonts (Source Sans Pro, Raleway)

## Development Workflow

- **Local preview:** VS Code Live Server on port 5501
- **Deploy:** push to `main` → GitHub Pages auto-deploys (no PR required)

## CSS Rule — Important

**All style changes go in `assets/css/custom.css` only.**

- Never edit `assets/css/main.css` — it's the Paradigm Shift template base; treat it as read-only
- Never edit files under `assets/sass/` — the SASS source is not part of the active workflow

## Design Constraints (always preserve)

- **Color scheme:** Navy/white — primary `#001f3f`, `#000f1f`; background `#f5f5f5`; accent `#0066cc`
- **Responsiveness:** Every change must work at 768px and 480px breakpoints
- **No new JS frameworks** — stay vanilla; no React, Vue, etc.
- **Minimize new dependencies** — avoid new CDN links or libraries unless clearly necessary

## Page Sections

Nav → Hero → About → Skills → Projects → Experience → Contact → Footer

### Projects (5 cards)
1. MLB Expected Runs Model (R, Statistics)
2. CFB Expected Points Model (Python, ML)
3. MLB Strike Zone Analysis (R Shiny, Visualization)
4. College Basketball Player Similarity (Python, Analytics)
5. Polymarket Edge Finder (Python, FAISS, Streamlit)

### Experience (5 entries, newest first)
1. Senior Technical Analyst — AMEND Consulting (Jul 2025–Present)
2. Data Scientist — UVA Sports Science and Analytics Collective (Jan 2023–Jul 2025)
3. Researcher — UVA Sports Analytics and Statistics Laboratory (Sep 2021–May 2024)
4. Researcher — Visual Intelligence Laboratory (Jan 2023–Jan 2024)
5. Data Science Intern — UVA Biocomplexity Institute (May 2023–Jul 2023)

## Planned Features

- Individual project detail pages
- **Resume/CV download button** — Tyler will provide the PDF; add as `.btn.btn-secondary` in the hero `.cta-buttons` with `href="assets/resume.pdf"` (or similar path) and `download` attribute

## Headshot

Profile photo lives at `images/headshot.jpg`. The About section displays it as a round image alongside the bio text. If the file is missing, the `onerror` handler hides it gracefully. LinkedIn blocked automated fetching — Tyler needs to add the file manually.

## Critical Files

| File | Purpose |
|---|---|
| `index.html` | All markup — single page |
| `assets/css/custom.css` | **Edit here for all style changes** |
| `assets/css/main.css` | Template base — READ-ONLY |
| `.vscode/settings.json` | Live Server port 5501 |
