# Data Visualisation And Publishing

Create static and interactive data visualisations for reports, repos, and data storytelling — prioritising a curated inventory of open-source tools.

This plugin opinionates the tool choice. Instead of reaching for whatever library the model happens to recall, it selects from a maintained inventory (Matplotlib, Bokeh, Chart.js, ECharts, D3, visx, Vizzu, VChart, Plotly Dash, Lightweight Charts, fl_chart, Constellation, DataWarrior, Iris, QuantInvestStrats, react-globe.gl, and others) and matches the tool to presentation purpose, data shape, runtime, and audience.

## Skills

- **tool-inventory** — canonical catalogue of preferred libraries grouped by use case (scientific, web, app, animated, Python, geospatial).
- **choose-tool** — decision protocol that maps presentation purpose + data shape + runtime to a tool in the inventory.
- **setup-environment** — scaffolds a reproducible dataviz project (Python / web / Flutter / desktop) with a working "hello chart" example.
- **data-storytelling** — narrative-driven visualisation design: headline-first charts, annotation, animated transitions, interactive elements that earn their place.

## Commands

- `/dataviz-pick` — pick the right tool from the inventory for a given task.
- `/dataviz-setup` — scaffold a dataviz environment using the chosen tool.
- `/dataviz-story` — design and build a data-storytelling piece.

## Philosophy

1. **Pick from the inventory first.** Only reach outside if nothing fits, and justify it.
2. **Match the medium.** Static PDF figure, web embed, dashboard, animated story, and geospatial all want different tools.
3. **Storytelling ≠ dashboards.** If the goal is persuasion, build one chart one claim; if the goal is exploration, build a dashboard.
4. **Reproducible by default.** Pin deps, commit lockfiles, keep data/code/output separate.

## Installation

```bash
claude plugins install data-visualisation-and-publishing@danielrosehill
```

## License

MIT
