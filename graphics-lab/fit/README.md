# FMX Rider Studio — iPhone 3D fit preview

Open: https://brendojones.github.io/fmx-freeride/graphics-lab/fit/

This is a separate visual fitting tool. It does not change any existing games, and does not mean the paid motocross character has been obtained.

## Three views

1. RIDING POSITION: a realistic [dirt-bike and rider reference](https://sketchfab.com/3d-models/dirt-bike-enduro-rider-bb55f56ddaa04cbdb9cca1f6c262d042) from lewislabram, shown with its original interactive Sketchfab embed. This is NOT the selected Honda.
2. OUR HONDA: [2022 Honda CRF450 by Jacobdesigns](https://sketchfab.com/3d-models/free-honda-crf-450-c80f0e732e844580af412958c9d67315), offered for download by the artist under Creative Commons Attribution (CC BY). The exact file is not bundled.
3. FIT OUR MODELS: on-device Three.js viewer accepts properly licensed GLB or Sketchfab glTF ZIP files from iPhone Files. Rider scale, height, fore-aft and facing can be adjusted. The contents stay on the device; there is no upload to a server.

## Important constraints

- A high-quality motocross rider is not included: the rigged model previously shortlisted on CGTrader costs approximately US$50 and has an asset licence requiring review. No purchase has been made or authorised.
- Without the licensed Honda and rider mesh files, the viewer cannot truly mount the chosen paid rider on the chosen Honda. Sketchfab embeds show reference imagery only; they are not downloadable assets for this project.
- This is geometry alignment only. A T-pose character must still be posed and animated using skeletal joints, IK, and rider-to-bike contacts before it looks like Mad Skills Motocross 3.
- Do not publish third-party model files in GitHub without checking the licence terms and retaining required attribution.
- iPhone device rendering and Sketchfab iframe loading have not been independently verified.

## iPhone downloading and fitting — November 2026

Sketchfab's own Download API requires a logged-in user's authorisation; free CC BY models are **not** anonymous direct GLB links. Never use a site ripper or bypass authentication.

1. Open the **Fit Our Models** tab and tap **OPEN HONDA DOWNLOAD**.
2. In Sketchfab sign in with a free account, tap **Download 3D Model**, and select **glTF**. Save the provided ZIP unchanged to the iPhone Files app.
3. Return to **Fit Our Models** and tap **LOAD HONDA 3D**, selecting the saved ZIP. The WebGL scene reads it locally; no upload.
4. When an appropriately licensed rider 3D file is acquired, load its GLB/Sketchfab ZIP in **LOAD RIDER 3D**.
5. Adjust the four placement sliders, then select **SAVE FIT SETTINGS** (a JSON containing only positioning and filenames) and **SAVE PREVIEW PHOTO** (a PNG screenshot from the studio).

The site now provides the official source links, download notes, and screenshot/fit export directly on iPhone. This is **not** an automatic download from Sketchfab. Its authentication requirement can't be bypassed by the assistant. The earlier chosen Hisenberg CGTrader asset is listed as "Royalty Free License (no AI)", so the full licence and AI-assisted usage permissions should be checked before purchase or import. No purchase has been made.

The CC BY free "Low-poly Motocross Character (rigged)" is only 1,700 triangles and is intentionally not silently substituted. Another free CC BY "MX-Rider" model is about 1.5 million triangles, much too heavy for mobile without authoring/decimation and not confirmed as rigged. Neither is automatically suitable for this graphics-first approach.

## Next art milestone

Obtain properly licensed downloadable Honda and rider files; inspect their geometry and skeleton; fit a seated and standing pose with hands on handlebars and boots on pegs. Share an actual iPhone screenshot for art review before building jumps or gameplay.