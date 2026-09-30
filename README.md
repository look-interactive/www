# look-interactive.com

Landing page for Look Interactive — a single self-contained static HTML page
(no build step, no dependencies), served by GitHub Pages at
https://look-interactive.com.

- `index.html` — the page (inline CSS + JS). The design treats the page as a
  lenticular print: pointer position is the "viewing angle" that flips the hero
  tagline, shifts the striped numerals, and steers the light-field shader,
  holo object and AI dot field. With no pointer it drifts on its own;
  `prefers-reduced-motion` stops all animation.
- `demo.html` — live in-browser tech demo.
- `CNAME` — custom apex domain (look-interactive.com).
- `.nojekyll` — serve files as-is, no Jekyll processing.
