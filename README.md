# characterdesign.io

Experimental landing page: a ball of clay inside a wireframe cube that deforms into characters, stretches out to the wireframe, and falls back into a ball. A synth drone follows the same motion.

It is one static file, `index.html`, with no build step. Three.js loads from a CDN. Open it through any static server (for example `npx serve .`).

## Playing with it

Everything worth changing is at the top of the script in `index.html`:

- `CONFIG` holds cube size, tendril count and thinness, the timing of each phase, and the drone's base note.
- `CHARACTERS` is a list of characters. Each one is a handful of soft ellipsoids (`c` centre, `r` radii), a colour and its eyes. Edit or add entries to make new forms.
- In the browser console, `__cd.jump(seconds)` moves to a point in the ball → excite → snap → hold → melt cycle.

Controls: drag to turn the cube, click (or press space) to disturb the clay, move the cursor near the clay to pull it.
