# Photogram

A full-stack, Instagram-like social app built with **React + Express + SQLite**.

- Full source: see the `photogram.zip` delivered with the project (React frontend, Express API, SQLite database, seeded demo data)
- **Live demo:** https://mohitjatktp.github.io/photogram-demo/

## About the live demo

The live site is the static demo build. Since GitHub Pages only serves static files,
the app runs fully in your browser in **demo mode**:

- All features work: login, feed, likes, comments, stories, direct messages, profiles, follows, explore, dark mode
- Demo login: **mohit / password123** (or create your own account)
- Your posts, likes and messages are saved in your browser's local storage only — they never leave your device
- No other users are real; the seeded users are demo data

The full multi-user backend (Express + SQLite) is in the source zip — run it locally
with `npm install && npm run seed && npm start`, or deploy it to any Node host
(Render, Railway, Fly.io, Replit).

## Updating the demo site

1. Build the client: `cd client && npm run build`
2. Zip the contents of `client/dist` as `photogram-dist.zip`
3. Attach it to the `demo` release

The `publish` workflow unpacks the zip and pushes it to the `gh-pages` branch.
