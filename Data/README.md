# 20 Country Pilot – News Classification Dataset

This folder contains the output of a pilot project focused on scraping and classifying news related to China’s global diplomatic and economic engagements across **20 selected countries**.

## Contents

- `20CountryPilot.xlsx`: Compiled dataset of news articles for 20 countries.
  - Each sheet corresponds to a specific country.
  - Columns include article title, snippet, date, and **classified theme** (e.g., Symbolic, Economic, Strategic).

## Methodology

- Data was scraped using **SerpAPI** with Google News queries for each country.
- Thematic classification was done using **zero-shot learning** with a Hugging Face transformer model (`facebook/bart-large-mnli` or equivalent).
- Themes used:
  - `0 = No Info`
  - `1 = Symbolic`
  - `2 = Economic/Diplomatic`
  - `3 = Strategic`

## Limitations

- Due to **SerpAPI's monthly API call limits**, only **20 countries** were processed.
- Countries were scraped and processed **individually** in separate notebook runs, then compiled manually.
- The process used is **brute-force** but easily extendable to additional countries or custom queries.

## How to Extend

- Add more country names to the search query list.
- Run the same scraping and classification pipeline (see `SerpAPIScrapingInfo.ipynb` and `Theme_Classification.ipynb` in the main repo).
- Append the results to this Excel file or compile into a new dataset.

## Note

This pilot serves as a **proof of concept** and a **template** for larger-scale thematic media tracking and analysis related to China's international diplomacy.





