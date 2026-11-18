# Animator

A CS 61A project: write small Gleam-like `draw` programs and watch them animate on a canvas.

**Live app:** [https://luise-haller.github.io/animator/](https://luise-haller.github.io/animator/)

## Run locally

```bash
gleam dev
```

Then open [http://localhost:8000](http://localhost:8000).

## Features

- Live code editor with built-in reference
- Animated path reveal on a canvas
- Shape slider (passed to `draw` as `shape_slider`) and speed slider (including reverse)
- Play / pause / reset
- Drawing library with examples, auto-save to `localStorage`, and “+ new” drawings

## Extension: Colored Sketch Orchestra

Beyond plain `Line` strokes, drawings can use coloured geometry and colour helpers:

| Shape / helper | Role |
| --- | --- |
| `ColorLine`, `Polyline`, `Circle`, `Arc`, `QuadCurve` | Coloured strokes and curves |
| `Color(r, g, b)` / `rgb` / `hue` / `palette` | RGB colour values (the language has no strings) |

Try the **orbit** example in the Draw menu, and drag the shape slider to change rings and colour.

See `extension.txt` for the full design write-up.

## Publish

```bash
gleam dev publish
```

Uploads the contents of `public/` (`index.html`, `animator.css`, `app.mjs`) to GitHub Pages for this repo.
