# PoseNet Mustache Filter

A webcam filter that places a mustache image at a detected nose landmark.

**Repository created:** 2022-06-22  
**Project status:** Learning project / historical snapshot  
**Earliest recorded commit (author date):** 2022-06-22

## Features and implementation

- P5.js canvas.
- Ml5 PoseNet.
- Nose-coordinate tracking.
- Image overlay.
- PNG snapshot export.

## Technologies

HTML, CSS, JavaScript, Bootstrap, jQuery, p5.js, ml5.js, PoseNet.

## How the code works

`gotPoses()` reads the nose landmark, `draw()` renders the camera view and overlay, and `take_snapshot()` saves the canvas.

## Project structure

| File | Purpose |
| --- | --- |
| [`index.html`](index.html) | Main page and user interface |
| [`main.js`](main.js) | Project-specific JavaScript |
| [`style.css`](style.css) | Page styling |

Key functions in the source:
- `main.js`: `gotPoses()`, `take_snapshot()`.

## Run or explore locally

```bash
git clone https://github.com/Avenger-Sonic123/mustache-thingy.git
cd mustache-thingy
python -m http.server 8000
```

Open [http://localhost:8000](http://localhost:8000) in your browser. The local server requires Python 3; browser-based dependencies may also require internet access.

Allow camera access, position your face in view and use the snapshot button.

## Current status and limitations

The overlay is loaded from an external URL even though a local image asset exists; live performance depends on model and asset availability.

## Related project snapshots

Other repositories in this project family:
- [Project-113](https://github.com/Avenger-Sonic123/Project-113) — repository created 2022-03-11
- [project-114](https://github.com/Avenger-Sonic123/project-114) — repository created 2022-03-11

---

Source reference: [`db791383`](https://github.com/Avenger-Sonic123/mustache-thingy/tree/db7913838a1e50a140fc1c053fea9cb63b8bf9a9) on `main`, verified against GitHub on 2026-11-24. Documentation is based on static source review; runtime behavior has not been tested.
