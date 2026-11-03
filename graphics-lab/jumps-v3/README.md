# FMX Jump Lab V3 — Big Lips

**Open on an iPhone:** https://brendojones.github.io/fmx-freeride/graphics-lab/jumps-v3/

**Previous preview, unchanged:** https://brendojones.github.io/fmx-freeride/graphics-lab/jumps-v2/

## What's changed from V2

The user requested **all jumps at least 2× the previous height**, with a deliberate mix of small and enormous jumps, and a **steel ramp that genuinely curves UP at its launch lip instead of becoming horizontal**.

| Feature | V2 height (prototype units) | V3 height | Ratio |
| --- | ---: | ---: | ---: |
| Small warm-up roller | 1.52 | 3.18 | 2.09× |
| Big dirt tabletop | 3.45 | 7.50 | 2.17× |
| Steel FMX kicker | 5.25 | 11.20 | 2.13× |
| Huge dirt receiving lander | 6.25 | 13.40 | 2.14× |
| Step-down | 2.88 | 6.10 | 2.12× |
| Finishing jump | 2.20 | 4.60 | 2.09× |

The new dirt line runs 420 prototype metres, expanding horizontal spacing so the large features remain distinct.

## Actual geometry changes

- Smooth warm-up roller remains rounded.
- Tabletop and small/medium finishing takeoffs are *lip-led* using a quadratic-cubic rise shape `t²(.74+.26t)`. Unlike a smoothstep, the face has positive and noticeably steep tangent at its crest. Its landing downhill is still a smooth quintic eased-out transition.
- The main dirt lander reaches 13.4 units, with a longer gently declining catch face and run-out.
- The steel kicker runs from x=132 to 160 units, rising 11.2 units. Its deck shape is `h·(.67t²+.33t⁵)`: convex all the way to the crest, with a sharply increasing rise at the lip. At the tip the slope approaches 1.20 (roughly 50° above horizontal). It **does not flatten at the lip** like the V2 smoothstep ramp. Structural trusses follow this new shape.
- The camera uses a gradual zoom-out around the main kicker/lander, with height look-ahead, so large jumps can fit on a mobile screen.

This prototype is **original, independently drawn motocross-inspired scenery**. It does not copy screenshots, terrain data, trademarks or code from Mad Skills Motocross 3.

## How to try it

1. Open the URL on an iPhone, ideally landscape.
2. Tap **02 BIG TABLETOP** and inspect the tall jump face.
3. Tap **03 CURVED KICKER** to examine the curved steel takeoff as it flicks upward at the crest.
4. Tap **04 HUGE LANDER** to check the long dirt catching face.
5. Tap **PLAY** to follow the full line. Drag to explore; pinch to zoom.

**Still a track-art preview only, not a playable riding game.** The separately approved Honda/rider visual references remain untouched. A rideable game still requires real licensed 3D bike/rider files, skeleton animation, correct collision curves, gravity and landing physics.

## Test state

- JS source syntax check: passed.
- Canvas simulated in four portrait/landscape mobile view sizes: passed.
- Simulated animation loop: passed.
- Individual shape heights compared against V2: all at least 2.09×.
- Steel ramp tangent sampled near base, centre and tip: increasing (0.019, 0.377, ~1.19). Tip angle ~50°.
- Dirt height checked at 1-cm intervals; no sharp discontinuities (`max |dy| ~0.0097` per 0.01 unit).
- **Not visually verified on physical Safari/iPhone in this session**. The next step is to inspect the actual page on the user's phone and adjust visual proportions from that screenshot.
