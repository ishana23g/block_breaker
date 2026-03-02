# Block Breaker 🧱

A mobile-first block puzzle game — no build tools, no dependencies. Just open `index.html` and play, or install it as a PWA straight from your phone.

## Play Online

👉 **[Play now on GitHub Pages](https://ishana23g.github.io/block_breaker/)**

---

## How to Play

1. **You get 3 pieces per round.** Drag any piece from the bottom tray onto the 8×8 grid.
2. **Fill a complete row _or_ column** and it clears, scoring points. Fill multiple at once for a combo bonus.
3. **Every 5 rounds** a handful of obstacle blocks are added to the grid — plan ahead!
4. **Game over** when none of your 3 pieces can fit anywhere on the board.

### Controls

| Platform | Drag piece | Place piece |
|----------|-----------|-------------|
| Mobile   | Touch & drag | Release finger |
| Desktop  | Click & drag | Release mouse |

### Hover / Drag Preview

| Highlight | Meaning |
|-----------|---------|
| **Purple dashed** | Valid placement for the piece |
| **Gold glow** | Row or column that will be cleared on drop |
| **Red dashed** | Invalid placement (overlapping or out of bounds) |

---

## Scoring

| Action | Points |
|--------|--------|
| Place a piece | +1 per block in the piece |
| Clear 1 line | 8 × 10 = **80 pts** |
| Clear N lines at once | 8 × 10 × N × N (**combo multiplier**) |

---

## Piece Types

33 Tetris-inspired shapes across 6 size categories:

- **Singles & Dominoes** — 1–2 blocks
- **Trominoes** — 3 blocks (straight, L-corners)
- **Tetrominoes** — all 7 classic Tetris shapes (I, O, T, L, J, S, Z) with rotations
- **Pentominoes** — selected 5-block shapes (I, L, T, S, Z variants)
- **Rectangles** — 2×3 and 3×2 blocks
- **Squares** — 2×2 and 3×3 solid squares

Piece sizes are **weighted by how full the board is** — the more occupied the grid, the more likely you'll receive smaller pieces that can still fit.

---

## Install on Your Phone (PWA)

The game is a Progressive Web App (PWA):

- **iOS Safari** → tap the Share icon → *Add to Home Screen*
- **Android Chrome** → tap the browser menu → *Install app* (or *Add to Home Screen*)

Once installed it works offline and feels like a native app.

---

## Deploy on GitHub Pages

1. Go to **Settings → Pages** in this repository.
2. Under *Source*, select **Deploy from a branch**.
3. Choose **main** and **/ (root)**, then click **Save**.
4. Your game will be live at `https://<username>.github.io/block_breaker/`.

## Run Locally

No server needed — just open the file directly:

```bash
open index.html      # macOS
xdg-open index.html  # Linux
start index.html     # Windows
```
