# Version 2 — Daily Build Tracker

Personal habit tracker for installing **Version 2 of me**. One page, no accounts, no dependencies. Data stays in the browser (localStorage).

**Live app:** `https://YOURUSERNAME.github.io/version-2/` *(replace with your username after enabling Pages)*

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

## Setup

1. Upload `index.html` and `README.md` to this repo
2. **Settings → Pages** → Source: `main` branch, root → Save
3. Open the live URL on your phone → Share → **Add to Home Screen**

## Features

- **Rank ladder** — consistency moves you from Baseline to **Top 2%** (v2.00 at 400 pts)
- **Hero ring** — four pillar arcs close around your version number as the day completes
- **Metrics with sparklines** — log weight, HRV, sleep, screen time against your targets
- **Badges** — streaks, perfect days, floor saves, habit swaps
- **Weekly audit tab** — reads your last 7 nightly notes, commit habit swaps
- **Rank-up celebrations** with confetti

## Notes

- Data is stored locally in your browser per device. Clearing browser data resets progress.
- Everything is in one `index.html` — edit habits, colors, or point values directly in the file.

## Family: Dawut's Daily Bloom 🌱

`dawut.html` is a companion app for tracking our son's development (born 13 March 2024). Now a **PWA** — installable to home screen, works offline.

### Daily activities
- Auto-computes his age and serves stage-appropriate daily activities (6 domains: Body, Brain, Language, Heart, Food, Create)
- Activities rotate daily from a research-informed roadmap (14–48 months); shuffle button if one doesn't fit today
- Progress ring shows today's completion at a glance

### Mama's Daily Plan tab
- **Daily routine** — 3 time blocks (Morning 07-10, Midday 10-14, Evening 16-20) with 16 checkable activities, each with a research-based explanation
- **Weekly focus goals** — 12-week progressive cycle, each week targets one skill area (language, balance, empathy, pre-math, memory, etc.); current week highlighted
- **Skill ladder** — 27 developmental skills from 12-48 months, showing done/current/future status based on Dawut's age, so Mama always knows what's next
- **Peer benchmarks** — 12 typical development milestones with CDC/WHO typical ages; shows if Dawut is ahead, on track, or approaching each milestone

### Growth tracking (WHO Child Growth Standards)
- Height, weight, and head circumference logged with **real WHO LMS percentile calculation** (not approximate)
- Growth charts with **P3/P15/P50/P85/P97 percentile bands** — see exactly where he falls on the curve
- His data plotted as a green line over the WHO reference bands

### Sleep tracking (AAP guidelines)
- Log nightly sleep hours; AAP recommends **11–14h for ages 1–3**
- Weekly bar chart with color-coded compliance (green/amber/red)

### Screen time tracking (AAP guidelines)
- Log daily screen minutes; AAP recommends **≤60 min/day for ages 2–5**
- Weekly bar chart with color-coded compliance

### Language development
- Word tracker — log new words as he learns them
- Milestone markers: 50 words (~18mo), 100, 200 (~24mo), 500 (~30mo)

### CDC developmental milestones (2022 update)
- Official CDC checklist for 15mo, 18mo, 2yr, 30mo, 3yr
- Check off each milestone as achieved; only shows age-relevant groups

### Vaccination schedule (Japan routine immunizations)
- Full Japan schedule: BCG, HepB, Rotavirus, DTaP-IPV/Hib, PCV, MR, DT, OPV, Japanese encephalitis
- Tap to mark done; shows Due/Upcoming/Done status; badge count on nav

### Milestone journal
- Save first words, first jumps, sweet moments with **photo attachments**
- Delete milestones; all data exportable

### Other features
- **Dark mode** — auto-detects system preference, manual override
- **PWA** — manifest.json + service worker for offline use and home-screen install
- **Accessibility** — ARIA labels, keyboard navigation, focus states, reduced-motion support
- Consistency garden (GitHub-style heatmap), streak tracking, confetti celebrations
- Browser notifications for morning/evening reminders
- Auto-backup reminder (7-day interval)
- Export/import full data backup (JSON)
- Schema versioning for safe data migrations
- Live at: `https://YOURUSERNAME.github.io/version-2/dawut.html`
