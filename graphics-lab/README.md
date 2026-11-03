# FMX Visual Studio — graphics-first rebuild

**Purpose:** start fresh, separate from the older browser games. Compare the quality of licensed 3D motorcycle and rider assets on an iPhone before working on gameplay, jump designs or trick animations.

## Open the graphics test

https://brendojones.github.io/fmx-freeride/graphics-lab/

Touch controls: select THE BIKE / THE RIDER / SIDE BY SIDE, drag to rotate, pinch to zoom. This is an **artwork inspection tool**, not a playable game. No keyboard-based controls were added.

## Actual assets attempted

1. **Detailed dirt motorcycle**, Innerscene — original unbranded public-domain CC0 asset, ~6.7 MB, real scale. Source: https://www.innerscene.com/tools/library/3d-parts/dirt-motorcycle-0a9c8589 . Direct URL used: https://www.innerscene.com/api/library/dirt-motorcycle-0a9c8589/download . Direct cross-origin loading and iPhone performance are not independently verified.
2. **Mobile fallback motorcycle**, 3DAssets.dev — CC0 trials competition bike, 6,288 triangles, ~308 KB, permanent CORS-enabled direct URL https://cdn.3dassets.dev/assets/15417/v1/model.glb . Source: https://3dassets.dev/assets/motorcycle-racing-and-street-bikes-trials-bike-5643520e . This is a **trials bike**, not final MX bike artwork.
3. **Rigged athlete trial**, CodeLove Male Athlete 03 — MIT license, 80 bone skeleton, 9,534 tris, 785 KB, real 3D asset. Published source: https://models.codelove.in/models/sports-male-03/ . **CAUTION:** The viewer now first reads the publisher's CORS-enabled public `catalog.json` and attempts to load the athlete's published direct GLB URL from the catalog. If that lookup fails, it tries two unverified URL conventions and then clearly reports failure. Live loading on an iPhone remains unverified. If this model is eventually bundled, retain the asset's MIT copyright and license text.
4. The rider is NOT wearing a proper motocross helmet or MX gear yet and is NOT in a fitted riding pose. These are later modelling/rigging steps after we select a convincing base model. Do not present it as finished FMX character art.

## Principles

- **No fabricated box/capsule bike or rider** when the real model fails to load. Failure must be visible.
- This first prototype features neutral studio lighting, floor shadows, model rotation and zoom; no jumps, tracks or trick physics.
- The older playable prototypes are unchanged: `../index.html`, `../side-on/index.html`, `../side-on-v2/index.html`.
- We need screenshots from an **actual iPhone** to verify load, silhouette, model orientation, character, texture, frame rate and whether this is substantially closer to Mad Skills Motocross 3 visual quality.
- No purchased or copyrighted commercial-game assets may be added without the proper permissions.
- The next work after art review is source a genuine detailed motocross helmet/gear and fit/animate the rider with skeletal poses, then choose the motorcycle that looks right and optimize for iPhone.

## Current status

HTML and JavaScript committed (Model Review 0.2, including dynamic public-catalog rider resolution), but no live render/device verification by the assistant. If neither athlete link works, select a verified direct CORS GLB or add a licensed rider to the project as a bundled file; don't replace with procedural primitives.
