# Proverbs Study Group App

A 31-day group study of the Book of Proverbs — a single-file web app (`index.html`) you can deploy to Netlify in seconds.

## Deploy to Netlify

### Option 1: Drag & Drop
1. Download `index.html` (rename it `index.html` if your browser saved it differently).
2. Go to https://app.netlify.com/drop
3. Drag the file (or this folder) onto the page.
4. Done — you get a live URL instantly.

### Option 2: Git Deploy (recommended — auto-redeploys on every push)
1. In Netlify: **Add new site → Import an existing project → Deploy with GitHub**.
2. Select this repo (`itsnotmarquez/proverbs-study-app`).
3. Build command: *(leave blank)*. Publish directory: `.` (or `/`).
4. Deploy.

The included `netlify.toml` sets the publish directory and adds basic security headers — no other configuration needed.

## Features
- User signup (stored locally in the browser)
- Create a study group with members (entered manually) and a leader
- Select 31-day months (Jan, Mar, May, Jul, Aug, Oct, Dec)
- Choose Bible version (NKJV, KJV, ESV, NIV, NLT)
- Daily chapter links out to Bible Gateway, Bible Hub, and YouVersion
- Daily 3-question reflections with per-question "Share with group" toggles
- Shared reflections view for the group
- Leader messaging to the whole group or individuals
- Browser-based daily reminders via the Notification API

## Limitations (Static App)
- Cannot access phone contacts (that requires a native mobile app) — members are entered manually.
- Data is stored per-device in `localStorage` (no cloud sync).
- Messages are simulated locally (no real SMS/push to other devices).

For a full production version, consider:
- Firebase or Supabase for real accounts and cross-device sync
- A native wrapper (React Native / Flutter) for contacts and push
- Twilio for real SMS reminders
