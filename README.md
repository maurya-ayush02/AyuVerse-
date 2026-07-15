# AyuVerse

**Where future engineers are built.**

AyuVerse is a free study hub for JEE Advanced aspirants — structured notes, previous year papers, and practice tests for **Physics**, **Chemistry**, and **Mathematics**, all in one place, all free.

This repo currently contains the **home page** and the site scaffold. Subject pages (`physics.html`, `maths.html`, `chemistry.html`) are live as branded "coming soon" placeholders, ready for real content next.

---

## What's inside

- Fully responsive home page (mobile menu, animated hero, subject cards, resources preview, about, contact)
- Animated announcement ticker at the very top
- A subjects dropdown in the nav (Physics / Mathematics / Chemistry)
- Custom favicon + app icons generated from your logo
- GitHub Codespaces config — opens ready to preview, no setup
- GitHub Actions workflow to auto-deploy to GitHub Pages
- Plain HTML/CSS/JS — no build step, no framework required

## Folder structure

```
ayuverse/
├── .devcontainer/
│   └── devcontainer.json      # Codespaces config
├── .github/
│   └── workflows/
│       └── deploy.yml         # auto-deploy to GitHub Pages
├── assets/
│   └── images/                # logo, icons, subject artwork
├── css/
│   └── style.css
├── js/
│   └── script.js
├── index.html                 # home page
├── physics.html                # placeholder — full page next
├── maths.html                  # placeholder — full page next
├── chemistry.html              # placeholder — full page next
├── 404.html
├── site.webmanifest
├── favicon.ico
├── package.json
├── LICENSE
└── .gitignore
```

## Run it locally / in Codespaces

1. Open this repo in **GitHub Codespaces** (or clone it and open in VS Code).
2. The dev container installs dependencies automatically on first boot.
3. Start the preview server:
   ```bash
   npm start
   ```
4. Codespaces will pop up a forwarded-port preview automatically on port `3000`. Locally, open `http://localhost:3000`.

No Node experience needed — you can also just right-click `index.html` and choose **"Open with Live Server"** if you're using the VS Code extension (already recommended in the dev container).

## Push this to GitHub (create the repo)

You'll need to create the GitHub repo yourself (from github.com or the `gh` CLI) — here's the fastest path:

```bash
# 1. Unzip the download, then from inside the ayuverse folder:
git init
git add .
git commit -m "Initial commit: AyuVerse home page"

# 2. Create the repo on GitHub (pick ONE option):

# Option A — using GitHub CLI (if installed)
gh repo create ayuverse --public --source=. --remote=origin --push

# Option B — manually
# Go to github.com/new, create a repo named "ayuverse" (don't add a README there),
# then run:
git branch -M main
git remote add origin https://github.com/<your-username>/ayuverse.git
git push -u origin main
```

## Deploy for free (GitHub Pages)

1. In your new repo on GitHub: **Settings → Pages**.
2. Under "Build and deployment", set **Source** to **GitHub Actions**.
3. Push to `main` — the included workflow (`.github/workflows/deploy.yml`) builds and deploys automatically.
4. Your site will be live at `https://<your-username>.github.io/ayuverse/`.

## Before you go live — a few placeholders to swap

- `hello@ayuverse.com` — appears in `index.html` and the footer of every page. Search for `TODO` comments and replace with your real email.
- The GitHub link in the footer (`https://github.com/`) — point it at your actual profile or repo.
- `LICENSE` — MIT license is applied to the **code**. If you want different terms for the actual study content you add later (notes, PDFs, etc.), that's a separate decision worth making explicitly.

## Roadmap

- [x] Home page
- [x] Site-wide design system, favicon/icons, mobile nav
- [ ] Physics hub (notes, PYQs, tests)
- [ ] Mathematics hub
- [ ] Chemistry hub
- [ ] Resources library page

---

Built with plain HTML, CSS, and JavaScript — no framework, no build step.
