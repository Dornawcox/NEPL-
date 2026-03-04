# NEPL — New England Polo League (v6)

Club team polo league platform with multi-season support, game-day resource management, and a chukker scheduling tool.

## What's New in v6

- **Multi-Season Support** — Season selector bar on schedule and standings pages. Create and switch between seasons. Data scoped per season.
- **Game Day Resources Tab** — Sign up as umpire, timekeeper, third man, announcer. Provide umpire horses or spare horses for visiting players. Resource dashboard shows coverage gaps across upcoming games.
- **Spare Horse Board** — Per-game listings where horse owners can offer mounts for visiting players with terms (free/fee/reciprocal).
- **Resource Needs Alerts** — Visual indicators when games are missing required resources (umpire, timekeeper, umpire horse).
- **Chukker Scheduler** — Standalone practice tool (`NEPL_Chukker_Scheduler.html`). Enter players with handicaps and horse counts, set format (3v3/4v4) and balance style, generate a printable chukker chart.

## Files

- `index.html` — Main NEPL league site
- `NEPL_Chukker_Scheduler.html` — Standalone chukker scheduling tool
- `.nojekyll` — GitHub Pages config

## Deploy to GitHub Pages

```bash
git init && git add . && git commit -m "NEPL v6"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/nepl-league.git
git push -u origin main
```

Settings → Pages → main branch → / (root) → Save

## Supabase Migration Path

This frontend is architected for migration to Supabase + Next.js:
- All data access goes through a centralized state/save layer (currently localStorage)
- Role concepts (Admin, Venue Manager, Team Captain, Player) are reflected in the UI
- Resource sign-up workflows mirror the confirmation model described in the Platform Recommendation doc
- Season scoping is built into the data model

The next step is to replace `localStorage` calls with Supabase client SDK calls and add real authentication.
