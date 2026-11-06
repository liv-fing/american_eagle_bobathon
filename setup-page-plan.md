# Plan: Standalone Setup Page

## Overview

Create a new standalone page `docs/setup.html` that shows only the Environment Setup card. No changes to the main page (`docs/index.html`), `app.js`, or any existing files. The Setup card will remain on the main page as-is.

The new page reuses all shared CSS, JS, images, and the existing `docs/tracks/setup.html` partial. The only mechanism needed is setting `window.FLIGHT400_CONFIG.tracks = ['setup']` before `app.js` loads — this uses the existing config override that already exists in `app.js`.

**Scope:**
- Create `docs/setup.html` (new file only)

**Non-goals:**
- No changes to `docs/index.html`
- No changes to `docs/js/app.js`
- No changes to `docs/tracks/setup.html`
- No changes to any exercise track files
- No changes to `docs/_template/`

---

## Sub-Task 1 — Create `docs/setup.html`

**Intent:** Build a self-contained standalone page that loads only the Setup card, reusing all shared assets and interactivity.

**Expected Outcomes:**
- `docs/setup.html` exists and renders only the Setup card
- All setup interactivity works: accordion steps, copy buttons, attendee table row selection, student badge, token replacement (`FLGHT4nn`, `30nn`, etc.)
- Page has a "← Back to Lab Exercises" link pointing to `index.html`
- Page title is "Environment Setup — FLIGHT400 Lab"
- Visually consistent with the main page (same theme toggle, same starfield, same CSS)

**Todo List:**
1. Create `docs/setup.html`
2. Copy the full `<head>` from `docs/index.html` — update the `<title>` to `Environment Setup — FLIGHT400 Lab`
3. Include the theme toggle button (same as `index.html`)
4. Include the starfield `<canvas id="stars-canvas">` inside `.page-clip`
5. Replace the hero section with a minimal page header: "Environment Setup" title + "← Back to Lab Exercises" link to `index.html`
6. Add a `<section class="scroll-section" id="tracks-section">` containing `<div class="tracks-stream" id="tracks-stream"></div>` — `app.js` injects the card here
7. Add the student badge markup (same as `index.html`) so token replacement works
8. Add a `<footer>`
9. Before loading `js/app.js`, add an inline `<script>` that sets `window.FLIGHT400_CONFIG = { tracks: ['setup'] }` — this uses the existing override in `app.js` (line 138–139) to load only the setup track
10. Load `<script src="js/app.js?v=2"></script>`

**Relevant Context:**
- `docs/js/app.js` lines 138–139: `var cfgTracks = (window.FLIGHT400_CONFIG || {}).tracks;` — if set, this replaces `DEFAULT_TRACK_SLUGS` entirely, so `{ tracks: ['setup'] }` loads only the setup card with no other changes needed
- `docs/index.html`: reference for full page structure, student badge markup, theme toggle
- `docs/tracks/setup.html`: the setup card partial — loaded as-is, no changes
- `docs/css/styles.css`: shared stylesheet — referenced as `css/styles.css` (same relative path works from `docs/`)

**Status:** [x] done

---

## Sub-Task 2 — Verify and push

**Intent:** Confirm the setup page works end-to-end before committing.

**Expected Outcomes:**
- `docs/setup.html` renders the Setup card with all steps and interactivity
- Student row selection and token replacement work
- Theme toggle works
- Back link points correctly to `index.html`
- No broken assets or console errors
- Changes committed and pushed to `origin` and `upstream`

**Todo List:**
1. Open `docs/setup.html` in a browser and confirm the Setup card loads
2. Click a student row and confirm `FLGHT4nn` / `30nn` tokens are replaced throughout
3. Confirm the back link navigates to the main page
4. `git add`, `git commit`, `git push origin main`, `git push upstream main`

**Status:** [ ] pending
