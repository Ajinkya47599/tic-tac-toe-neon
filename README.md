# Tic Tac Toe 3D Neon – Poki Submission Package

This package contains a **fully playable** HTML5 game ready for Poki. It includes neon 3D visuals, win/draw/lose animations, PvP and AI modes, a persistent scoreboard, and **Poki SDK hooks** with safe fallbacks (so it runs without the SDK in local testing).

## Files
- `index.html` – the complete game (no external assets required).

## How to integrate Poki SDK
Paste their SDK script before `</body>` in `index.html`:

```html
<script src="https://game-cdn.poki.com/scripts/v2/poki-sdk.js"></script>
<script>
  // After the script loads, the in-file helpers will call PokiSDK.init()
  // You can also explicitly call:
  PokiSDK.init().then(() => console.log('Poki SDK initialized'));
</script>
```

The game already uses:
- `pokiSDK.gameplayStart()` / `pokiSDK.gameplayStop()`
- `pokiSDK.commercialBreak()` (toggle with `POKI_BREAK_ON_EACH_ROUND`)

## Mobile & Desktop
- Responsive layout via CSS grid
- Touch-friendly: buttons for cells, no text selection, no zoom traps

## Submission Metadata (prepare these)
- **Title:** Tic Tac Toe 3D Neon
- **Description:** A glowing 3D Tic Tac Toe with PvP and a smart AI. Win pulses, draw shakes, and clean neon style.
- **Controls:** Mouse / Touch
- **Genre:** Puzzle, Strategy
- **Screenshots:** 2–3 in‑game images (desktop + mobile)
- **Developer:** Your name or studio
- **Version:** 1.0.0

## Local testing
- Open `index.html` directly in a browser.
- Play a few rounds; try both modes and difficulties.
- Toggle `POKI_BREAK_ON_EACH_ROUND` if you want fewer/more ad breaks on Poki.
