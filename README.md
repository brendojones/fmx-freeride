# FMX Freeride

A free, original, mobile-first 3D freestyle motocross experiment. This project deliberately focuses on **one jump, one bike, and one rider** before expanding the game.

## Current version: graphics pass 0.5

The latest build prioritises the rider and the bike over extra game modes:
- One steel FMX takeoff ramp and one dirt landing
- Sculpted plastic fairings instead of plain box panels
- Detailed engine, side panel graphics, wheel hubs, spokes, rear sprockets, tire tread and exhaust
- More detailed helmet with chin guard, goggle lens, vents and straps
- Rider jersey graphics, knee protectors, boots, pads and articulated trick poses
- A closer third-person camera for a better view of the rider and bike
- Backflip, Superman and whip; no extra tricks or new tracks

This is still a **custom procedural browser prototype**, not photorealistic racing-game footage. The next major quality leap will require importing professionally modeled and optimised GLB bike and rider assets, with a proper animated character skeleton, plus testing on a real iPhone.

## Controls

| Action | iPhone / Android | Computer |
| --- | --- | --- |
| Throttle | THROTTLE | W / Up |
| Brake | BRAKE | S / Down |
| Steer | ◀ / ▶ | A / D |
| Backflip | BACKFLIP | Space |
| Superman | SUPERMAN | Q |
| Whip | WHIP | E |
| Camera | CAMERA | C |
| Reset | RESET | R |

## Live website

The static HTML game is published through GitHub Pages (Settings → Pages, Deploy from main / root).

https://brendojones.github.io/fmx-freeride/

No paid hosting or account is required to play, and there are no game purchases. The game currently loads Three.js from a public CDN.

## Technical and safety notes

Three.js ES module, original mesh silhouettes, generated canvas decals and procedural materials. The ramp and handling are for entertainment and not validated against real-world FMX jumps or riding physics. This project does not include game assets copied from MX vs ATV, MX Bikes or Supercross.

## Future art workflow

Research free-to-use or commissioned high-quality GLB dirt bike models, character rigs, PBR textures and helmet/gear meshes; only replace placeholder geometry once licensing and mobile performance are verified.
