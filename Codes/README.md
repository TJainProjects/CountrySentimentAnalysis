Project Summary

This project focuses on **automated news scraping and classification** related to China's global engagements. It consists of two major components:



### Project Structure

#### 1. `SerpAPIScrapingInfo.ipynb`

* **Purpose**: Uses SerpAPI to scrape news articles related to Chinese diplomatic visits or global influence.
* **Key Steps**:

  * Sends search queries (possibly customized by date, country, or leader).
  * Collects metadata such as title, date, link, and snippet.
  * Cleans and stores the news dataset for analysis.

#### 2. `Theme_Classification.ipynb`

* **Purpose**: Classifies each news article into a thematic category (e.g., economic, political, symbolic) using NLP techniques.
* **Key Techniques**:

  * Zero-shot classification using a transformer model (possibly BART or RoBERTa via HuggingFace).
  * Custom label set (e.g., "Symbolic", "Economic", "Strategic").
  * Outputs labeled data for visualization or dashboarding.

---

### Suggested Reading Order

1. **`SerpAPIScrapingInfo.ipynb`** – Start here to generate the news dataset from Google search via SerpAPI.
2. **`Theme_Classification.ipynb`** – Next, classify the scraped data into meaningful categories for deeper analysis.

---

### Requirements

You’ll likely need:

```bash
pip install serpapi
pip install transformers
pip install pandas
pip install torch
```

Also ensure you have a valid **SerpAPI key** stored as an environment variable or directly used in the code.

---

### Outputs

* A CSV file or DataFrame with classified news articles including:

  * Title
  * Date
  * URL
  * Predicted theme (Symbolic/Economic/Strategic/etc.)



