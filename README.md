# UoM SNOW Design System

A static HTML/CSS design system and interactive prototype extracted from the University of Melbourne's Staff Services ServiceNow portal.

## Live prototype

This project is ready to publish as a static site on GitHub Pages.

After the folder is pushed to a GitHub repository and Pages is enabled, the site will be available at:

`https://<your-github-username-or-org>.github.io/<repo-name>/`

Use `index.html` as the public entry point. It now links to the main live prototype pages.

| Page | Description |
|---|---|
| `index.html` | Landing page with links to all live prototype pages and design system showcase |
| `home.html` | Faculty of Science Lab Reuse Initiative homepage |
| `ServiceNow_form_prototype_ver2.html` | Donation form prototype |
| `reuse-store.html` | Reuse store prototype |
| `ServiceNow_receiver_form_prototype.html` | Receiver request form prototype |

---

## What's included

### Design tokens (`css/tokens.css`)
All visual values as CSS custom properties — colours, typography, spacing, radii, shadows.

| Token | Value | Usage |
|---|---|---|
| `--uom-blue` | `#0076de` | Primary actions, links, badges |
| `--uom-navy` | `#004576` | Header logo block, page titles |
| `--uom-body` | `#191414` | Body text |
| `--uom-bg` | `#f9f9f9` | Page background |
| `--uom-font` | Roboto, Helvetica, Verdana | All text |

### Component styles (`css/uom-snow.css`)
- Header / Navbar (UoM logo block, breadcrumb, avatar)
- Page title block
- Panels / Cards
- Form inputs (text, select, textarea, date, file upload)
- Radio groups & checkboxes
- Buttons (primary, secondary, danger · sizes: sm, default, lg)
- Alerts (success, info, warning, danger)
- Badges
- Validation states (error, focus)
- Footer

---

## GitHub Pages setup

This repo includes a GitHub Actions workflow at `.github/workflows/deploy-pages.yml` that deploys the site automatically.

### Step 1 — Create a GitHub repository

1. Create a new GitHub repository.
2. Choose any repository name you want.
3. Set visibility to `Public` if you want GitHub Pages on a free plan.

### Step 2 — Push this folder

Run these commands from this project folder:

```bash
cd "/Users/pleonravest/Library/CloudStorage/OneDrive-TheUniversityofMelbourne/Documents/UoM - Github/ServiceNow-form---Reuse-initiative-main"

git init
git add .
git commit -m "Prepare static site for GitHub Pages"
git branch -M main
git remote add origin https://github.com/<your-account>/<repo-name>.git
git push -u origin main
```

### Step 3 — Enable GitHub Pages

1. Open the repository on GitHub.
2. Go to `Settings` > `Pages`.
3. Set `Source` to `GitHub Actions`.

Each push to `main` will redeploy the site automatically.

### Step 4 — Open the live site

Your site URL will be:

`https://<your-github-username-or-org>.github.io/<repo-name>/`

The main pages will then be available at:

- `/`
- `/home.html`
- `/ServiceNow_form_prototype_ver2.html`
- `/reuse-store.html`
- `/ServiceNow_receiver_form_prototype.html`

---

## Project structure

```
/
├── index.html              Design system showcase
├── form-prototype.html     Re-use Lab Equipment form prototype
├── css/
│   ├── tokens.css          CSS custom properties (design tokens)
│   └── uom-snow.css        Component styles
├── assets/
│   ├── logo.png            UoM header logo (dark navy square)
│   └── lockup.png          UoM footer lockup
└── README.md
```

---

## Source reference

Design tokens extracted from:
- `Faculty of Science Lab Operations Request - Staff Services.html`
- `FEIT lab services - Staff Services.html`

University of Melbourne Staff Services portal — ServiceNow Service Portal.
