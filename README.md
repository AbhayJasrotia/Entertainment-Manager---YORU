# YORU 夜
A personal anime, movie and series tracker. Plain HTML, CSS and JavaScript. No build step, no backend, no API keys.

## Run locally
Open `index.html` in a browser, or run `python3 -m http.server` in this folder and visit http://localhost:8000.

## Deploy to GitHub Pages
1. Create an empty repository on GitHub (for example `yoru`).
2. In this folder run:
```
git init
git add .
git commit -m "YORU"
git branch -M main
git remote add origin https://github.com/USERNAME/yoru.git
git push -u origin main
```
3. In the repository go to Settings → Pages, choose "Deploy from a branch", pick `main` and `/ (root)`, and save.
4. Your app appears at `https://USERNAME.github.io/yoru/` after a minute. Routing uses `#/page` URLs, so refresh and relative paths work on project sites.

## Notes
- Data lives in your browser's localStorage on one device. It doesn't sync. Use Settings → Export backup regularly.
- Reminders show inside the app only. No notifications are sent when the browser is closed.
- Posters are optional links you paste into a title. Without one, YORU draws a fallback cover.

## Customize
- Name and title: `index.html` and the `.brand` element in `app.js` (`render`).
- Colors and spacing: CSS variables at the top of `styles.css`. Accent swatches are in `V.settings`.
- Demo data: the `demo()` function in `app.js`. Users can also remove it from Settings.
