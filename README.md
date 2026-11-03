# CyberZone Academy — B.Sc. Cybersecurity Semester IV

Desktop-first educational website, built with Vite, vanilla JavaScript, CSS and JSON.

## Run on your laptop

1. Install Node.js (LTS) if not installed.
2. Open a terminal in this folder.
3. Run `npm install` (internet needed the first time).
4. Run `npm run dev`.
5. Open the localhost URL printed in the terminal (usually http://localhost:5173/).

For production, run `npm run build` and serve the `dist` folder with a server that falls back to `index.html` for nested routes. The app uses clean History API URLs.

## Content

- Syllabus: `src/data/wireless.json`, `ethical.json`, `essentials.json`, `game.json`.
- Practicals: `src/data/practicals.json`.
- Official titles preserved; no study notes or practical answers were invented.
- Game Development has no syllabus units until supplied.
- Cyber Security Essentials is hidden from Practicals until official practicals are supplied.
- Notes content uses each topic's `content` array; practical details are intentionally blank.

## Navigation and preferences

- Icon-only fixed sidebar; light/dark theme stored in browser localStorage.
- Accordion states saved across refreshes.
- Back/forward navigation and in-session scroll restoration.
- Direct deep links work with the Vite dev server or an SPA-compatible production host.

## Implementation note

Inter loads via Google Fonts when online; local fallback is Arial. `npm run build` requires Vite dependencies installed.
