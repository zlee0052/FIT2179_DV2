# Malaysia Tourism Rebound Was Strong — But Uneven

This project is created for **FIT2179 Data Visualisation 2** at **Monash University Malaysia**.

The visualisation explores Malaysia’s tourism recovery in 2024 through visitor arrivals, source markets, tourism receipts, hotel demand, domestic and foreign hotel guests, and air connectivity. The main story is that Malaysia’s tourism rebound was strong, but uneven across markets, sectors, and states.


## Project Overview

This project uses **Vega-Lite** to create ten data visualisations in a single scrolling webpage. The page is designed as a guided data story for a general Malaysian audience.

The story is divided into three sections:

1. **The rebound was visible in arrivals and entry routes**
2. **The recovery was shaped by different markets and spending patterns**
3. **The rebound was uneven across places and supported by infrastructure**

## Visualisations Included

1. Monthly foreign visitor arrivals, 2023 vs 2024
2. Foreign visitors by mode of entry
3. Top source markets for Malaysia
4. Source market growth from 2023 to 2024
5. Tourism receipts by spending category
6. Visitor arrivals vs tourism receipts by source market
7. Hotel occupancy rate by state using a choropleth map
8. Hotel guests by state using a proportional symbol map
9. Domestic vs foreign hotel guest share by state using a heatmap
10. Flight seat capacity by destination region using a slope chart

## Tools and Libraries

* HTML
* CSS
* JavaScript
* Vega
* Vega-Lite
* Vega-Embed
* GitHub Pages

## Data Sources

The datasets used in this project are based on publicly available tourism statistics and reports, mainly from:

* Tourism Malaysia official statistics reports
* Official Malaysia tourism datasets
* Public Malaysia state TopoJSON map data

The data was cleaned and reshaped for visualisation purposes. Some derived values were created, including:

* Growth percentages
* Market share percentages
* Foreign guest share
* Domestic guest share
* Receipts per visitor
* Year-based long-format data for Vega-Lite charts

## File Structure

```text
FIT2179-DV2/
│
├── index.html
├── styles.css
├── README.md
│
├── js/
│   └── vega_lite_vis.js
│
├── charts/
│   ├── chart1_monthly_visitors.json
│   ├── chart2_entry_mode.json
│   ├── chart3_source_markets.json
│   ├── chart4_market_growth.json
│   ├── chart5_spending_categories.json
│   ├── chart6_arrivals_vs_receipts.json
│   ├── chart7_occupancy_map.json
│   ├── chart8_hotel_guests_symbol_map.json
│   ├── chart9_domestic_foreign_heatmap.json
│   └── chart10_flight_connectivity_slope.json
│
└── data/
    ├── monthly_foreign_visitors_2023_2024.csv
    ├── entry_mode_2023_2024.csv
    ├── source_markets_2023_2024.csv
    ├── tourism_receipts_by_category_2023_2024.csv
    ├── source_markets_arrivals_receipts_joined_2024.csv
    ├── hotel_occupancy_by_state_2023_2024.csv
    ├── hotel_guests_by_state_2023_2024.csv
    └── flight_connectivity_to_malaysia_by_region_2023_2024.csv
```

## Design Rationale

Different chart idioms were selected to match the type of data being shown.

* Line charts are used for time trends.
* Dumbbell charts are used for year-to-year comparison.
* Bar and lollipop charts are used for ranking and category comparison.
* Bubble scatterplots are used to compare visitor volume and tourism value.
* A choropleth map is used only for normalised data, such as hotel occupancy rate.
* A proportional symbol map is used for absolute values, such as total hotel guests.
* A heatmap is used to compare domestic and foreign guest shares.
* A slope chart is used to show changes in air connectivity between 2023 and 2024.

The visualisation uses annotations, section headers, tooltips, and concise narrative text to guide the reader through the story.

## Author

Created by: **Lee Zhi Ming**
Unit: **FIT2179 Data Visualisation 2**
Institution: **Monash University Malaysia**
Date: **May 2026**

## AI Acknowledgement
Generative AI tools were used to support wording refinement, debugging, and data preparation.

Generative AI tools were used to support coding guidance, wording refinement, debugging, and data preparation. The final design, implementation, and interpretation were reviewed and edited by the author.
