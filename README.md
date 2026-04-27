# Image Fold

Interactive image break tool. Drop an image, drag a line through it, and watch the two halves fold toward you in real-time 3D perspective.

**Live preview:** https://ricardommatos.github.io/image-fold/

## Controls

- **Drop / click** — load an image
- **Drag handles** — move the fold line endpoints
- **Angle slider** — fold intensity (0–80°)
- **Depth slider** — perspective depth (400–2000px)
- **Reset Line** — restore default horizontal line
- **R** — reset everything
- **E** — export SVG

## Export

Exports the current state as a clean SVG with the source image embedded as base64 and the fold preserved via piecewise-affine triangulation (16×16 mesh per half). The SVG is portable to Figma, Illustrator, and any browser.

## Stack

- Vanilla HTML/CSS/JS, zero dependencies
- CSS 3D transforms for the live fold (GPU-accelerated)
- Custom mesh-triangulation for vector SVG export
- JetBrains Mono for UI typography
- Open `index.html` directly or via any static server
