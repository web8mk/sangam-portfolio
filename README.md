# Sangam's Developer Portfolio — GitHub Pages Deployment

This folder contains the complete, standalone static build of Sangam's Developer Portfolio website. It is fully pre-compiled and ready to be hosted on **GitHub Pages**, **Netlify**, **Vercel**, or any static web host.

---

## What is in this folder?

- `index.html` — Main website entry point with SEO metadata and Open Graph tags.
- `404.html` — Fallback page for single-page routing on GitHub Pages.
- `.nojekyll` — Bypasses Jekyll processing on GitHub Pages to ensure all assets load reliably.
- `favicon.svg` — Custom monogram favicon for Sangam.
- `assets/` — Production-compiled, minified JavaScript bundle and CSS styles.
- `landmark/` — Authentic image assets for the Hotel Landmark Premier featured project showcase.

---

## How to Deploy to GitHub Pages (2 Methods)

### Method 1: Using GitHub Web UI (Easiest — No Git commands needed)

1. **Create a GitHub Repository**:
   - Go to [GitHub](https://github.com/) and click **New repository**.
   - Name it `portfolio` (or `<your-username>.github.io`).
   - Choose **Public**.
   - Click **Create repository**.

2. **Upload the Files**:
   - On the new repository page, click **uploading an existing file**.
   - Open this `portfolio-deploy` folder on your computer.
   - **Select all files and folders inside `portfolio-deploy`** (i.e., `index.html`, `404.html`, `.nojekyll`, `favicon.svg`, `assets`, and `landmark`).
   - Drag and drop them into the GitHub upload area.
   - Wait for the upload to complete, enter a commit message like `"Initial portfolio release"`, and click **Commit changes**.

3. **Enable GitHub Pages**:
   - In your repository, go to **Settings** → **Pages** (in the left sidebar).
   - Under **Build and deployment** > **Source**, select **Deploy from a branch**.
   - Under **Branch**, select `main` (or `master`) and folder `/ (root)`.
   - Click **Save**.
   - Within 1–2 minutes, GitHub will display your live website URL (e.g., `https://<your-username>.github.io/portfolio/`).

---

### Method 2: Using Git Terminal (Command Line)

Run these commands inside the `portfolio-deploy` folder:

```bash
cd "portfolio-deploy"
git init
git add .
git commit -m "Deploy Sangam's Developer Portfolio"
git branch -M main
git remote add origin https://github.com/<your-username>/<your-repo-name>.git
git push -u origin main --force
```

Then enable Pages in **Settings → Pages** with branch `main` and folder `/ (root)`.
