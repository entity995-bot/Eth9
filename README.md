# ether9* — Android-ready PWA starter

This is the first installable web-app prototype for ether9*. It is a static Progressive Web App (PWA), designed for mobile screens.

## What works now
- Responsive dark dashboard and module navigation
- Capability tracker with locally saved levels
- Development journal with locally saved entries
- SoundLab idea notes
- App Studio module proposals
- Offline app shell after first successful load

## What is not connected yet
- No live AI model or chat backend
- No cloud database or cross-device synchronization
- No real autonomous agents, code deployment, financial accounts, or physical-device control

Data is stored in the browser's local storage on the device. Clearing browser/site data can erase it. Export/backup and cloud sync should be added before relying on it for important records.

## Publish it so Android can install it
A PWA must be served over HTTPS (or localhost) for installation and service-worker support.

1. Upload the contents of this folder to a static host such as GitHub Pages, Netlify, or Cloudflare Pages.
2. Open the resulting HTTPS address in Chrome on your Android phone.
3. Open Chrome's menu (⋮) and choose **Install app** or **Add to Home screen**.
4. Confirm. The ether9* icon will appear on your home screen.

## Local preview
For a quick desktop preview, run a local static server from this folder, for example:
`python -m http.server 8000`
Then open `http://localhost:8000` on that computer. For phone installation, use a public HTTPS deployment.

## Next engineering steps
1. Add secure backend authentication and encrypted cloud storage.
2. Add a real AI conversation endpoint without exposing API keys in browser code.
3. Add export/import and backup/restore.
4. Add module sandboxing, tests, approval gates, audit logs, and rollback.
5. Deploy updates through a controlled release process.
