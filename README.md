# Roblox Break-even Calculator (Single-file MVP)

A static, single-page calculator for Roblox creators. No backend. Host it on GitHub Pages.

## Deploy on GitHub Pages (current steps)

**A) Web UI (no Git)**
1. Go to **https://github.com/new** → create a Public repo (e.g., `roblox-be-calc`).
2. Click **Add file → Upload files**. Drag **`index.html`** into the repo root. Commit.
3. Go to **Settings → Pages**.
4. Under **Build and deployment**, set **Source** to **Deploy from a branch**.
5. Set **Branch** to **`main`** and **Folder** to **`/ (root)`** → **Save**.
6. Wait ~30–60 seconds. Your URL will appear on that page, typically:
   `https://<your-username>.github.io/<repo-name>/`

**B) Git (CLI)**
```bash
git init roblox-be-calc && cd roblox-be-calc
# Add index.html here
git add index.html
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/<your-username>/roblox-be-calc.git
git push -u origin main
```
Then enable Pages as above.

## Swap in the full-feature file
- Replace this `index.html` with the full calculator you downloaded earlier (`roblox-break-even-mvp.html`), **renamed to** `index.html`.
- Commit/push, wait ~1 minute, hard-refresh.

## Troubleshooting
- **404/old page** → wait 1–2 min and hard refresh (Ctrl/Cmd+Shift+R).
- Must be `index.html` at repo root; case-sensitive.
- To add a custom domain later, use **Settings → Pages** and set a CNAME.