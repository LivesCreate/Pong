# Pong

Vertical Pong against an AI opponent, in the AMOLED-black / amber house style. You play the bottom paddle; the AI defends the top. No accounts, no internet, no backend.

Installable as a PWA on any device.

## Features
- **Vertical court** built for phones — drag your finger to move; on desktop use the mouse, arrow keys, or A / D.
- **Real ball behavior** — the bounce angle depends on where the ball hits your paddle, and the rally speeds up the longer it lasts.
- **Three AI levels** — Easy, Normal, Hard (reaction speed + aim accuracy). First to 7 wins.
- **Pause / resume** and a win–loss tally, both saved to localStorage.
- **Haptics** on paddle hits and points.

## Tech stack
- React 18 via CDN (`React.createElement`, no JSX, no bundler)
- HTML5 Canvas + requestAnimationFrame game loop
- `localStorage` for difficulty preference and stats
- PWA: `manifest.json` + `sw.js` (network-first, auto-reloads on update)

## Files
| File | Purpose |
|------|---------|
| `index.html` | The whole game |
| `sw.js` | Service worker |
| `manifest.json` | PWA manifest (AMOLED, fullscreen, embedded icon) |
| `version.txt` | Current version string |
| `.nojekyll` | Tells GitHub Pages to skip Jekyll processing |

## Deploy (GitHub Pages)
1. Put all files in the repository root.
2. **Settings → Pages**, source = your default branch, root folder.
3. Open the URL; install via "Add to Home Screen" / "Install app".

## Version
`1.0.0`
