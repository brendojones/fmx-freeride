# FMX Jump Lab V2 — Sculpted Dirt (track art pass 02)

Open on iPhone: https://brendojones.github.io/fmx-freeride/graphics-lab/jumps-v2/

Earlier comparison (unchanged): https://brendojones.github.io/fmx-freeride/graphics-lab/jumps/

## Completed passes

**Track Pass 1 — flowing profiles:** Continuous 330 m ground profile with eased-math rolling warm-up jump, long tabletop, prominent separated steel FMX takeoff with dirt lander, and finishing step-down. Curves are continuous and avoid box-shaped terrain. A 0.01 m numerical sweep found no abrupt dirt-height discontinuities.

**Track Pass 2 — visual depth:** The track is painted as a banked, thick ribbon with back and front lips, grain-oriented dirt shading, layered earthen face, soil strata, grooves, dispersed gravel, sparse ground plants and warm light catching riding-line highlights. Each surface-shading step samples the local terrain slope.

**Camera Pass — side-scrolling:** Smoothly eased side camera, roughly 30% left placement to show upcoming jumps, height lookahead weighted toward the upcoming lander, playback speed 0.5–2x and manual scrub/drag/pinch. iPhone-sized landscape and portrait viewports supported.

**Polish Pass — scenery and HUD:** Atmospheric desert sunset sky, clouds, distant hill silhouettes, sandstone outcrops, gum-tree silhouettes, subtle scrub and vignetting, bright feature markers. Clean touch UI with one-tap feature buttons for roller, tabletop, kicker, lander and step-down.

## How to review
1. Open the V2 URL in iPhone Safari; landscape mode makes it easier to see long gap/lander.
2. Tap **PLAY** and let the camera move along the course.
3. Tap **03 STEEL KICKER** or **04 BIG LANDER** to inspect the main feature.
4. Drag to look around, pinch to zoom; tap **V1 comparison** in the footer to compare.

## Important
This is an **original terrain and camera prototype**, not Mad Skills Motocross 3 game code, screenshots or game assets. It is not yet professional 3D graphics, and uses 2D Canvas with 2.5D depth cues. The objective is to iteratively improve jumping shapes and visual presentation, not claim equivalence to a commercial game.

There is deliberately **no bike or rider** in this art-only build. The approved Honda and rider direction is preserved in separate graphics-lab pages; the proper model files and rigging remain an asset workflow to solve later. No old "Minecraft-y" bike has been substituted.

## Testing / limitations
- JavaScript syntax parsed successfully.
- Simulated 844x390 Canvas rendering across multiple frames succeeded.
- Terrain height sampled at 23 stations with no sudden 0.01 m height jumps.
- iPhone Safari appearance and performance have **not yet been visually verified** in this session. Actual-device screenshots/feedback are the next gate before integrating gameplay.
