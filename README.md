# ALABASTER

A cinematic, scroll-driven low-poly city rendered entirely in the browser with three.js — from a fog-shrouded aerial of the metro down to a bustling sidewalk, in monochrome white.

## Run it

- **Locally**: open `index.html` in any modern browser (it works offline — three.js is vendored beside it), or serve the folder with any static server.
- **GitHub Pages**: Settings → Pages → deploy from the `main` branch, then visit your Pages URL.

Scroll to descend: aerial island → cloud layer → rooftop skim → avenue canyon → street level. On desktop/tablet the journey ends in a lateral storefront scene; on mobile it ends looking down the avenue through traffic.

## What's inside

- One self-contained `index.html` (~2,000 lines): procedural city, no downloaded assets
- Rotated street-grid districts, rivers, bridges, outer boroughs, a park with a pond
- ~33 building archetypes (ribbon-slab, chamfered, twin-with-skybridge, terraced, deco setback, and more) built from instanced unit shapes with a procedural window shader
- 12 vehicle types in flowing traffic, soft vinyl-toy pedestrians with phones, a working intersection
- Device-tier presets: ~45 draw calls / <500k triangles on mobile

## Tuning

Key dials at the top of the script in `index.html`: `PRESETS` (per-device counts), `districts` (grid layout), `WALL_STEPS` (palette), and the mist `defs` (fog shroud density).
