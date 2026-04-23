---
name: choose-tool
description: Decision protocol for selecting the right data visualisation tool from the inventory based on output medium, data shape, runtime, and storytelling needs. Use when the user asks for a chart/graphic/dashboard but hasn't specified a library.
---

# Choose the Right Visualisation Tool

Use this when the user wants a visualisation and hasn't named a library. The goal is to start from the purpose-organised inventory (`skills/tool-inventory`) so the pick is grounded, rather than defaulting to whatever first comes to mind.

The inventory is a head start, not a cage — if nothing listed fits, go outside it and say why.

## Decision axes

Ask (or infer) along these axes before picking:

1. **Presentation purpose**
   - Static figure for a report/PDF/print
   - Embedded chart on a web page / blog
   - Interactive dashboard
   - Animated / narrative data storytelling
   - Scientific / exploratory analysis
2. **Data shape**
   - Tabular (rows × columns)
   - Time-series / financial
   - Network / graph
   - Gridded / geospatial raster (netCDF, climate)
   - Geospatial points / globe
3. **Runtime the user works in**
   - Python pipeline
   - JS / web front-end (vanilla, React, general)
   - Flutter
   - Desktop app (no code)
4. **Interactivity required**
   - None (export PNG/SVG)
   - Hover / tooltip
   - Full linked-brushing dashboard
   - Animated transitions between states
5. **Audience**
   - Technical / analyst — exploration
   - General — storytelling, clarity-first

## Quick mapping (defaults)

| Need | Pick |
|---|---|
| Publication-quality static figure, Python | Matplotlib |
| Interactive Python dashboard | Plotly Dash or Bokeh |
| Lightweight web chart, minimal deps | Chartist or Chart.js |
| Dashboard-class web charts with many types | Apache ECharts |
| Bespoke / custom visual, web | D3 |
| React-native chart primitives | visx |
| Financial / time-series, web | Lightweight Charts |
| Flutter app chart | fl_chart |
| Animated storytelling transitions | Vizzu |
| Narrative / story-driven charts | VChart |
| Network / graph exploration | Constellation |
| Multi-dim interactive exploration (desktop) | DataWarrior |
| Earth-science gridded data | Iris |
| Quant finance research | QuantInvestStrats |
| 3D globe | react-globe.gl |

## Protocol

1. Read `skills/tool-inventory` for the canonical list and repo links.
2. If the user's need maps cleanly to the table above, propose that tool and state why in one sentence.
3. If two inventory tools fit, present both with a one-line tradeoff and ask.
4. If nothing in the inventory genuinely fits, propose a non-inventory tool and say so explicitly with the reason.
5. Once chosen, hand off to `skills/setup-environment` if the user needs the toolchain stood up, or proceed to implementation.
