# Like the Wind — Breez Clifford, Ceramic Artist

A single-page static website. No framework, no build step — just HTML, CSS,
and image files. It can be opened directly in a browser or deployed as-is.

## Structure

    like-the-wind/
    ├── index.html      # the entire site (HTML + CSS in one file)
    ├── images/         # all photos, referenced by index.html
    └── README.md

That's it. There is nothing to compile.

## View it locally

Open `index.html` in any browser (double-click it, or drag it onto a browser
window). The `images/` folder must sit next to `index.html` for the photos to load.

## Add a new piece

1. Drop the photo into `images/` (e.g. `images/new-vase.jpg`).
2. In `index.html`, find the section you want (`<!-- SELECTED WORK -->` for
   sculptural pieces, `<!-- POTS -->` for functional work).
3. Copy an existing item block and change the `src`, the title, and the caption.

Sculptural pieces use full-width "plate" blocks (`<div class="plate">`);
functional pieces use the grid (`<div class="fn">`). The pot images display at
their natural shape — no cropping — so any photo orientation is fine.

## Deploy (static — IMPORTANT)

This is a static site. When setting up hosting:
- Framework preset: **None**
- Build command: **leave empty**
- Publish / output directory: the folder containing `index.html` (root)

Do NOT set a build command — there is nothing to build, and a build step is
what causes deploy failures. Drag-and-drop hosts (Netlify Drop) and Git-connected
hosts (Cloudflare Pages, Netlify) both work.

## Notes on content

- The three sculptural piece names/labels and Breez's bio are her own words.
- The three plate descriptions and the four pot captions/glaze names are
  placeholders drafted to be confirmed or replaced by Breez.
- Statement text is adapted from her artist statement (non-first-person).
- Open decision: the wordmark reads "Like the Wind" with "Breez Clifford" beneath;
  swap if the site should lead with her own name instead.
