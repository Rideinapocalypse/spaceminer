# ⭐ Space Colony — Idle Game

A pixel-art retro idle/clicker game built with pure HTML, CSS, and vanilla JavaScript. No frameworks, no dependencies — just one single HTML file.

![Space Colony](https://img.shields.io/badge/genre-idle%20clicker-blueviolet?style=flat-square)
![Tech](https://img.shields.io/badge/tech-HTML%20%2F%20CSS%20%2F%20JS-cyan?style=flat-square)
![Size](https://img.shields.io/badge/size-single%20file-green?style=flat-square)

---

## 🎮 How to Play

1. **Click the planet view** to hand-mine credits.
2. Spend credits on **buildings** to generate credits automatically (idle income).
3. Watch your colony grow on screen as you unlock new structures.
4. Reach **1,000,000 total credits** to unlock **Prestige** — reset for a permanent bonus multiplier.

---

## 🏗️ Buildings

| Building      | Base Cost  | Credits/sec | Visual |
|---------------|-----------|-------------|--------|
| Ore Drill     | 10        | 0.1         | Spinning drill on the surface |
| Solar Array   | 60        | 0.5         | Blue solar panels |
| Mining Bot    | 300       | 2.0         | Bobbing robot |
| Fusion Core   | 2,000     | 10          | Glowing reactor tower |
| Warp Gate     | 12,000    | 50          | Spinning purple portal |
| Dyson Sphere  | 100,000   | 300         | Golden light bathes the planet |

Each building you buy increases its own cost by **×1.15**.

---

## ✨ Features

- **Pixel art canvas** — animated colony that visually evolves as you build
- **Twinkling stars** in the background
- **Floating +N numbers** on click
- **Comms log** panel with milestone messages
- **Stats panel** — total earned, CPS, hand-mined count, run time
- **Prestige system** — resets progress for a multiplier bonus
- **Responsive layout** — works on mobile too
- **Zero dependencies** — one `.html` file, that's it

---

## 🚀 Deploy to GitHub Pages

1. Fork or clone this repo.
2. Go to **Settings → Pages**.
3. Set source to `main` branch, `/ (root)`.
4. Your game will be live at `https://<your-username>.github.io/<repo-name>/`.

Or just open `space-colony-idle.html` directly in any browser — no server needed.

---

## 🛠️ Customisation Tips

All game data is in the `G` object at the top of the `<script>` block:

```js
buildings: [
  { id:'drill', name:'Ore Drill', desc:'+0.1 cps each', base:10, cps:0.1, ... },
  ...
]
```

- Change `base` to adjust cost.
- Change `cps` to adjust income.
- Change `mult` (default `1.15`) to make cost scaling steeper or gentler.
- Add new buildings by appending to the array — the UI and canvas will pick them up automatically.

---

## 📄 License

MIT — free to use, remix, and publish.
