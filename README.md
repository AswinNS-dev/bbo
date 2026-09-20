# 2V2 Skirmish Showdown – Tournament Bracket

Interactive tournament bracket web application for the **2V2 Skirmish Showdown**.

## Features
- **32-Team Single Elimination Bracket** with dynamic round-by-round path progression.
- **Interactive Match Winner Selection** (click to advance, click again to undo).
- **Auto State Persistence** via browser `localStorage` (picks are preserved across page reloads).
- **Shareable URL Bracket State** (`#b=...` permalinks) allowing players & organizers to share bracket predictions.
- **Safe Reset Confirmation** so tournament picks are not accidentally erased.
- **Fast, Zero-Build Static Web App** with zero external dependencies (pure HTML, CSS, JavaScript).

---

## Deploy to Vercel (Ready Out-of-the-Box)

This repository is pre-configured for Vercel deployment via `vercel.json` and standard `index.html`.

### Option 1: Deploy with Vercel CLI
```bash
npx vercel
```
Follow the interactive prompts (select defaults by pressing Enter). Your tournament bracket will be live in seconds with a free `.vercel.app` URL.

### Option 2: Deploy via GitHub / Git
1. Push this folder to a GitHub repository:
   ```bash
   git init
   git add .
   git commit -m "Initial tournament bracket"
   git branch -M main
   git remote add origin https://github.com/your-username/your-repo.git
   git push -u origin main
   ```
2. Go to [vercel.com/new](https://vercel.com/new).
3. Import the repository and click **Deploy**.
4. Vercel automatically detects the static HTML project and deploys it instantly.

### Option 3: Drag & Drop
You can also drag and drop this project folder directly onto the [Vercel Dashboard](https://vercel.com/).

---

## File Structure
- `index.html` — Main production entry point for Vercel and web browsers.
- `2v2-skirmish-showdown-bracket.html` — Synchronized alternate entry point.
- `favicon.svg` — Esports tournament trophy icon.
- `vercel.json` — Vercel configuration with clean URLs, security headers, and rewrites.
