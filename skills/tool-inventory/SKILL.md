---
name: tool-inventory
description: Purpose-organised catalogue of validated data visualisation libraries, grouped by use case so a tool can be located quickly. Reference this at the start of any dataviz task to get a head start.
---

# Data Visualisation Tool Inventory

This is a curated, **purpose-first** catalogue. It exists so that when a task arrives, the right tool can be located by jumping to the matching section rather than reasoning from scratch.

**This is a guide, not a cage.** Every entry here has been validated as a sensible default for its category. If none of them fit, reach for whatever works — but start here, because the categories below cover the overwhelming majority of real-world dataviz work.

## How to use

1. Identify the task's **primary purpose** from the section headings below (e.g. "Graph / network", "Geospatial maps", "Story-driven animation").
2. Jump to that section.
3. Pick from the listed tools — each entry notes the sweet spot.
4. If nothing in the matching section fits, scan adjacent sections before going off-inventory.

---

## 1. Static publication figures (Python / R / C++)

For print, PDF reports, journal figures, Typst embeds — anywhere the output is a high-DPI PNG / SVG / PDF.

| Tool | Repo | Sweet spot |
|---|---|---|
| Matplotlib | https://github.com/matplotlib/matplotlib | Default for any Python static figure |
| Seaborn | https://github.com/mwaskom/seaborn | Statistical plots on top of Matplotlib — distributions, regressions, facets |
| ggplot2 | https://github.com/tidyverse/ggplot2 | The R classic; grammar of graphics; default for R workflows |
| matplotplusplus | https://github.com/alandefreitas/matplotplusplus | C++ projects needing Matplotlib-style output without Python |

## 2. Interactive web charts — general purpose

For embedding in blog posts, web apps, dashboards, static reports. Canvas or SVG output, runs in the browser.

| Tool | Repo | Sweet spot |
|---|---|---|
| Chart.js | https://github.com/chartjs/Chart.js | Simple canvas charts, ubiquitous, low ceremony |
| Chartist | https://github.com/chartist-js/chartist | Lightweight, responsive SVG |
| Apache ECharts | https://github.com/apache/echarts | Rich built-in chart types, dashboards, annotation-heavy work |
| ApexCharts | https://github.com/apexcharts/apexcharts.js | Modern SVG charts with good defaults; easy React/Vue/Angular wrappers |
| C3 | https://github.com/c3js/c3 | D3-backed wrapper, straightforward API |
| charts.css | https://github.com/ChartsCSS/charts.css | Pure CSS — no JS, great for static/email-safe charts |
| Plotly.js | https://github.com/plotly/plotly.js | Scientific chart types in JS; same API as Python Plotly |
| Highcharts | https://github.com/highcharts/highcharts | Classic polished charts; ubiquitous; commercial licence for commercial use |

## 3. High-performance / large-dataset web

When the dataset is big, the refresh rate is high, or latency matters.

| Tool | Repo | Sweet spot |
|---|---|---|
| uPlot | https://github.com/leeoniya/uPlot | Millions of points in milliseconds, tiny footprint, time-series |
| Perspective | https://github.com/perspective-dev/perspective | Streaming analytics viewer (WebAssembly), pivotable grids + charts |
| Lightweight Charts | https://github.com/tradingview/lightweight-charts | Financial / time-series, TradingView quality |

## 4. Low-level / bespoke

When the visual idiom isn't a stock chart — custom layouts, unusual encodings, data art.

| Tool | Repo | Sweet spot |
|---|---|---|
| D3 | https://github.com/d3/d3 | Ultimate flexibility; reach for this when no chart library fits |
| Observable Plot | https://github.com/observablehq/plot | Grammar-of-graphics layer on D3 — concise code, quick exploration |
| Vega | https://github.com/vega/vega | Declarative visualisation grammar (JSON spec) |
| Vega-Lite | https://github.com/vega/vega-lite | Concise higher-level grammar over Vega — the modern declarative classic |
| visx | https://github.com/airbnb/visx | React primitives built on D3, bring-your-own-composition |
| Victory | https://github.com/FormidableLabs/victory | React component charts, good for product UIs |
| Three.js | https://github.com/mrdoob/three.js | 3D scenes — reach for it when a chart needs true 3D beyond react-globe.gl |

## 5. Python / R dashboards & data apps

Interactive Python and R — dashboards, notebook-embedded viz, data apps.

