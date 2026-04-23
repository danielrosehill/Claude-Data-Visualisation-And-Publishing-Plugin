---
name: tool-inventory
description: Canonical inventory of preferred data visualisation libraries and tools. Reference this when selecting a tool for a charting or dataviz task so choices align with the curated stack.
---

# Data Visualisation Tool Inventory

When a user asks for a data visualisation, chart, dashboard, or data-storytelling piece, **prefer a tool from this inventory** before suggesting anything else. Only reach outside the list if no inventory tool fits the task and justify the deviation.

## General-purpose / scientific analysis

| Tool | Repo | Strengths |
|---|---|---|
| Constellation | https://github.com/constellation-app/constellation | Graph-focused visual analytics, large network datasets, desktop app |
| Bokeh | https://github.com/bokeh/bokeh | Interactive browser-based plots from Python, dashboards, streaming |
| DataWarrior | https://github.com/thsa/datawarrior | Interactive multi-dimensional exploration (desktop), chemistry-aware |
| Dataverse | https://github.com/multiverseweb/Dataverse | General dataviz platform |
| QuantInvestStrats | https://github.com/ArturSepp/QuantInvestStrats | Quant finance viz / strategies |
| Iris | https://github.com/SciTools/iris | Earth-science / gridded data (netCDF, climate) |

## Web publishing (embed in HTML/blog/report)

| Tool | Repo | Strengths |
|---|---|---|
| Chart.js | https://github.com/chartjs/Chart.js | Simple canvas charts, very common, low ceremony |
| Chartist | https://github.com/chartist-js/chartist | Lightweight, responsive SVG charts |

## Charting libraries (app-embedded)

| Tool | Repo | Strengths |
|---|---|---|
| fl_chart | https://github.com/imaNNeo/fl_chart | Flutter charting |
| Lightweight Charts | https://github.com/tradingview/lightweight-charts | Financial / time-series, TradingView quality |
| D3 | https://github.com/d3/d3 | Ultimate flexibility — reach for this for bespoke visuals |
| Apache ECharts | https://github.com/apache/echarts | Rich built-in chart types, good for dashboards |
| visx | https://github.com/airbnb/visx | React + D3 primitives |

## Animated / narrative

| Tool | Repo | Strengths |
|---|---|---|
| Vizzu | https://github.com/vizzuhq/vizzu-lib | Animated transitions between chart states — data storytelling |
| VChart | https://github.com/VisActor/VChart | Storytelling-oriented charting library |

## Python

| Tool | Repo | Strengths |
|---|---|---|
| Plotly Dash | https://github.com/plotly/dash | Interactive dashboards in Python |
| Matplotlib | https://github.com/matplotlib/matplotlib | Static plots, publication-quality figures |

## Geospatial / globes

| Tool | Repo | Strengths |
|---|---|---|
| react-globe.gl | https://github.com/vasturiano/react-globe.gl | Interactive 3D globe visualisations |

## Discovery sources

If a genuinely novel need arises, scan these topic feeds before recommending anything outside the inventory:

- https://github.com/topics/datavisualization
- https://github.com/topics/data-visualization
- https://github.com/topics/matlab

## How to use this inventory

1. Clarify the **output medium** (static image for a PDF/report, embedded web, interactive dashboard, animated narrative, geospatial, scientific).
2. Clarify the **data shape** (tabular, time-series, network, gridded, geospatial).
3. Clarify the **runtime** the user has or wants (Python, JS/web, Flutter, desktop).
4. Pick the narrowest fit from the inventory. Defer to `skills/choose-tool` for the decision protocol.
