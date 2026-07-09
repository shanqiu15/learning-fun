# ABC & 123 Fun! 🐻

A cute, tap-and-listen learning app for a 3-year-old — the whole app is one file: `index.html`.

## Activities

- **🅰️ Letters** — Big rainbow flash cards A–Z. Tap the card to hear "A! A is for Apple!". Includes a "Find the letter" game (with a 🔠 ABC / 🔡 abc toggle for upper- or lowercase answers) and ✏️ finger tracing.
- **🔢 Numbers 0–20** — See the numeral, hear its name, and tap each object one-by-one to count out loud. Includes a "How many?" game (with tappable objects to count) and ✏️ number tracing. A 🔊 I count / 🤫 You count toggle mutes the count-along voice so she can count by herself.
- **🧮 Math** — Picture addition and take-away within 10, with three answer buttons.
- **✏️ Tracing** — Scribble over a big dashed letter or number with rainbow finger-paint; when it's mostly colored in, she gets a star and the next one appears.

Every correct answer earns a ⭐ (saved between sessions), plus confetti and a spoken cheer. Wrong answers get a gentle "Almost! Try again!" — nothing scary, no penalties.

## Put it on the iPad

iPadOS can't open a local HTML file in Safari, so the page has to be served over HTTP. The app is a PWA (`manifest.json` + `sw.js`), so once it's hosted on GitHub Pages, open the site in Safari and tap **Share → Add to Home Screen** — it installs with its own icon, launches full-screen like a real app, and keeps working offline after the first load.

For quick testing from a Mac on the same Wi-Fi: `python3 -m http.server 8000` in this folder, then visit `http://<mac-ip>:8000` on the iPad.

Tips:
- Turn on **Guided Access** (Settings → Accessibility) so she can't exit the app mid-play.
- Sound uses the iPad's built-in text-to-speech — make sure the mute switch/volume is on.

## Develop / test locally

Just open `index.html` in any browser. No build, no dependencies.
