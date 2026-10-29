# Family AI Game Day

A dark, responsive family game web app with five original games, local player profiles, live scoring, saved match history, trophies, and settings.

## Run locally

Requirements: Node.js 20+ and npm.

```sh
npm install
npm run dev
```

Open the local URL printed by Vite.

## Build and checks

```sh
npm run build
npm test
npm run lint
```

## Live AI

The app includes clearly labelled prepared demo content, so games can still be played without live generation. Live AI generation is handled on the server through the Lovable AI Gateway and requires `LOVABLE_API_KEY` to be configured as a **server-side environment secret** in the deployment environment. Never place the key in client-side code or commit it to GitHub. When the secret is missing or the provider is unavailable, use the prepared demo content.

## Data and privacy

Player profiles, teams, preferences, session history, and achievements are stored in the browser's local storage on that device. Use **Settings → Export backup** to save a JSON backup. Clearing browser storage or switching devices will not automatically move this data.

## Included game modes

- **Football Challenge:** match timer, goals, undo, missions, and trivia.
- **Desert Decision:** team choices, resource costs, consequences, and scoring.
- **Heritage Quest:** host-confirmed cultural questions, answer explanations, and a timer.
- **Family Budget Blitz:** essentials and optional purchases, live totals, budget scoring.
- **Logic Lab:** puzzles, hints, answer reveal, and host-confirmed scoring.
