# LifeSync

Single-file daily planner PWA — Bengali UI, roster/shift timeline, gym/food/study/money trackers, prayer times, reminders.

## Files

- `index.html` — app entry (identical to `lifesync.html` for legacy paths)
- `lifesync.html` — same app content (service worker `openWindow` target)
- `sw.js` — service worker (`lifesync-v3`, cache-first app shell)

## Run locally

```powershell
python -m http.server 8000 --bind 127.0.0.1
# open http://127.0.0.1:8000/lifesync.html (or /index.html)
```

Service worker requires `http://` or `https://` (not `file://`).

## Deploy

Static site — drag to Vercel (`vercel --prod`) or Netlify.
