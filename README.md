# F.I.R.S.T. STEP — Leadership Pilot Dashboard (Deployable Bundle)

Zero-dependency static web application ready for instant hosting on **Netlify**, **Vercel**, **GitHub Pages**, **Cloudflare Pages**, or internal SharePoint/intranet hosting.

## Files Included
- `index.html` — Complete self-contained dashboard (HTML, CSS, JS, and baseline cohort data).
- `vercel.json` — Security headers and cache rules for Vercel.
- `netlify.toml` — Publish configuration and security headers for Netlify.

## 1-Minute Deployment Options
1. **Netlify Drop:** Drag and drop this folder onto [app.netlify.com/drop](https://app.netlify.com/drop).
2. **Vercel CLI:** Run `npx vercel --prod` inside this folder.
3. **GitHub Pages:** Push these files to a repository and enable **Settings → Pages → Deploy from branch (`main` / root)**.

## Connecting Live Master Tracker Data (No Backend Needed)
1. Open your Google Sheet (`FIRST-STEP-Master-Tracker`) and go to **File → Share → Publish to web**, select the tracker sheet and **Comma-separated values (.csv)**, and copy the URL.
2. In the deployed dashboard, click **Data sync** in the top bar and paste the CSV URL—or share the dashboard link with `?csv=YOUR_ENCODED_CSV_URL` appended so every leadership viewer automatically sees the latest tracker state.
3. Alternatively, use **Data sync → Import Master Tracker CSV from disk** to load any exported CSV offline.
