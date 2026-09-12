# Proverbs Study Group App

A single-file, 31-day group study of the Book of Proverbs — one chapter per day (the day of the month = the chapter).

## Deploy to Netlify

### Option 1: Drag & Drop
1. Download `index.html`.
2. Go to https://app.netlify.com/drop
3. Drag the file onto the page. Done — you get a live URL instantly.

### Option 2: Git Deploy
1. In Netlify: **Add new site → Import from Git**.
2. Select this repo. Build command: (leave blank). Publish directory: `.`
3. Deploy.

## Features
- **Sign Up & Begin** — name + email signup stored locally, then straight into today's study
- Create a study group with members (entered manually — web apps cannot access phone contacts)
- Assign a study leader
- Select 31-day study months (Jan, Mar, May, Jul, Aug, Oct, Dec)
- Bible versions: NKJV, KJV, ESV, NIV, NLT
- Link out to Bible Gateway, Bible Hub, and YouVersion for the day's chapter
- Three daily reflection questions with a per-reflection "Share with group" toggle
- Shared reflections feed + private reflections
- Leader tools: encouragement/accountability messages to the group or individuals
- Browser daily reminders via the Notification API

## Limitations (static app)
- No phone contacts access or real SMS (requires a native mobile app).
- Data is stored per-device in `localStorage` (no cloud sync). For real cross-device group sharing, add a backend such as Firebase or Supabase.
