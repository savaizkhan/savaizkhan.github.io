# Muhammad Savaiz Khan — Portfolio

A responsive, dark-themed single-page portfolio website built with React + TypeScript + Vite.

## Live URL

🔗 [https://muhammadsavaizkhan.tech/](https://muhammadsavaizkhan.tech/)

## Tech Stack

- **Framework:** React 18 + TypeScript (strict mode)
- **Bundler:** Vite
- **Styling:** CSS Modules
- **Fonts:** Plus Jakarta Sans (headings) + Manrope (body) via Google Fonts
- **Deployment:** GitHub Pages via GitHub Actions

## Setup

```bash
# Install dependencies
npm install

# Start dev server
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview
```

## Project Structure

```
src/
  components/       # All 8 section components
  data/
    portfolio.ts    # Single source of truth — all CV data
  assets/
  App.tsx
  main.tsx
public/
  cv.pdf            # CV file for download
.github/
  workflows/
    deploy.yml      # GitHub Pages deployment workflow
```

## Deployment

`pages-build-deployment` runs first, then `.github/workflows/deploy.yml` publishes the Vite `dist` artifact to GitHub Pages so production always serves compiled assets.
The published domain is configured via `CNAME`/`public/CNAME` as `muhammadsavaizkhan.tech`.
In GitHub Pages settings, keep **Custom domain** set to `muhammadsavaizkhan.tech` and enable **Enforce HTTPS** after DNS is pointed to GitHub.
