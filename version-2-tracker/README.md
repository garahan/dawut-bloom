# Version 2 — Daily Build Tracker

Personal habit tracker for installing **Version 2 of me**. One page, no accounts, no dependencies. Data stays in the browser (localStorage). Real PWA — installable, works offline.

## The system

Four daily habits ("the Big 4"), each with a full version and a **Floor** — a tiny fallback for bad days that keeps the streak alive:

| Habit | Full | Floor |
|---|---|---|
| 🏋️ Move | Gym Day A/B, progressive overload | 1 set pushups + squats |
| 🥩 Fuel | ~168 g protein + small surplus | 1 protein meal |
| 💻 Build | Deep-work block on the product | 10 min / 1 commit |
| 🌙 Wind down | Phone out of bedroom, no late scroll | Just the phone rule |

**Rules:** Never miss twice. On bad days, do the Floor.

## Scoring

- Full habit = 1 pt · Floor = 0.5 pt · Perfect day = 4 pts
- Version counter: `v1.00 + total points / 400` → hit **v2.00** at 400 pts (~100 perfect days)
- GitHub-style heatmap = commit history of your days

## Features

### Today tab
- **Hero ring** — four pillar arcs close around your version number as the day completes
- **Habit cards** — tap to complete, floor button for bad days, expandable details
- **Mood check-in** — 5-level emoji selector with nightly reflection
- **Nightly note** — one bad habit today? one win?
- **Daily quote** — rotating motivation
- **Missed yesterday warning** — "never miss twice" reminder

### Progress tab
- **Overview stats** — streak, perfect days, total points, avg pts/day, consistency rate
- **Interactive heatmap** — tap any day to see full breakdown in a bottom sheet modal
- **Body & recovery metrics** — weight, HRV, sleep, screen time with area charts (gradient fills)
- **Insights engine** — most-skipped habit, best day of week, floor save rate, 7-day trend
- **Rank ladder** — consistency moves you from Baseline to **Top 2%** (v2.00 at 400 pts)
- **Badges** — streaks, perfect days, floor saves, habit swaps, version milestones

### Audit tab
- **Week at a glance** — perfect/floor/missed counts for last 7 days
- **Weekly notes review** — last 7 nightly notes with mood tags
- **Habit swap system** — name the trigger, replace the habit
- **Weekly goal** — set a target, track progress bar
- **Swap history** — permanent log of every habit swap

### Settings tab
- **Data export/import** — backup and restore as JSON
- **Accent color picker** — 8 colors to personalize
- **Habit editor** — customize names, icons, subtitles, details
- **PWA install** — add to home screen for full-screen experience
- **Reset** — clear all data (double confirmation)

### PWA
- **manifest.json** — installable on iOS/Android, standalone display
- **service-worker.js** — offline support, caches all assets
- **Installable** — "Add to Home Screen" or via browser prompt

## Deploy to Vercel

1. Push this repo to GitHub
2. Go to [vercel.com](https://vercel.com) → **New Project**
3. Import your GitHub repo
4. Vercel auto-detects the static site — no build command needed
5. Click **Deploy**
6. Open the live URL on your phone → Share → **Add to Home Screen**

## Project structure

```
├── index.html          # The entire app (HTML + CSS + JS)
├── manifest.json       # PWA manifest for installable app
├── service-worker.js   # Offline caching
├── vercel.json         # Vercel routing & cache config
├── .gitignore
└── README.md
```

## Notes

- Data is stored locally in your browser per device. Use Settings → Export to backup.
- Everything is in one `index.html` — edit habits, colors, or point values directly in the file or via Settings.
- No build step, no dependencies, no backend — pure static deployment.
- First-time visitors see an onboarding screen. Clear browser data to see it again.
