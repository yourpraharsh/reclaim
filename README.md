# Reclaim — Office Lost & Found

A two-sided lost & found for the office: employees report lost/found items,
security logs and verifies claims, and 3-month-old unclaimed items go to a
midnight charity auction (proceeds to education & environment NGOs).

## Host on GitHub Pages (no terminal needed)

1. On github.com click **New repository** → name it `reclaim` → Public → Create.
2. Click **uploading an existing file** → drag in `index.html` and `bundle.js` → Commit.
3. Go to **Settings → Pages** → Source: **Deploy from a branch** → Branch: `main`, folder `/ (root)` → Save.
4. In ~1 minute your app is live at `https://<your-username>.github.io/reclaim/`

## Or with git

```bash
git init && git add index.html bundle.js README.md
git commit -m "Reclaim lost & found"
git branch -M main
git remote add origin https://github.com/<your-username>/reclaim.git
git push -u origin main
```
Then enable Pages as in step 3 above.

## Notes on this hosted build

- Data is stored in each visitor's **browser (localStorage)** — not shared
  between people. Real multi-user data needs a small backend (Firebase/Supabase).
- The **AI photo match** only works inside the Claude artifact environment;
  on GitHub Pages it shows a graceful error. Search by details works fully.
- Click **Reset demo** in the header to load the seed items.
