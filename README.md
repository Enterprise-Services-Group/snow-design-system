# UoM SNOW Design System

A static HTML/CSS design system and interactive prototype extracted from the University of Melbourne's Staff Services ServiceNow portal.

## Live prototype

> After GitHub Pages is enabled, the site will be available at:  
> `https://enterprise-services-group.github.io/<repo-name>/`

| Page | Description |
|---|---|
| `index.html` | Design system component showcase |
| `form-prototype.html` | Re-use Lab Equipment Initiative form prototype |

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

### Step 1 — Create the repository

1. Go to [github.com/Enterprise-Services-Group](https://github.com/Enterprise-Services-Group)
2. Click **New repository**
3. Name it `snow-design-system` (or your preferred name)
4. Set visibility to **Public**
5. Leave "Initialize this repository" **unchecked**
6. Click **Create repository**

### Step 2 — Push files

Run these commands from the project folder:

```bash
cd "/Users/pleonravest/Library/CloudStorage/OneDrive-TheUniversityofMelbourne/Documents/UoM - Github/SNOW design system"

git init
git add .
git commit -m "Initial commit: UoM SNOW design system + form prototype"
git branch -M main
git remote add origin https://github.com/Enterprise-Services-Group/snow-design-system.git
git push -u origin main
```

### Step 3 — Enable GitHub Pages

1. Go to the repository on GitHub
2. Click **Settings** → **Pages**
3. Under *Source*, select **Deploy from a branch**
4. Branch: `main` · Folder: `/ (root)`
5. Click **Save**

Your site will be live at `https://enterprise-services-group.github.io/snow-design-system/` within ~1 minute.

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
