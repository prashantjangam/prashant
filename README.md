# JANGAME Portfolio — Netlify Deployment

## Deploy in 60 seconds

### Option 1: Drag & Drop (Fastest)
1. Go to https://app.netlify.com
2. Log in (or create a free account)
3. On the dashboard, find the **"Deploy manually"** box at the bottom
4. Drag the entire **`jangame-site`** folder into that box
5. Done — your site is live at a random `.netlify.app` URL

### Option 2: Netlify CLI
```bash
npm install -g netlify-cli
cd jangame-site
netlify deploy --prod --dir .
```

### Option 3: GitHub + Auto-Deploy
1. Push this folder to a GitHub repo
2. In Netlify dashboard → "Add new site" → "Import from Git"
3. Select your repo
4. Set **Publish directory** to `.` (root)
5. Click Deploy — every push auto-deploys

## Custom Domain
In Netlify dashboard → Site settings → Domain management → Add custom domain → enter `jangame.org`

## Files
- `index.html` — the full portfolio (self-contained, no build step needed)
- `netlify.toml` — Netlify config (headers, redirects, caching)
- `_redirects` — fallback redirect rules
