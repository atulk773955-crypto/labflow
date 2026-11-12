# LabFlow: Every Laboratory. Under Control.

Laboratory management and inventory demo built for E-SUMMIT 2026 (Web / App Development).

**Live site:** `https://YOUR-USERNAME.github.io/labflow/` (after you follow the steps below)

## What it is
A static, no-build web app (plain HTML, CSS and JavaScript in one `index.html`). Click **Explore Live Demo** to open a working lab workspace:

- Chemical inventory: add, edit, delete, search, filter, sort
- Consumption recording with negative-stock protection
- Alerts for low stock, expiring or expired chemicals, maintenance due and pending requests, recalculated from current data
- Procurement: Pending, Approved, Ordered, Received (stock changes only on receipt)
- Equipment maintenance and fault reporting
- Analytics charts, CSV export and print for reports
- LabFlow Intelligence: rule-based answers from your data (no AI model connected)
- Reset Demo button

## Limitations (be upfront in your pitch)
- Demo data is stored in the visitor's browser (`localStorage`). There is no server, login or database.
- Roles are not enforced. Real authentication, row-level security and an AI integration need a backend (planned: Supabase).
- Pricing is a proposal, and no payment processing exists.
- Sample data is fictional. No safety or regulatory claims are made.

## Run locally
Open `index.html` in a browser. No install needed.

## Deploy with GitHub Pages
1. Create a new public repository named `labflow` on GitHub.
2. Push these files (see commands below).
3. Repo **Settings → Pages → Build and deployment → Source: Deploy from a branch**, branch `main`, folder `/ (root)`, then Save.
4. Wait 1 to 2 minutes. The site appears at `https://YOUR-USERNAME.github.io/labflow/`.

```bash
git init
git add .
git commit -m "LabFlow demo"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/labflow.git
git push -u origin main
```

## Roadmap
Supabase auth and Postgres with row-level security, atomic stock functions, server-side AI assistant, batch-level tracking, analytics filters.
