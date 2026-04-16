# 🏨 Hotel Reviews Analysis — NLP & Geospatial Visualization

An end-to-end data analysis project that applies **Natural Language Processing (NLP)** and **geospatial visualization** to a large dataset of European hotel reviews. The goal is to surface actionable insights from customer feedback and present them on an interactive map.

---

## 📌 Project Overview

This project processes thousands of hotel reviews to extract sentiment patterns and key themes, then visualizes the results geographically using interactive maps. It demonstrates a full NLP pipeline — from raw text cleaning through to browser-based map exploration.

**Dataset:** [515K Hotel Reviews in Europe](https://www.kaggle.com/datasets/jiashenliu/515k-hotel-reviews-data-in-europe) — Kaggle

---

## 🔍 Key Features

- **Text Preprocessing** — Tokenization, stopword removal, and text normalization
- **Sentiment Analysis** — Positive/negative scoring of individual reviews
- **Topic Modeling** — Identifying recurring themes across thousands of reviews
- **City Extraction** — Parsing structured city names from raw hotel address strings
- **Interactive Geospatial Map** — Folium-powered map with clickable hotel markers showing aggregated review data and sentiment scores

---

## 📁 Repository Structure

| File | Description |
|------|-------------|
| `Hotel Review Analysis.ipynb` | Core NLP pipeline: preprocessing, sentiment analysis, and topic modeling |
| `Extracting City from Address and plotting using Folium.ipynb` | Parses city names from addresses and generates the interactive map |
| `Folium - Map_Plots.ipynb` | Additional map visualization experiments |
| `Hotel_Addresses_only.csv` | Extracted hotel address data |
| `city_data.csv` | Processed city-level aggregated data |
| `Hotel_Reviews_Interactive_Map.html` | Rendered interactive Folium map (open in browser) |

---

## 🛠️ Technologies Used

- **Python** (Jupyter Notebooks)
- **pandas**, **NumPy** — Data manipulation
- **NLTK** / **spaCy** — NLP preprocessing and sentiment analysis
- **scikit-learn** — Topic modeling (LDA)
- **Folium** — Interactive geospatial maps
- **Matplotlib** / **Seaborn** — Exploratory data visualization

---

## 🚀 Getting Started

### Prerequisites

```bash
pip install pandas numpy nltk folium matplotlib seaborn scikit-learn
```

### Running the Analysis

1. Clone the repository:
   ```bash
   git clone https://github.com/Hemanth-Mydugolam/Hotel-Reviews-Analysis.git
   cd Hotel-Reviews-Analysis
   ```

2. Download the dataset from [Kaggle](https://www.kaggle.com/datasets/jiashenliu/515k-hotel-reviews-data-in-europe) and place it in the project root.

3. Run the notebooks in order:
   - Start with `Hotel Review Analysis.ipynb` for the NLP pipeline
   - Then run `Extracting City from Address and plotting using Folium.ipynb` for geospatial visualization

4. Open `Hotel_Reviews_Interactive_Map.html` in your browser to explore the interactive map.

---

## 🗺️ Interactive Map

The output map (`Hotel_Reviews_Interactive_Map.html`) lets you:
- Browse hotels pinned across European cities
- Click on markers to view aggregated review counts and sentiment scores
- Explore geographic patterns in guest satisfaction

---

## 📊 Analysis Workflow

```
Raw Reviews
    │
    ▼
Text Cleaning & Tokenization
    │
    ▼
Sentiment Scoring (per review)
    │
    ▼
Topic Modeling (LDA)
    │
    ▼
City Extraction from Addresses
    │
    ▼
Geospatial Aggregation
    │
    ▼
Interactive Folium Map
```

---

## 📄 License

This project is open source. Dataset is sourced from Kaggle and subject to its original license terms.