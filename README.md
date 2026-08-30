# EPSS Warehouse Logistics Dashboard — GitHub-ready PWA

This is the final PWA package. The full dashboard application is inside `index.html`; it is not an iframe shell.

## Files
- index.html
- manifest.json
- service-worker.js
- icons/icon-192.png
- icons/icon-512.png
- README.md

## Deploy
1. Open the GitHub repository for the EPSS dashboard.
2. Replace its `index.html` with this package's `index.html`.
3. Upload `manifest.json`.
4. Upload `service-worker.js`.
5. Upload the `icons` folder.
6. Commit and push.
7. Open the GitHub Pages HTTPS address in Chrome on Android.
8. Choose Install app / Add to Home screen.

## Supabase security
The browser uses the existing publishable/anon key. Never put a Supabase service-role/secret key in frontend code.
Use Supabase Auth and Row Level Security (RLS) to protect writes and administrative operations.

## Important
The app remains connected to the live Supabase database. PWA installation does not make Supabase data operations work without internet.
