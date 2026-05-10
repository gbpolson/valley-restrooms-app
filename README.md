# Valley Portable Restrooms — Operations app (mockup)

Clickable demo of the Valley Portable Restrooms operations system. Static HTML — no backend wired yet.

## What's in here

- `index.html` — the full clickable mockup. Switch between Kim, Greg, Driver, and Customer views via the role toggle in the top-right.
- `valley_logo.png` — the Valley logo (sourced from valleyrestrooms.com).
- `vercel.json` — minimal Vercel config (clean URLs, basic security headers).

## Deploy to Vercel

### Option A — Vercel CLI (fastest, no GitHub needed)

From inside this folder:

```bash
npx vercel deploy --prod
```

Follow the prompts to log in (browser auth) and link to a project. You'll have a live `*.vercel.app` URL in ~30 seconds. Good for the demo, or anytime you want a quick public link.

### Option B — GitHub + Vercel (best for ongoing changes)

1. **Create a new repo** at https://github.com/new
   - Name: `valley-restrooms-app` (or whatever you prefer)
   - Keep it private if you want — Vercel works either way
   - Don't add README / .gitignore — we already have them

2. **Initialize and push** from this folder:

   ```bash
   git init -b main
   git add .
   git commit -m "Initial mockup"
   git remote add origin https://github.com/YOUR_USERNAME/valley-restrooms-app.git
   git push -u origin main
   ```

3. **Connect to Vercel:**
   - Go to https://vercel.com/new
   - Import the GitHub repo
   - Hit Deploy (no build config needed — Vercel auto-detects static)

After that, every `git push` to `main` redeploys automatically. This is the right setup for the actual project — every change to the mockup goes live within seconds.

### Option C — Drag and drop (no CLI, no git)

If you just want a quick demo URL with zero setup:

1. Go to https://vercel.com/new
2. Drag this entire folder onto the page
3. Done — you get a URL within seconds

You won't be able to push updates without re-uploading, but it's the fastest possible path for a one-shot demo link.

## Local preview

Open `index.html` in any browser, or run:

```bash
npx serve .
```

## Notes for the demo

- All data is hard-coded inside `index.html` for the demo. No real customer info, no real driver tracking, no real ba