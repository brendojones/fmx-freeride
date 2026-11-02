# FMX Freeride — iPhone 3D prototype

The project is intentionally narrow: **one motocross bike, one FMX rider, one steel takeoff ramp and one sculpted dirt landing.** No new areas or additional jumps until the rider and lander look believable.

## Version 0.8: rider + dirt lander

- Rebuilt the **single landing mound** as a detailed 3D dirt surface, with soft shoulder transitions into the surrounding terrain, varying surface normals, organic dirt colour and subtle tyre marks. The same surface-height function is used for collision/landing.
- Refined the **procedural rider** with tapered anatomy, shoulder guards, joint folds, jersey back number graphics, gear seams, and a more active motocross riding posture that adjusts with speed and airtime.
- Kept the proper 3D motorbike model loader, original three FMX tricks and iPhone-only touchscreen controls.
- The bike is shown from a closer, adjustable mobile chase camera with an HD / smooth option.

## Play on iPhone

https://brendojones.github.io/fmx-freeride/

Open in Safari, rotate the phone sideways, and use the on-screen controls. Drag over the scenery to adjust camera direction. Updates to the same public GitHub Pages website don't require installing an app or downloading a ZIP.

### Graphics limitations (important)
The rider is still a **procedurally built, articulated model** and is not equivalent to a professional modelled, rigged FMX rider from a console game. The highest realistic visual-quality improvement would be a licensed, detailed 3D rider (GLB/FBX) with genuine skeletal animations and gear textures, adapted to this bike in a separate modelling workflow. No paid asset has been purchased or approved.

The motorcycle model loader attempts a public-domain detailed dirt bike, then a more mobile-friendly public-domain backup; if remote loading fails, the original procedural fallback stays playable. Status text under the game's title shows which model loads.

Current bike handling, trick animations and lander geometry remain entertainment-only and **must not be used for real FMX jump measurements**.

## Technical details
Three.js WebGL, glTF Loader, physically based materials, generated decals and dirt textures, collision height field, touchscreen pointer controls. One static HTML page hosted free on GitHub Pages. No account needed to play.

Model sources: Innerscene CC0 Dirt Motorcycle https://www.innerscene.com/tools/library/3d-parts/dirt-motorcycle-0a9c8589 , 3DAssets.dev backup https://3dassets.dev/ . No game graphics, animations or code copied from MX vs ATV or other commercial games.
