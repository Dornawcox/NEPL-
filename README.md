# NEPL — New England Polo League

League management site and chukker scheduling tool for New England polo clubs.

## Files

| File | Purpose |
|------|---------|
| `index.html` | Main NEPL league site (teams, venues, schedule, results, standings, stats, game-day resources) |
| `NEPL_Chukker_Scheduler.html` | Standalone practice chukker scheduling tool |
| `.nojekyll` | Tells GitHub Pages to serve files as-is (no Jekyll processing) |

## Deploy to GitHub Pages

### Option A: Upload via GitHub.com (no git needed)

1. Go to [github.com/new](https://github.com/new) and create a repository (e.g., `nepl-league`)
2. Check "Add a README file" and click **Create repository**
3. Click **Add file → Upload files**
4. Drag all 4 files from this zip (`index.html`, `NEPL_Chukker_Scheduler.html`, `.nojekyll`, `README.md`) into the upload area
5. Click **Commit changes**
6. Go to **Settings → Pages**
7. Under "Source" select **Deploy from a branch**
8. Select branch **main** and folder **/ (root)**
9. Click **Save**
10. Wait 1–2 minutes. Your site is live at `https://YOUR_USERNAME.github.io/nepl-league/`

### Option B: Using git from the command line

```bash
# In the folder where you unzipped these files:
git init
git add .
git commit -m "NEPL league site"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/nepl-league.git
git push -u origin main
```

Then enable Pages in Settings as described above.

### Custom domain (optional)

To use a custom domain like `newenglandpolo.org`:

1. In your repo, go to **Settings → Pages → Custom domain**
2. Enter your domain and click Save
3. At your domain registrar, add a CNAME record pointing to `YOUR_USERNAME.github.io`

## Local use

Just open `index.html` in any browser. No server required.

## Data

All data is stored in your browser's localStorage. Click **Restore Demo Data** in the footer to reload the demo season with 10 teams, 8 venues, and pre-populated results.
