# Forest Carbon Infographic

This repository contains the source code for an interactive, accessible infographic embedded in a [Forest Carbon ArcGIS StoryMap](https://storymaps.arcgis.com/stories/77eac7cb51b04f77bb77343be1bcee2d).

## Overview
This infographic compares greenhouse gas emissions across human sectors in Massachusetts to the sequestration capacity of the state’s natural and working lands. It was designed to replace a static chart with an interactive, screen-reader-accessible experience.

## Data Sources
The data used to populate this graphic is sourced from the Commonwealth of Massachusetts' official climate reporting:
* **Emissions (2021):** [Massachusetts Clean Energy and Climate Metrics](https://www.mass.gov/info-details/massachusetts-clean-energy-and-climate-metrics#ghg-emissions-snapshot)
* **CECP 2050:** [Clean Energy and Climate Plan for 2050 (CECP 2050)](https://www.mass.gov/info-details/massachusetts-clean-energy-and-climate-plan-for-2050)
* **FIA Data (2021):** [US Forest Service Forest Inventory and Analysis (FIA) Program](https://research.fs.usda.gov/programs/fia)

## Methodology & AI Generation
This graphic was generated in collaboration with Google Gemini. The development process involved:
1. **Data Interpretation:** Parsing complex emission inventory snapshots into individual units (1 symbol = 1 million metric tons of CO₂e).
2. **Interactive Logic:** Implementing JavaScript event listeners to create "Gestalt" grouping behavior, allowing users to hover over symbols to highlight entire sectors while dimming the rest.
3. **Accessibility (a11y):** Adding `aria-label` tags, keyboard navigation (`tabindex`), and a semantic "Implicit Legend" structure to ensure compliance with WCAG 2.1 AA standards.
4. **Responsiveness:** Using CSS Flexbox and media queries to ensure the side-by-side layout functions correctly across mobile, tablet, and desktop viewports within the StoryMap frame.

## Credits
* **Developer:** Alex Simmons
* **AI Collaborator:** Google Gemini