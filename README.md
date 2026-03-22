# Protein Tracker

A personal protein tracking web app — designed to live on your iPhone home screen.

## Features

- **Daily progress ring** — visual goal tracking with a 135–155g target range
- **Manual entry** — log any food by name and grams instantly
- **Quick-add chips** — one-tap logging for your most common foods
- **Saved meals** — store go-to combinations (e.g. "Banana Yogurt Bowl") for one-tap logging
- **AI logging** — describe what you ate in plain English and Claude interprets it, asks one follow-up if needed, and logs an estimate
- **Honest estimates** — approximate values are marked with `~` so you always know what's exact vs. estimated
- **History** — past days with progress bars, expandable entry lists
- **Settings** — update your protein goal, manage your API key, export/restore data

## Setup

### 1. Host it
Upload `index.html` and `icon.png` to a public GitHub repo and enable GitHub Pages under **Settings → Pages**.

Your app will be live at:
```
https://yourusername.github.io/protein-tracker
```

### 2. Add to iPhone home screen
1. Open the URL in **Safari** on your iPhone
2. Tap the Share button (⬆️)
3. Tap **Add to Home Screen**
4. Tap **Add**

### 3. Set up AI logging (optional)
AI-powered food logging requires a free Anthropic API key.

1. Get a key at [console.anthropic.com](https://console.anthropic.com)
2. Open the app → tap ⚙️ Settings → API Key
3. Paste your key and save

Your key is stored only on your device — it is never sent to GitHub or anyone else.

## Data & Privacy

- All data (logs, meals, goals) is stored in your browser's `localStorage` — it never leaves your device
- GitHub only hosts the app code, not your data
- To back up your history: Settings → Export & Backup → Share

## Tech

Plain HTML/CSS/JS — no frameworks, no build step, no server. The only external dependency is the Anthropic API for the optional AI logging feature.
