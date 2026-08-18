# ALABASTER

A cinematic, scroll-driven low-poly city rendered entirely in the browser with three.js — from a fog-shrouded aerial of the metro down to a bustling sidewalk, in monochrome white.

## Run it

- **Locally**: open `index.html` in any modern browser (it works offline — three.js is vendored beside it), or serve the folder with any static server.
- **GitHub Pages**: Settings → Pages → deploy from the `main` branch, then visit your Pages URL.

Scroll to descend: aerial island → cloud layer → rooftop skim → avenue canyon → street level. On desktop/tablet the journey ends in a lateral storefront scene; on mobile it ends looking down the avenue through traffic.

## What's inside

- One self-contained `index.html` (~2,000 lines): procedural city, no downloaded assets
- Rotated street-grid districts, rivers, bridges, outer boroughs, a park with a pond
- 36+ building archetypes (ribbon-slab, chamfered, twin-with-skybridge, terraced, deco setback, zigzag slab, H-plan pre-war, framed dark-glass tower, and more) built from instanced unit shapes
- Four procedural facade languages — punched masonry, pier-and-spandrel strips, horizontal ribbon, curtain wall — with deep-set window reveals, corner quoins, loggia crowns, and radio masts
- 12 vehicle types in flowing traffic, each a swept superellipse shell with a dark wraparound greenhouse, light dish hubs, and a continuous light bar — in two detail tiers (fine on the hero street, lean for district traffic seen from altitude)
- Soft cumulus clouds and rounded tree canopies — smooth-shaded lobes, nothing faceted
- The borough fabric runs past the rivers all the way into the haze on desktop, so the metro never visibly ends
- A working intersection, and soft vinyl-toy pedestrians whose limbs are single Catmull-Rom swept tubes — leg into boot, arm into fist, no seams
- Tokyo-tight blocks: narrow carriageways, slim setbacks, and lots built out to their edges
- Hero sidewalks on a flat uniform plate with one square paver module, so the paving reads even from eye level
- Device-tier presets: ~45 draw calls / <500k triangles on mobile

## Tuning

Key dials at the top of the script in `index.html`: `PRESETS` (per-device counts), `districts` (grid layout), `WALL_STEPS` (palette), and the mist `defs` (fog shroud density).
