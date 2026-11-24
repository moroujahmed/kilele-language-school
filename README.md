# Kilele Language School — GitHub Pages task

This repository contains the static website for the S2 Core Services & Platform Navigation task.

## Files
- `index.html` — Resource B starter website with a visible registration announcement.
- `404.html` — custom not-found page for GitHub Pages.
- `contact.html` — demonstration registration page; it does not transmit or store form data.
- `ROLLBACK_RUNBOOK.md` — five-step rollback procedure.
- `.github/workflows/pages.yml` — Pages deployment workflow.

## Enable publishing
1. Open **Settings → Pages**.
2. Under **Build and deployment → Source**, select **GitHub Actions**.
3. The workflow deploys the repository root when commits are pushed to `main`.
4. Wait for the **Deploy to GitHub Pages** workflow to complete, then open the published URL shown under Settings → Pages.

## Important
This public repository is only for the public website. It is not suitable for private student records or the school's 50 GB storage requirement. The form is a front-end demo only. Before collecting real data, connect an approved secure form/backend and implement the school's privacy, access-control, retention, and under-16 consent requirements.