| Tool | Repo | Sweet spot |
|---|---|---|
| Bokeh | https://github.com/bokeh/bokeh | Interactive browser plots from Python, streaming, dashboards |
| Plotly Dash | https://github.com/plotly/dash | Full reactive dashboards in Python |
| Altair | https://github.com/vega/altair | Declarative Python charts (Vega-Lite backend) — concise, composable |
| Streamlit | https://github.com/streamlit/streamlit | Python → web app in minutes; the modern classic for data demos |
| Gradio | https://github.com/gradio-app/gradio | ML/data demos, quick shareable UIs |
| Shiny | https://github.com/rstudio/shiny | R's classic reactive web-app framework (Python port exists) |
| D-Tale | https://github.com/man-group/dtale | Drop-in pandas DataFrame explorer — EDA without writing plot code |
| Briefer | https://github.com/briefercloud/briefer | Notebook + dashboard platform, shareable reports |
| Preswald | https://github.com/StructuredLabs/preswald | Lightweight Python data apps |

## 6. Data storytelling — animated / narrative

Persuasion and explanation. See `skills/data-storytelling` for the design side.

| Tool | Repo | Sweet spot |
|---|---|---|
| Vizzu | https://github.com/vizzuhq/vizzu-lib | Animated transitions between chart states — scrollytelling |
| VChart (VisActor) | https://github.com/VisActor/VChart | Narrative-first charting library |
| vue-data-ui | https://github.com/graphieros/vue-data-ui | Vue component set with story/presentation-friendly chart types |
| SandDance | https://github.com/microsoft/SandDance | Unit-visualisation explorer — every row becomes a mark, memorable for audiences |

## 7. Graph / network visualisation

Nodes and edges — knowledge graphs, social networks, dependency trees.

| Tool | Repo | Sweet spot |
|---|---|---|
| Constellation | https://github.com/constellation-app/constellation | Desktop analytics for large network datasets |
| G6 (AntV) | https://github.com/antvis/G6 | Web graph library, rich layouts, good defaults |
| sigma.js | https://github.com/jacomyal/sigma.js | Large-scale graph rendering in the browser, WebGL |
| GoJS | https://github.com/NorthwoodsSoftware/GoJS | Commercial, diagramming / interactive diagrams (flowcharts, org charts) |
| Cytoscape.js | https://github.com/cytoscape/cytoscape.js | Mature graph analysis + viz in the browser; strong algorithms |
| Gephi | https://github.com/gephi/gephi | Desktop classic for exploring and laying out large graphs |
| Graphviz | https://gitlab.com/graphviz/graphviz | DOT language — generated/diagrammatic graphs from code or pipelines |
| 3d-force-graph | https://github.com/vasturiano/3d-force-graph | Force-directed 3D graphs |

## 8. Geospatial / maps / globes

| Tool | Repo | Sweet spot |
|---|---|---|
| deck.gl (visgl) | https://github.com/visgl/deck.gl | WebGL geospatial layers at scale — hex bins, arcs, trips |
| react-map-gl (visgl) | https://github.com/visgl/react-map-gl | React wrapper for MapLibre / Mapbox GL |
| Leaflet | https://github.com/Leaflet/Leaflet | The classic lightweight web map — simplest path to an interactive map |
| MapLibre GL JS | https://github.com/maplibre/maplibre-gl-js | OSS fork of Mapbox GL; vector tiles, the modern default |
| OpenLayers | https://github.com/openlayers/openlayers | Classic; powerful projection / GIS-grade features |
| folium | https://github.com/python-visualization/folium | Python → Leaflet maps in notebooks |
| react-globe.gl | https://github.com/vasturiano/react-globe.gl | Interactive 3D globes |

## 9. Mobile

| Tool | Repo | Sweet spot |
|---|---|---|
| fl_chart | https://github.com/imaNNeo/fl_chart | Flutter charting |
| F2 (AntV) | https://github.com/antvis/F2 | Mobile-first web charting, small footprint |

## 10. Exploratory / auto-EDA tools

When the user doesn't yet know what they want to show — hand them a tool that surfaces structure.

