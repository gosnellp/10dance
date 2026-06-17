# 10Dance — Tap-to-track attendance

A single-file, client-side web app for tracking class attendance by tapping
name pills. Three states: **present** (green ✓), **tardy** (amber ◷),
**absent** (red ✕). The app detects the live class from your schedule and the
device clock, keeps running tallies, and surfaces a one-click policy-reminder
email when a student crosses the absence threshold.

- **No server, no login.** All data lives on your device (IndexedDB, with a
  `localStorage` fallback in file mode).
- **Privacy / FERPA.** Student records never leave the browser. Roster backups
  (which contain names and emails) are **never** committed to this repo — see
  `.gitignore`.
- **Stack.** Plain HTML/CSS/JS in `index.html`. No build step, no framework.

## Run it

Open `index.html` in Chrome, or visit the GitHub Pages URL.

## Hosting

Deployed on GitHub Pages from the `main` branch (root). Any push to `main`
updates the live site.
