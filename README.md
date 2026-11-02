# FMX Freeride

An original, mobile-first 3D freestyle motocross **graphics and riding prototype**. The aim is a realistic-looking Australian FMX training compound, not a huge open-world game.

## Features in prototype 0.4
- One dedicated compound with a steel FMX takeoff and dirt landing
- Selectable 75 ft (22.86 m) or 100 ft (30.48 m) landing gap
- Backflip, Superman and whip controls
- Rider pose animation for Superman; body/bike rotation for backflip and whip
- Mobile touchscreen and desktop controls
- Procedural terrain texture, steel frame details, riding camera and simple trick feedback

## Controls
| Action | Mobile | Desktop |
| --- | --- | --- |
| Accelerate | THROTTLE | W or ↑ |
| Brake | BRAKE | S or ↓ |
| Steer | ◀ / ▶ | A / D or ← / → |
| Backflip | BACKFLIP | Space |
| Superman | SUPERMAN | Q |
| Whip | WHIP | E |
| Reset | RESET | R |
| Toggle gap | 75 FT / 100 FT | G |
| Camera | CAMERA | C |

## Play it on iPhone / desktop
Enable **GitHub Pages** in this repository's **Settings > Pages**.
Choose **Deploy from a branch**, select **main** and **/(root)** and save.
Once published, the game is served from the same website address after each commit.
Open the Pages URL in Safari or a desktop browser. Landscape orientation is recommended on mobile.

## Development direction
Focus on real-looking bike and rider assets, more believable trick poses, realistic steel ramp and dirt landing, and improved bike physics before adding new locations or game modes.

## Current limitations
Prototype 0.4 uses original geometry and textures made with Three.js. It does **not yet** include a photorealistic imported 3D dirt bike or a mocap-rigged rider, and handling is **not** validated against real-world FMX jump trajectories. This is a game, not a jumping or rider-safety calculator.

## Technology
Static single-page Three.js ES-module web app. Three.js loads from a public CDN. No server, analytics, paid API or sign-in required for players.

No trademarked MX vs ATV or other game's source materials are used.
