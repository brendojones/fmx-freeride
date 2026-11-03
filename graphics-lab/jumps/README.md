# FMX Jump Lab — iPhone Side-Scrolling Track Preview

Viewer: https://brendojones.github.io/fmx-freeride/graphics-lab/jumps/

## What this does

A NEW graphics-first terrain-and-camera prototype, separate from the older playable games. The focus is the side-on **scrolling landscape** and the flow of the jump line. **There is intentionally no bike, rider, bike silhouette or gameplay in this test.** We are not reintroducing a fake low-detail bike while the approved Honda and licensed rider models are still pending.

## Jump features

- Warm-up roller: broad rounded lips with a gentle roll-through.
- Dirt tabletop: curved takeoff, level crown and curved downhill.
- Steel freestyle kicker: 15-unit shaped deck and visible structural bracing, followed by a gap.
- FMX dirt lander: large, long landing hill with rounded shoulders and smooth downhill.
- Short finishing step-down: smaller lift and soft receiving lander.

The entire earth track uses smooth interpolation, shaded hardpack dirt, subtle ruts, strata lines, fine soil particles, distance haze, scrolling distant hills, trees and fence parallax. The camera scrolls horizontally to the right relative to the travelling viewpoint, matching the side-view concept without copying any proprietary game code or assets.

## Controls

- **PLAY CAMERA** pans through the course. Tap again to pause.
- **SPEED** cycles through 0.5×, 1×, 1.5× and 2×.
- **Scrubber** jumps to any position along the course.
- Drag the scenery left/right to look around. Pinch to zoom. **RESET** returns to the start.

Optimised for Safari on iPhone; no keyboard input or PC-specific interface. The drawing is entirely original 2D Canvas artwork. A complete final game would use approved 3D bike/rider artwork and a stronger 2.5D rendering pipeline.

## Relationship to the rider / Honda studio

Approved appearance references remain available in [Bike Review](../index.html) and [Rider Fit Studio](../fit/). The selected Honda CRF450 is still only present as an external Sketchfab 3D preview, not a bundled playable bike. The rider reference is similarly an external model preview; the realistic rigged rider was not bought or downloaded. The lab makes no claim these assets are included.

## Validation

HTML and Canvas JavaScript committed and syntax-checked. Simulated startup and frame rendering were tested with stubbed DOM and canvas API, and sample jump heights verified. Real Safari/iPhone visuals and performance still need a user screenshot before any final art approval.

## Next stage

Approve the jump shapes and side-camera framing, then adapt a collision-aware 2.5D runner and load correctly licensed, downloadable motocross bike/rider model files. Keep model art and terrain art as separate milestones.