# 👗 Memory Match — Fashion Edition

A tiny, fast web game: flip cards to match fashion items.  
Features **Women, Men, Accessories, Shoes** packs with real image links, **2-Player hot-seat**, **Countdown mode**, hints, shuffle, and local personal bests.

## ✨ Features

- 🎴 **Real photos** per card (fixed links)
- 🧩 **4 items per pack** (Women, Men, Accessories, Shoes) + **Mixed**
- 👥 **2-Player mode** (keep your turn on a match; swap on miss)
- ⏱️ **Modes**: Classic (count up) & Countdown
- 🪄 **Hint** power-up (briefly reveals a pair)
- 🔀 **Shuffle** remaining unmatched tiles
- ⭐ **Combo scoring** (+3 each consecutive match)
- 🥇 **Personal Bests** saved locally per *Level • Mode • Pack*
- 🌗 **Light/Dark theme**, keyboard support, vibrate feedback
- 📦 **No build tools** — a single `index.html`

## 🚀 Quick Start

Open `index.html` in any modern browser.

Or serve locally:

```bash
# Option A: Python
python3 -m http.server 5173
# visit http://localhost:5173

# Option B: Node (if you have http-server)
npx http-server -p 5173
```

## 🕹️ Controls

- Click / Tap a tile to flip
- **P** = pause/resume
- Dropdowns: category, level, mode
- Buttons: Restart, Shuffle, Hint, Pause, Theme
- 2P toggle to play hot-seat

## 🧱 Project Structure

```
fashion-memory-match/
├─ index.html     # the entire app
├─ README.md
├─ LICENSE
└─ .gitignore
```

## 🌐 Deploy to GitHub Pages

1. Create a new repo on GitHub (e.g. `fashion-memory-match`).
2. Push files:

```bash
git init
git add .
git commit -m "feat: initial release"
git branch -M main
git remote add origin https://github.com/<your-username>/fashion-memory-match.git
git push -u origin main
```

3. In GitHub: **Settings → Pages → Build and deployment**
   - Source: **Deploy from a branch**
   - Branch: **main** / **root**
4. Your site will appear at:  
   `https://<your-username>.github.io/fashion-memory-match/`

## 🔧 Configuration

All data lives inside `index.html`:

- **Catalog** (`CATALOG`): update `name`, `img`, `link` per item.
- **Levels** (`LEVELS`): tweak pairs, grid columns, countdown limits, hints.
- **Scoring** (`SCORE`): match/miss values, combo step, finish bonus.

## 🔒 Privacy

- Personal bests are saved in `localStorage` **on the device only**.
- No analytics, no external scripts.

## 🙏 Credits

- **Images**: Your linked images + Unsplash links per product.
- **Vibrate API**: standard navigator feature.
- No sound assets (intentionally removed).

## 📝 License

MIT © **Katlego Sambo** — see [LICENSE](./LICENSE).
