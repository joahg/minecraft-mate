# ⛏ Minecraft Mate ⛏

A Minecraft-themed chess checkmate practice app. Solve mate-in-1 puzzles on a blocky, pixelated chessboard with grass-block light squares and dirt-block dark squares.

🎮 **Play it:** [https://joahg.github.io/minecraft-mate/](https://joahg.github.io/minecraft-mate/)

## Features

- 🧩 A library of classic mate-in-1 puzzles (Back Rank, Smothered, Arabian, Damiano's, Epaulette, Swallow's Tail, Suffocation, Fool's Mate, Scholar's Mate, Promotion mates, and more)
- ♟️ Click-to-move with full legal-move highlighting and check/mate detection
- 💡 Hint button highlights the piece to move
- 🏁 Solution button plays the mating move for you
- 📊 Score tracker (solved / attempted)
- 🎨 Minecraft-inspired pixel art: grass + dirt board, blocky pieces, pixel fonts, inventory-style UI
- 🔊 Web Audio sound effects
- 📱 Installable PWA — works fully offline once loaded
- 🚫 Zero external runtime dependencies (chess engine is embedded)

## How it works

The app is a single-page PWA built with vanilla HTML/CSS/JavaScript. It includes a tiny embedded chess engine that handles:

- FEN parsing
- Legal move generation for all pieces (with check/pin filtering)
- Check & checkmate detection
- Pawn auto-promotion to queen

Every puzzle is validated on load — its stored solution must be a legal move that produces actual checkmate, otherwise it's filtered out.

## Local development

It's just static files. Serve the directory with anything:

```sh
# Python
python3 -m http.server 8000

# Or any static server
npx serve .
```

Then open <http://localhost:8000>.

## Deployment

Deployed via **GitHub Pages** from the `main` branch root.

## License

MIT
