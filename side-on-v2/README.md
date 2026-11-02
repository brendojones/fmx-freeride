# FMX Side Stage — Compound V0.2

Separate playable iPhone-focused side-on freestyle motocross prototype. This build follows the signed-off design direction and leaves both existing games intact.

## Play

https://brendojones.github.io/fmx-freeride/side-on-v2/

GitHub Pages serves this directly from `side-on-v2/index.html`, using the same free hosting as before. This is a test version; new commits may take time to publish.

## What's actually implemented

- **Reversed the side camera** relative to the earlier side-on build: rider now travels across the screen toward the right.
- **Four features** in one continuously playable line:
  1. Dirt warm-up roller
  2. Long rounded dirt tabletop
  3. Steel FMX kicker and sculpted landing mound
  4. Smaller dirt step-down kicker and receiving lander
- **Matching height fields** for collision and visual dirt meshes, using hundreds of subdivisions, continuous side falloffs and layered soil textures.
- **More stable iPhone camera**, framed closer to the rider and looking ahead, plus sunrise-style sky gradient, bike-centred sun shadows and subtle dust.
- **Rider graphics pass**: shaped MX visor, refined shoulder armour, smoother anatomy, patterned riding gear, knee and boot detailing.
- **Touch only**, with throttle, brake, lean backward/forward, and backflip, Superman and whip; reset available onscreen.
- **Detailed motorbike model loader** from a CC0 source, with smaller CC0 fallback model when unavailable.
- Keeps the original side-on prototype at `../side-on/index.html` and the original chase-camera game at `../index.html`.

## Important limitations

This is not console-quality art yet. The character is still procedural; an actual rigged motocross rider asset plus artist-quality animation is needed to get rid of the remaining homemade look. The detailed motorcycle model is loaded from a third-party CDN and has a procedural fallback. These graphics improvements are not a substitute for testing on a real iPhone.

A syntax check, simulated launch, terrain-height samples and a simulated full-throttle run across the course passed, but visual rendering and performance on the user's phone remain unverified.

## Asset licensing

- Innerscene CC0 dirt motorcycle: https://www.innerscene.com/tools/library/3d-parts/dirt-motorcycle-0a9c8589
- CC0 3DAssets.dev mobile backup bike: https://3dassets.dev/

All procedural game code and art are original. No code, character rigs, or meshes were copied from MX vs ATV, Mad Skills, or commercial FMX games.

Game physics are fictional and not appropriate for real-life jump calculations.
