# Recovery notes

This project archive was missing the four non-football gameplay board components even though the live-game route imported them. It also linked to History, Trophy Room, Settings, and Results routes that were not implemented. Those missing pieces have been added here.

Implemented in this recovery:
- Added playable Desert Decision, Heritage Quest, Family Budget Blitz, and Logic Lab boards.
- Corrected live board rendering to mount the selected board as a React component.
- Added History, Trophy Room, Settings, and per-match Results pages.
- Added route-tree entries for the missing pages.
- Added JSON export and local-data reset controls in Settings.
- Updated the README with setup, data, and live-AI configuration notes.

Important: dependencies could not be installed in the working environment, so a full production build, browser QA pass, and live-AI request could not be executed here. Run `npm install`, `npm run build`, `npm test`, and `npm run lint` locally before submitting the competition project. Live AI also requires the server-side `LOVABLE_API_KEY`; prepared demo content remains available without it.
