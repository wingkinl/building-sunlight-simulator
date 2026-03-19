# AGENTS.md

## Project Overview
Building Sunlight Simulator is a pure frontend web tool for architectural sunlight analysis. It converts 2D floor plans into 3D scenes, then simulates sunlight and shadow with geographic and solar calculations.

## Tech Stack
- Static HTML/CSS/JavaScript (no backend)
- Three.js (WebGL rendering)
- Offline-capable local usage

## Core Workflow
1. Use `editor.html` to upload a plan, calibrate scale, draw buildings, and export JSON.
2. Use `index.html` to import JSON, adjust location/date/time, and run sunlight analysis.
3. Optionally run quantified sunlight-duration calculation with heatmap results.

## Key Files
- `editor.html`: data creation UI
- `index.html`: visualization and simulation UI
- `js/editor.js`: editor logic
- `js/viewer.js`: viewer/simulation logic
- `js/config.js`: global settings
- `js/utils.js`: shared utility functions
- `js/i18n.js`: language support
- `js/cities.js`: built-in latitude/city data
- `examples/sample.json`: sample input data

## Run Instructions
- Open `editor.html` or `index.html` directly in a browser, or
- Serve locally (recommended) via tools like `live-server` or `python -m http.server`.

## Guiding Principles
- Only made changes that is relevant and necessary.
- Add comments if needed.
- Do not touch any code that is not relevant or not requested.
