# Meridian Travel Advisory

Landing page for Meridian, a route-aware travel advisory app. The layout is inspired by philonet.ai.

## Sections

- Hero with a "Join the waitlist" button that expands into an email form
- Three-step account sign-up: account details, travel profile, confirmation
- Invite codes (format `MRD-1234`) skip the waitlist and activate the account
- Advisory level scale (Level 1 Normal precautions to Level 4 Do not travel)
- App previews: trip alert feed and destination brief
- Field Notes article grid
- Light and dark themes

## Run locally

It's a single static file with no build step:

```bash
open index.html
```

Or serve it:

```bash
python3 -m http.server 8000
```

## Notes

Sign-ups are saved in the browser's `localStorage`. When the page runs as a claude.ai artifact, it saves them to the artifact database instead. Connect a real backend (and email sign-in links) before using it in production.
