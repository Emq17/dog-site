# Can I pet your dog? 🐶

A playful mini web page with a cute SVG character, a sneaky “No” button that runs away, and full-screen confetti when you click “Yes”.

## What it does
- **Cute prompt** with a soft gradient background and a glassy card UI
- **“No” button dodges your cursor/touch** inside the button zone
- **“Yes” button grows** every time “No” runs away
- **Full-screen confetti celebration** (using `canvas-confetti`) + a fireworks GIF reveal on “Yes”

## Tech stack
- **HTML + CSS + Vanilla JavaScript**
- **canvas-confetti** via CDN
- Inline **SVG** art (no image files needed)

## Hosting
Perfect for GitHub Pages or any static host. No build step required.

## Run locally
Open `index.html` in your browser.

## Customize
- Change the question:
  - Edit the `<h1>`:
    ```html
    <h1>Can I pet your dog?</h1>
    ```
- Change your reaction:
  - Edit the `<h2>`:
    ```html
    <h2>Yayyyy! 🎉</h2>
    ```
- Change colors:
  - Update the CSS variables in `:root` (in `styles.css`):
    ```css
    --bg1: #ffd6e7;
    --bg2: #ffeef6;
    --yes: #ff3b7a;
    --yesHover: #ff1f68;
    ```
- Swap the celebration GIF:
  - Replace the `src` on `fireworks` in `index.html`

## Notes
- Works on desktop + mobile (uses `pointermove` + `pointerdown` for touch-friendly behavior)
- Confetti is rendered on a full-screen `<canvas>` layered above the UI

## Credits
- Confetti: `canvas-confetti` (CDN)
- Fireworks GIF: Giphy
