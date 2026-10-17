# YORU 夜
A personal anime, movie and series tracker. Plain HTML, CSS and JavaScript. No build step, no backend, no API keys.

## How to Run
http://yoru-app.s3-website.ap-south-2.amazonaws.com

## Notes
- Data lives in your browser's localStorage on one device. It doesn't sync. Use Settings → Export backup regularly.
- Reminders show inside the app only. No notifications are sent when the browser is closed.
- Posters are optional links you paste into a title. Without one, YORU draws a fallback cover.

## Customize
- Name and title: `index.html` and the `.brand` element in `app.js` (`render`).
- Colors and spacing: CSS variables at the top of `styles.css`. Accent swatches are in `V.settings`.
- Demo data: the `demo()` function in `app.js`. Users can also remove it from Settings.
