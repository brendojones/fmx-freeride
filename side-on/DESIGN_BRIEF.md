# FMX Side Stage — iPhone game design brief

**Status:** agreed direction for the next build.  
**Project:** original, free-to-play browser-based freestyle motocross game on iPhone.  
**Scope:** side-on / 2.5D FMX, not open-world racing.  
**Existing playable demo:** `side-on/index.html` (keep it playable while developing).

## The vision

A proper-looking freestyle motocross game where the enjoyment comes from jumping, landing and throwing tricks, not racing. From a side-on camera, the player sees a convincingly modelled bike and rider moving across a compact FMX compound.

The next build must feel more like an authentic FMX game and less like a blocky, Minecraft-style prototype.

## Locked-in decisions

- **iPhone first and only for controls:** big multitouch targets, landscape layout, Safari compatible. Do not spend development time designing desktop/keyboard controls.
- **Reverse the travel direction relative to the current side-on build.** Keep the bike facing in the direction of travel and confirm the on-screen direction with a real iPhone screenshot.
- **Small freestyle line:** three to five well-designed jumps rather than a sprawling map.
- **One rider and one motorcycle** until they look good; avoid player customization or additional vehicles.
- **Backflip, Superman and whip** are the first three tricks. No trick expansion until these animate convincingly.
- **Keep the existing working demo** as a fallback while replacing its placeholder visuals in the side-on build.

## Course art: 4 jump features to build

1. **Warm-up dirt roller:** low, rounded lip with an equally smooth landing.
2. **Medium dirt tabletop:** clean side profile with obvious takeoff, flat top and downslope.
3. **Main freestyle jump:** realistic steel FMX kicker with visible braces, metal deck and a large sculpted dirt lander. This is the hero feature.
4. **Small step-down / finishing kicker:** a shorter flowing final jump for another trick opportunity.

Use one continuous terrain mesh, curved transitions, worn riding lines, ruts, scattered dirt and blended earth edges. No floating ramps, box-shaped platforms, giant cubes or harsh terrain seams. Keep collision geometry aligned with the visible dirt.

## Art direction: graphics are priority #1

**Bike**
- Use a properly modelled, optimised and licensed dirt-bike 3D asset in GLB/glTF format, not a stack of rectangles and cylinders.
- Correct FMX geometry: slim dirt-bike frame, realistic tyres and spoke wheels, front suspension, fenders, seat, exhaust, frame and number plates.
- PBR material treatment for painted plastics, rubber, aluminium and dusty components. Preserve silhouette and proportions when viewed from the side.
- Avoid copying branded game models or commercial graphics without permission.

**Rider**
- Replace the capsule-based placeholder with a properly modelled and rigged motocross rider where a suitable licensed asset is available.
- Full-face MX helmet, goggles, jersey, pants, gloves, knee protection and motocross boots.
- Natural proportions: no oversized spherical joints, stiff stick arms, floating boots or oversized torso.
- Rider crouches/stands naturally as the bike accelerates or leaves the lip.
- Superman moves the rider behind the bike while hands stay on the bars, then transitions back for landing.
- Backflips rotate rider and bike together; whip turns the bike sideways while the rider remains readable.
- Aim for smooth silhouettes and animation first, tiny details later.

**World and camera**
- Consistent side-on tracking with a clear view of the motorcycle, rider and landing ahead.
- Use a realistic sky gradient, atmospheric distance, directional sunlight, soft shadows and modest dust.
- The foreground riding area gets the highest texture/detail budget; the distant background stays subtle.
- The frame should never hide the landing behind UI controls or zoom out so far the rider becomes tiny.
- Keep asset weight and draw calls manageable on iPhone; provide quality settings if needed.

## Phone controls

- **Throttle** and **brake** as large hold-to-use buttons, grouped on the right.
- **Lean backward / forward** on the left, not 3D steering.
- **Backflip**, **Superman**, **Whip** as accessible multitouch trick controls.
- **Reset** available without opening a menu.
- Buttons must support multiple simultaneous fingers; safe areas must work in landscape.

## Build and quality gates

**First priority:** reverse the side-on travel direction and lock the camera and mobile UI.

**Second priority:** add the four distinctive jumps with sculpted, smooth terrain and working landings.

**Third priority:** replace the rider's crude geometric shapes with a high-quality licensed rigged character; align it to a believable dirt-bike mesh.

**Fourth priority:** polish lighting, dirt, decals, dust and each of the three tricks. Tune mobile performance only after visual direction is right.

**Done means:**
- A screenshot of the rider and dirt bike reads as motocross immediately, without Minecraft-like blocks.
- The rider and bike are large and clearly visible on an actual iPhone display.
- All four jumps have coherent ramps and safe visual transitions into landers.
- Throttle, braking, lean and all three tricks work together with touch.
- The game remains accessible through the existing free GitHub Pages project, using a separate side-on URL.
- We verify visual quality from actual mobile screenshots and do not call the result photorealistic unless it truly is.

## Explicitly out of scope

No desktop-control design, open-world map, racing opponents, online multiplayer, menus for customisation, extra tricks, extra bikes, sponsorship branding or new locations.

## Notes

This is a game prototype; jump dimensions and trick timing are not real-life FMX safety guidance. The previous version's real-asset loaders are experiments and must be verified for mobile loading and licensing before relying on them for final art. No payment or premium asset purchase is authorised by this brief.
