# NEPL — New England Polo League

A standalone web application for managing the New England Polo League: team registration, venue management, automatic schedule generation, game results entry, and live standings.

## Features

- **Team Registration** — 3-person teams (low or medium goal) with up to 2 alternates. Players can come from different clubs.
- **Venue Registration** — Clubs register with arena/outdoor availability, location, and contact info.
- **Automatic Schedule Generation** — Full double round-robin (home & away) generated from registered teams. Games run simultaneously at multiple venues. Season spans April (indoor) through December (indoor), with outdoor play May–October.
- **Game Results** — Click any game to enter final scores, chukker-by-chukker detail, and game notes.
- **Live Standings** — League table with W/D/L, goal difference, points, and recent form. Plus top scorers and best defense leaderboards.
- **Persistent Data** — All data saved to `localStorage` in your browser.

## Hosting on GitHub Pages

1. **Create a new GitHub repository** (e.g., `nepl-league`)

2. **Upload the files:**
   ```bash
   git init
   git add .
   git commit -m "Initial NEPL site"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/nepl-league.git
   git push -u origin main
   ```

3. **Enable GitHub Pages:**
   - Go to your repo → **Settings** → **Pages**
   - Under "Source", select **Deploy from a branch**
   - Select **main** branch and **/ (root)** folder
   - Click **Save**

4. Your site will be live at `https://YOUR_USERNAME.github.io/nepl-league/` within a few minutes.

## Quick Start (Local)

Just open `index.html` in any browser. No build step, no dependencies, no server required.

```bash
open index.html
# or
python -m http.server 8000
# then visit http://localhost:8000
```

## How It Works

1. **Add venues** — Register the clubs that will host games
2. **Register teams** — Create teams with rosters, assign home venues
3. **Generate schedule** — The algorithm builds a full home-and-away round-robin
4. **Play and record** — Enter results as games are played; standings update automatically

## Data

All data is stored in your browser's `localStorage`. Use the "Reset All Data" button in the footer to start fresh. Data does not sync between browsers or devices.

## Tech

Single HTML file. No frameworks, no build tools, no external dependencies beyond Google Fonts. Designed to be dropped onto any static hosting platform.

## License

MIT
