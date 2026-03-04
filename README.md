# NEPL — New England Polo League

Club team polo league management — teams, venues, schedule, results, standings, and stats.

## What's New in v5

- **Edit Teams and Venues** — Click the pencil icon on any team or venue card to edit all fields
- **Team and Venue Logos** — Emoji-based logos displayed on cards, standings, and stats. Choose from 30+ icons during registration or editing
- **Stats Tab with Sub-tabs** — Defaults to **Team Stats** (per-team cards with win rate, goals/game, conceded/game, form streak) with a **Player Stats** sub-tab for individual scoring and MVP leaderboards
- **Full November Schedule** — Games run through the last Saturday of November (indoor arena for the final month)

## Features

- 8 venues across MA, CT, RI, NH, VT with Indoor Arena / Outdoor / Outdoor Arena facility types
- 10 teams (low + medium goal) with full rosters and alternates
- April–November schedule with specific dates, times, alternate dates, round-robin weekends
- No outdoor games before May 15 or after October 15
- Game results with chukker-by-chukker scores, MVP selection, individual goal scorers
- Pre-populated results through June 30
- Live standings with division tags and recent form
- All data in localStorage with Reset and Restore Demo buttons

## Deploy to GitHub Pages

```bash
git init
git add .
git commit -m "NEPL v5"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/nepl-league.git
git push -u origin main
```

Settings → Pages → Deploy from branch → main → / (root) → Save

Live at: `https://YOUR_USERNAME.github.io/nepl-league/`

## Local

Just open `index.html` in a browser. No build step needed.
