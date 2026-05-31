# DV2 Malaysia Tourism Dataset Pack

Prepared for a Vega-Lite / VS Code DV2 project. All extracted CSVs are in `/data`.

## Recommended story
**Malaysia Tourism Recovery & Transformation:** how international visitors returned in 2024, where they came from, what they spent on, and which states/hotel markets benefited.

## 10 chart plan
1. `monthly_foreign_visitors_2023_2024.csv` — line chart comparing monthly 2023 vs 2024 foreign visitors.
2. `mode_of_transport_2023_2024.csv` — bar/donut chart showing how visitors entered Malaysia.
3. `top20_source_markets_visitors_2023_2024.csv` — ranked bar chart of top source markets.
4. `top20_source_markets_visitors_2023_2024.csv` — dumbbell chart comparing 2023 vs 2024 by country.
5. `visitor_expenditure_items_2023_2024.csv` — spending composition bar/treemap.
6. `source_markets_arrivals_receipts_joined_2024.csv` — scatterplot: arrivals vs receipts, with per-visitor spend in tooltip.
7. `hotel_supply_by_state_2023_2024.csv` — state bar chart or map for hotel rooms.
8. `hotel_occupancy_by_state_2023_2024.csv` — choropleth map of average hotel occupancy rate.
9. `hotel_guests_by_state_2023_2024.csv` — stacked bar chart showing domestic vs foreign hotel guests by state.
10. `flight_connectivity_to_malaysia_by_region_2023_2024.csv` — bar chart of weekly seat capacity growth by region.

Extra useful map-ready file: `state_tourism_map_ready_2024.csv`. Use with this TopoJSON URL:
https://raw.githubusercontent.com/jnewbery/CartogramMalaysia/master/public/data/malaysia-states.topojson

In Vega-Lite, join `topo_name` in the CSV to the TopoJSON state name/id. Note: the TopoJSON uses **Penang**, while Tourism Malaysia tables use **Pulau Pinang**, so I added a `topo_name` column.

## Important labelling note
The Tourism Malaysia 2024 PDF uses **foreign visitors** for the 37,961,485 figure. A visitor includes tourists and excursionists. Avoid labelling these rows as only “tourists” unless your chart uses a separate tourist-only dataset.

## Source summary
See `source_manifest.csv` for URLs. Keep these source links in your GitHub page footer/metadata section.

## Assignment reminder
DV2 requires at least one map, two data sources, at least 10 charts, Vega-Lite, and a publicly accessible GitHub page.