| Tool | Repo | Sweet spot |
|---|---|---|
| DataWarrior | https://github.com/thsa/datawarrior | Desktop multi-dimensional exploration; chemistry-aware |
| RATH (Kanaries) | https://github.com/Kanaries/Rath | Auto-EDA, pattern discovery |
| D-Tale | https://github.com/man-group/dtale | Pandas DataFrame explorer (also listed under Python) |
| SandDance | https://github.com/microsoft/SandDance | Unit-viz exploration (also listed under storytelling) |

## 11. BI-style dashboards (self-hosted)

When the user wants a full BI tool they can host.

| Tool | Repo | Sweet spot |
|---|---|---|
| Apache Superset | https://github.com/apache/superset | Full-featured OSS BI — SQL-driven dashboards, classic enterprise pick |
| Metabase | https://github.com/metabase/metabase | Friendly OSS BI — quick setup, good for non-technical users |
| Grafana | https://github.com/grafana/grafana | Ubiquitous for time-series / monitoring dashboards |
| Kibana | https://github.com/elastic/kibana | The Elastic stack's viz layer (logs, search, observability) |
| Redash | https://github.com/getredash/redash | SQL-first dashboards and query sharing |
| Chartbrew | https://github.com/chartbrew/chartbrew | Open-source BI / client reporting |
| Briefer | https://github.com/briefercloud/briefer | Notebooks + dashboards (also listed under Python) |

## 12. Database / schema visualisation

Not chart-of-data, but visualisation of the data's structure.

| Tool | Repo | Sweet spot |
|---|---|---|
| Liam | https://github.com/liam-hq/liam | Auto-generate ERDs from schema |
| WhoDB | https://github.com/clidey/whodb | Lightweight database explorer / visualiser |

## 13. Diagrams-as-code

When the visual is a diagram (flow, sequence, architecture, ER) generated from text — great for docs and repos.

| Tool | Repo | Sweet spot |
|---|---|---|
| Mermaid | https://github.com/mermaid-js/mermaid | Markdown-native diagrams (GitHub renders inline); flow, sequence, Gantt, ER |
| PlantUML | https://github.com/plantuml/plantuml | Classic — UML, sequence, deployment diagrams |
| Graphviz (DOT) | https://gitlab.com/graphviz/graphviz | See §7; the foundational diagrams-as-code tool |

## 14. Domain-specific

| Tool | Repo | Sweet spot |
|---|---|---|
| Iris (SciTools) | https://github.com/SciTools/iris | Earth-science / gridded data (netCDF, climate) |
| QuantInvestStrats | https://github.com/ArturSepp/QuantInvestStrats | Quant finance research & strategy visualisations |
| XCharts | https://github.com/XCharts-Team/XCharts | Unity / in-game charts |
| BizCharts (Alibaba) | https://github.com/alibaba/BizCharts | Enterprise React charts, large Chinese-ecosystem deployments |
| Dataverse | https://github.com/multiverseweb/Dataverse | General-purpose dataviz platform |

## 15. Java / JVM

| Tool | Repo | Sweet spot |
|---|---|---|
| Tablesaw | https://github.com/jtablesaw/tablesaw | Java dataframe + built-in plotting |

## 16. Upstream data preparation (not visualisation, but adjacent)

For when the data isn't ready to plot yet. Dataviz-adjacent — use before reaching for a chart tool.

| Tool | Repo | Sweet spot |
|---|---|---|
| Data-Juicer | https://github.com/datajuicer/data-juicer | Multimodal data processing (oriented at LLM training corpora but useful for viz prep) |

> For general tabular/JSON cleaning and enrichment before visualisation, defer to the separate `data-wrangler` plugin.

## Discovery beyond the inventory

The catalogue above is a head start, not an endpoint. If a task genuinely doesn't fit any category here, scan these topic feeds before committing to something arbitrary:

- https://github.com/topics/datavisualization
- https://github.com/topics/data-visualization
- https://github.com/topics/matlab

State explicitly when going off-inventory and say why nothing on the list fit.

## Selection heuristic

1. Presentation medium → section (static → §1, web embed → §2/3/4, dashboard → §5/11, story → §6, graph → §7, map → §8, mobile → §9, exploration → §10).
2. Data shape → narrow within the section (time-series → uPlot/Lightweight Charts, tabular → ECharts/Plotly, network → §7, gridded/geo → §8).
3. Runtime → eliminate mismatches (Python-only, React-only, no-JS, etc.).
4. Interactivity level → pick the smallest tool that covers it.

Hand off to `skills/choose-tool` for the full decision protocol.
