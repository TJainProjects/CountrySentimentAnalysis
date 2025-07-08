# News Article Scraping Project - China Diplomatic Visits Media Analysis

## Overview

This project aims to collect and organize media articles related to the international diplomatic visits made by top Chinese leaders (e.g., President, Premier) over the last two decades. The scraped articles can be used for downstream tasks such as sentiment analysis, thematic classification, and understanding international media perception of China.

The core motivation stems from China’s growing global influence. While the main project tracks the **frequency and intensity of diplomatic trips**, this sub-project focuses on **how these visits are represented in international media**.

---

## Project Structure

### 1. `Codes/`

This folder contains all the Jupyter notebooks used for the scraping and transformation processes:

* **`SerpAPIScrapingInfo.ipynb`**: Utilizes the SerpAPI to scrape Google search results for news headlines and metadata. Handles API call structure and query formatting.
* **`Theme_Classificattion.ipynb`**: Prepares the collected articles for thematic classification using keyword-based filtering and topic extraction techniques.

>  Due to monthly API limits, scraping has been completed for only 20 countries so far. The code is modular and designed to scale easily with more countries once API quota is available.

---

### 2. `20CountryPilot.xlsx` (in `csv_data/` folder)

This Excel file includes preprocessed and aggregated results for 20 countries. It summarizes the headline content, associated metadata (date, country, query used), and thematic labels.

---

## How to Use This Repository

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/china-diplomacy-media.git
   ```

2. Open the `Codes/` folder and run the notebooks in the following order:

   * `SerpAPIScrapingInfo.ipynb`
   * `Theme_Classificattion.ipynb`

3. Use the data inside the `csv_data/` folder for visualization or further NLP tasks (e.g., zero-shot classification, sentiment analysis).

---

## Footnote

This news scraping pipeline is part of a broader project to track and understand China’s diplomatic engagements globally. The core project also includes:

* Mapping trip frequency by country and year
* Classifying the nature of visits (symbolic, economic, strategic)
* Creating interactive dashboards using Tableau

For now, this sub-project focuses solely on building a dataset of news articles related to diplomatic visits.

---

## Future Work

* Expand scraping to cover all countries.
* Integrate multilingual search to capture non-English media.
* Conduct large-scale sentiment and framing analysis.
* Link article sentiment with trip purpose and region.

---


I have added a Tableau visaualisaiton of the current output which can be accessed and viwed with this link:
Perception Monitor: https://public.tableau.com/app/profile/tanushree.jain6697/viz/PerceptionMonitorPilot/Dashboard1?publish=yes

