# look-interactive.com

Landing page for Look Interactive — a single self-contained static HTML page
(no build step, no dependencies), served by GitHub Pages at
https://look-interactive.com.

- `index.html` — the page (inline CSS + JS). The design treats the page as a
  lenticular print: pointer position is the "viewing angle" that flips the hero
  tagline, shifts the striped numerals, and steers the light-field shader,
  holo object and AI dot field. With no pointer it drifts on its own;
  `prefers-reduced-motion` stops all animation.
- `demo.html` — the live lab: four full-screen WebGL2 experiences sharing one
  viewpoint input (on-device head tracker > device tilt > pointer > drift):
  **Window** (head-coupled off-axis 3D), **Hologram** (camera as scan-line
  relief), **Lenticular** (capture 8 frames, flip them under virtual lenses),
  **Wall** (bezel-compensated 3×3 wall, genlock on/off, real MediaRecorder
  codec round-trip with measured bitrate). Deep-link a mode with `#window`,
  `#holo`, `#lenti` or `#wall`. The camera never leaves the page.
- `CNAME` — custom apex domain (look-interactive.com).
- `.nojekyll` — serve files as-is, no Jekyll processing.
