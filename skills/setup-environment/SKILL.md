---
name: setup-environment
description: Stand up a working data visualisation environment in a repo or workspace — install deps, create a starter project, wire up a reproducible build. Use after a tool has been chosen and the user needs it ready to run.
---

# Set Up a Data Visualisation Environment

Use this after `skills/choose-tool` has selected a library. The goal is a minimal, reproducible environment the user can iterate in.

## General principles

- **Reproducible by default**: pin versions, commit lockfiles.
- **One tool per project** unless the user has asked for a composite.
- **Separate data from code**: raw input under `data/`, generated output under `output/` (or `dist/`), source under `src/`.
- **Headless-capable**: if the target is static figures in a report, ensure the build can run without a display server.

## Recipe: Python (Matplotlib / Bokeh / Plotly Dash)

```
project/
├── pyproject.toml        # or requirements.txt
├── data/
├── src/
│   └── plots.py
├── output/
└── README.md
```

- Use `uv` or `venv` to isolate.
- Pin: `matplotlib`, `pandas`, `numpy`; add `bokeh` or `dash`/`plotly` as needed.
- For static export from Plotly/Bokeh, install `kaleido` (Plotly) or use Bokeh's `export_png` (requires `selenium`/`chromedriver` or Playwright).

## Recipe: Web publishing (Chart.js / Chartist / ECharts / D3 / visx / Vizzu / VChart / Lightweight Charts / react-globe.gl)

```
project/
├── package.json
├── index.html
├── src/
│   └── chart.(js|ts|jsx|tsx)
└── data/
```

- Default to Vite for vanilla JS/TS or React.
- For static deploys (report embeds), build to `dist/` and host as static assets.
- For D3 / visx, prefer TypeScript for maintainability on anything non-trivial.

## Recipe: Flutter (fl_chart)

- Scaffold with `flutter create`, add `fl_chart` to `pubspec.yaml`, pin a version.

## Recipe: Scientific / desktop (Constellation, DataWarrior, Iris)

- **Constellation** and **DataWarrior** are desktop apps — download the release binary, don't attempt to `pip install`.
- **Iris** is a Python library — install with `conda`/`mamba` (it has non-trivial geospatial C deps); document the conda env.

## Data storytelling extras

If the target is data storytelling (narrative scrolling, animated transitions):

- Scaffold in web stack (Vizzu or VChart).
- Add a `narrative/` folder for Markdown/MDX copy alongside the chart code so the story and viz stay together.

## Deliverables

Always leave the user with:

1. A working "hello chart" example that renders against sample data.
2. A documented command to rebuild (e.g. `python src/plots.py` or `npm run build`).
3. A one-line note on how to export to the intended publishing target (PNG, SVG, HTML embed, PDF figure).
