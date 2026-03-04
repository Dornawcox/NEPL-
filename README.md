# NEPL — New England Polo League

A standalone web application for managing the New England Polo League: team registration, venue management, schedule generation with specific dates, game results with individual stats, and live standings.

## Features

- **8 Pre-loaded Venues** across MA, CT, RI, NH, and VT — with Indoor Arena, Outdoor, and Outdoor Arena facility types
- **10 Pre-loaded Teams** (low and medium goal) with full rosters and alternates
- **Full Season Schedule** — April through November 2027 with specific dates, game times, alternate dates, and round-robin weekends at single venues
- **Outdoor Rules** — No outdoor games before May 15 or after October 15
- **Game Results** — Final scores, chukker-by-chukker detail, MVP selection, and individual goal scorers per game
- **Pre-populated Results** — All games through June 30 have scores, MVPs, and goal scorers
- **Live Standings** — League table with W/D/L, goal difference, points, division tags, and recent form
- **Player Statistics** — Top scorers, MVP leaders, and goals-per-game leaderboards
- **Edit Game Details** — Change game times, dates, alternate dates, and venues
- **Contact Venues** — Email links to venue organizers directly from game cards
- **Persistent Data** — All data saved to localStorage

## Hosting on GitHub Pages

1. Create a new GitHub repository (e.g., `nepl-league`)

2. Upload the files:
   ```bash
   git init
   git add .
   git commit -m "NEPL League site"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/nepl-league.git
   git push -u origin main
   ```

3. Enable GitHub Pages:
   - Repository → **Settings** → **Pages**
   - Source: **Deploy from a branch**
   - Branch: **main**, folder: **/ (root)**
   - Save

4. Site goes live at `https://YOUR_USERNAME.github.io/nepl-league/`

## Local Development

No build step required. Open `index.html` in any browser:

```bash
open index.html
```

Or serve locally:

```bash
python -m http.server 8000
# visit http://localhost:8000
```

## Data Management

- **Reset All Data** — Clears everything and starts fresh
- **Restore Demo Data** — Reloads the 8 venues, 10 teams, full schedule, and pre-populated results
- All data lives in `localStorage` — does not sync between browsers/devices

## Tech

Single HTML file. No frameworks, no build tools. Google Fonts loaded externally. Designed for static hosting on GitHub Pages, Netlify, Vercel, or any web server.

## License

MIT
