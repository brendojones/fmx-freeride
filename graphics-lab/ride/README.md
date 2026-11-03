# FMX Side-On Ride Test — First Physics Integration

**iPhone URL:** https://brendojones.github.io/fmx-freeride/graphics-lab/ride/

**Locked artwork reference:** https://brendojones.github.io/fmx-freeride/graphics-lab/jumps-v3/

This is a new independent side-scrolling physics-and-model-loading experiment. It keeps the approved **Big Lips V3** jump artwork and up-curving metal FMX launch lip intact.

## What runs now

- Canvas V3 jump course reused, including the tall dirt jumps and strong curved steel kicker; a camera eases to follow the travelling rider and looks ahead to landings.
- Simple lightweight 2.5D kinematics: gravity, basic acceleration/deceleration, suspension/contact approximation from the track height profile, steep lip launches, airborne pitch control and a simple landing/crash check. THIS IS NOT simulation-quality real-bike suspension; collisions are estimated using a two-wheel spread and the centre track profile.
- Touch buttons: hold GAS, BRAKE, LEAN BACK / LEAN FORWARD. AUTO RIDE is a hands-free camera/physics demonstration. POWER cycles auto-throttle intensity. RESET restarts.
- Physics is visible even without a 3D bike, shown as a **clearly labelled orange physics marker**, not a low-quality stand-in motorcycle. Buttons work before model files are obtained.
- Transparent Three.js 3D layer over the V3 terrain. Can show an imported real motorcycle and separately imported rider that follow player physics, including airborne jumps and pitching.

## How to put REAL Honda/rider models in the riding test

1. Open the game page on iPhone Safari and tap **LOAD 3D**.
2. Open the official [2022 Honda CRF450 by Jacobdesigns](https://sketchfab.com/3d-models/free-honda-crf-450-c80f0e732e844580af412958c9d67315), download its CC BY model via Sketchfab's signed-in official Download 3D Model flow and save the glTF ZIP to iPhone Files.
3. Tap **SELECT FILE** beside HONDA and select that GLTF ZIP (or a permitted GLB) in Files. The model is loaded in the browser locally, not uploaded.
4. If a separately authorised realistic MX rider model is available, import it with the other **SELECT FILE** button. Use the fitting sliders and facing flip if necessary.
5. Close the load panel and tap **AUTO RIDE** or hold **GAS**; use LEAN to change angle in the air.

The previously approved [Hisenberg rigged motocross rider](https://www.cgtrader.com/3d-models/character/man/motocross-rider-rigged) is **not** bundled, purchased or downloaded. Its licence needs checking; do not assume an external 3D preview grants file rights.

Skinned character joints are not yet rigged into a seated position; imported rider may initially have a T-pose. Natural seated posture, hands-to-bars, boots-to-pegs, dynamically animated tricks, wheel spin, and genuinely realistic suspension/landing physics remain later tasks. A real 3D rider file is necessary for that work; the web 3D embed cannot be used as the model file.

### Technical implementation

- Existing original Canvas V3 track source reused in the new page, with no copying from Mad Skills Motocross 3.
- Three.js v0.170 overlay renders a licensed 3D GLB/glTF model using the same camera world scale as the 2D terrain. The overlay is side-on, transparent and resizes with iPhone orientation.
- Uses JSZip v3.10.1 for Sketchfab ZIP model imports; Three GLTFLoader with Draco and Meshopt decoder support.
- Imported assets stay in-browser for the session; the page does not store, publish, or upload model files.
- Physics loop subdivides time steps, samples the steel ramp profile all the way to its lip and takes off with upward velocity derived from final slope.
- Touch handlers use pointer capture. Basic keyboard controls are optional and not needed on phone.

## Validation

- Committed to GitHub separately from all previous games.
- Both inline and Three.js module script syntax: passed.
- Simulated iPhone-sized DOM/Canvas/WebGL startup: passed.
- Simulated driving physics through full 420-unit course: reached finish, launched and landed multiple times without JS exception.
- **Real iPhone Safari, downloaded Honda mesh orientation, rider pose, model import with actual downloaded files, and visual quality are not yet verified**. This is a technology milestone and **not** an announcement that the chosen high-quality bike and rider have already been integrated.

## Next step

Bring in actual legally downloadable Honda model and suitable rider mesh from iPhone Files or upload the files in ChatGPT. Inspect real screenshots, fix model orientation, fit the rider to the seat and manually animate posture, then refine terrain contact, tire roll and jump dynamics. The approved 3D reference pages remain available.
