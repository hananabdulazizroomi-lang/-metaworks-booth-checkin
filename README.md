# Metaworks Booth Check-in

A single-page check-in app for trade show booths. Collects visitor info and generates a personalized welcome message via Claude AI.

## Features

- Splash screen with brand identity
- 3-step form: name, email, phone, interest
- AI-generated personalized welcome message (Claude)
- Staff view (5 rapid taps on splash) with CSV export
- Works offline — data saved to localStorage
- Mobile-first responsive design

## Setup

1. Open `index.html` in a browser or deploy to any static host
2. Edit the `CONFIG` object in the `<script>` tag to customize:
   - `STARTUP_NAME` / `STARTUP_PITCH` / `CLOSING_LINE`
   - `INTEREST_OPTIONS` for booth-specific categories
3. For Claude AI integration, add your API key to the `generateMessage()` function

## Deploy to GitHub Pages

```bash
git init && git add . && git commit -m "Initial commit"
# Create repo on GitHub, then:
git remote add origin <your-repo-url>
git push -u origin main
# Enable Pages in repo Settings → Source → main branch
```

## Staff View

Tap the splash screen 5 times quickly to access the staff dashboard. Export all captured leads as CSV.
