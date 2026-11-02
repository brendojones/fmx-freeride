# FMX Freeride

Free browser-based freestyle motocross game prototype for iPhone and desktop.

**Current direction: one jump only. Get the motorbike and rider looking believable before adding new content.**

## What's new in 0.6 — an actual 3D model pipeline

The old all-procedural dirt bike looked too much like Minecraft. This version attempts to load an original, licensed detailed 3D motorcycle model with real mesh contours and authored materials. It uses the existing ride and trick mechanics rather than replacing the game.

The browser tries these **CC0 / public-domain** assets in order:

1. **Higher-detail dirt motorcycle** — Innerscene, 108,138 tris, ~6.7 MB, 815 separate meshes. Source: https://www.innerscene.com/tools/library/3d-parts/dirt-motorcycle-0a9c8589 — CDN API: https://www.innerscene.com/api/library/dirt-motorcycle-0a9c8589/download . This cross-origin download might fail or run slowly on phones.
2. **Mobile-compatible backup** — Trials competition bike by 3DAssets.dev, 6,288 tris, ~308 KB, CC0, +Y up and +Z forward. Reliable public CORS-enabled GLB: https://cdn.3dassets.dev/assets/15417/v1/model.glb — source: https://3dassets.dev/assets/motorcycle-racing-and-street-bikes-trials-bike-5643520e .
3. **Offline loading fallback** — our prior hand-built motorcycle only when both model downloads fail; the game should remain playable.

**On the game screen, the status underneath the FMX FREERIDE title reports what actually loaded:** DETAILED 3D DIRT BIKE, OPTIMISED 3D DIRT BIKE, or PROCEDURAL BIKE • MODEL UNAVAILABLE. Do not describe the model as upgraded unless its status shows it loaded.

Real model integration also rotates source model axes based on bounding-box proportions, normalizes the scale to the 2.2 m motocross bike and moves the existing articulated rider into a more realistic riding position. This is a static model swap, not yet true suspension or a skinned rider.

## Work in progress

- **The rider is still a procedural articulated character**, not a motion-captured rider. Proper helmet, jersey, pants, body shapes and animation need a licensed rigged character model and custom riding animations.
- Neither 3D model was play-tested on the user's specific iPhone as part of this commit; wait for feedback. CORS failures fall back gracefully.
- Jump motion, backflip, whip and Superman remain simplified arcade physics and should not be used as real FMX jump calculations.
- The high-detail model is too complex to guarantee smooth performance on every phone. We will need to optimise draw calls / materials or bundle an LOD model for future versions.

## Play

GitHub Pages (public GitHub repository, no additional paid host needed):
https://brendojones.github.io/fmx-freeride/

Landscape orientation strongly recommended on mobile.

| Action | iPhone | Desktop |
| --- | --- | --- |
| Throttle | THROTTLE | W / Up |
| Brake | BRAKE | S / Down |
| Steering | Arrows | A / D |
| Backflip | BACKFLIP | Space |
| Superman | SUPERMAN | Q |
| Whip | WHIP | E |
| Camera | CAMERA | C |
| Reset | RESET | R |

## Technology and licensing

Three.js WebGL, GLTFLoader, dynamic model replacement with fallbacks, authored PBR materials, one FMX steel launch and dirt landing. The CC0 third-party motorcycle assets above may be used without attribution; their source links are retained here as documentation.

This is an original prototype and contains no copied assets or code from MX vs ATV, MX Bikes or Supercross games.
