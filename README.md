# FinancialGodun

Offline-first personal wealth planning app — single HTML file, no backend, no build step. Runs entirely in your browser; your data stays in local storage on your device.

## Running it locally

Just double-click `index.html`, or open it directly in any modern browser. No server required.

## Auto-deploying to GitHub Pages

This repo includes `.github/workflows/deploy.yml`, which automatically publishes `index.html` to GitHub Pages every time you push to `main`.

**One-time setup:**

1. Push this repo to GitHub (create a new repo if you haven't already, then `git push`).
2. In your repo, go to **Settings → Pages**.
3. Under **Build and deployment → Source**, choose **GitHub Actions** (not "Deploy from a branch").
4. That's it — push to `main` and the workflow in the **Actions** tab will run automatically and publish your site. It usually takes 1–2 minutes.
5. Your live URL will be `https://<your-username>.github.io/<repo-name>/`, shown at the top of Settings → Pages once the first deployment finishes.

**Every future update:** just commit and push your changes to `main` — no manual deploy step needed.

**Manual trigger:** if you ever want to redeploy without a new commit (e.g., after changing a GitHub Pages setting), go to the **Actions** tab → **Deploy to GitHub Pages** → **Run workflow**.

## If your browser shows an old version after deploying

GitHub Pages (and your browser) can cache aggressively. Two things to try:

1. **In the app:** go to **Settings → App Version & Cache → Force refresh app**. This clears cached app files/service workers and reloads — it does *not* touch your saved financial data.
2. **In your browser:** a hard refresh (Ctrl+Shift+R / Cmd+Shift+R) usually resolves it if the app-level refresh doesn't.

Deployments also aren't instant — check the **Actions** tab to confirm the latest run finished (green checkmark) before assuming the update didn't go out.
