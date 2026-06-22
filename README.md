# FIT

A minimal, mobile-first workout app for a fat-loss + muscle-gain recomp. One static `index.html` — no build, no backend, no dependencies. Everything (plan, logs, theme) lives in your browser's `localStorage`.

**Live:** https://vasiroum.github.io/FIT/

Add to Home Screen on iOS/Android and it runs full-screen, offline, like a native app.

## Features

- **Plan** — a 7-day split (strength / boxing / pilates / kettlebell home day) with tappable, check-off exercises. Edit any day: rename, retag, add/delete exercises, change sets×reps. Checkmarks auto-reset every Monday.
- **Logging** — tap an exercise to log `weight × reps` with dated history, so progressive overload is tracked in-app instead of a notes app.
- **Guided morning primer** — an 11-step mobility + activation circuit. Hit **Start** and it runs hands-free in the timer: step name, countdown, auto-advance with a beep, screen stays awake.
- **Timer** — circular countdown with rest/round presets (incl. 3:00 boxing rounds) and ±15s adjust.
- **Targets** — daily protein / calorie / strategy reference.
- **Dark + light theme** — toggle persists; defaults to your system setting.

## Tech

Vanilla HTML/CSS/JS in a single file. Uses CSS variables for theming, the Web Audio API for beeps, the Wake Lock and Vibration APIs on mobile, and `localStorage` for persistence. iOS-style motion via `cubic-bezier(.32,.72,0,1)`.

## Develop

Just open `index.html` in a browser. To deploy changes:

```sh
git commit -am "your change"
git push
```

GitHub Pages redeploys automatically (~30s).
