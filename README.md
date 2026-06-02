# Cryptocurrency Market Behavioral Pattern Identification

> Final Year Project · Institut Teknologi Sepuluh Nopember (ITS) Surabaya · 2025

Identifying behavioral patterns in cryptocurrency markets using unsupervised machine learning clustering methods, based on price and trading volume data from 2020 to 2024.

---

## Overview

This project applies and compares four unsupervised clustering algorithms to identify distinct behavioral patterns across major cryptocurrencies. By analyzing historical market data, the study aims to uncover recurring market regimes such as bullish, bearish, or sideways trends that can support data-driven decision making in financial markets.

**Cryptocurrencies Analyzed:** Bitcoin (BTC) · Ethereum (ETH) · Solana (SOL) · Ripple (XRP)

**Period:** 2020 – 2024

---

## Clustering Methods

| Method | Type | Key Characteristic |
|---|---|---|
| **K-Means** | Partitional | Centroid-based, efficient for large datasets |
| **DBSCAN** | Density-based | Handles noise and outliers well |
| **GMM** | Probabilistic | Soft clustering with cluster probability |
| **Spectral Clustering** | Graph-based | Captures non-convex cluster shapes |

---

## Repository Structure

```
clustering-cryptocurrency-analysis/
│
├── clustering cryptocurrency analysis.ipynb   ← Main analysis notebook
├── crypto_market_data_2020_2024.csv           ← Dataset (2020–2024)
│
├── hasil_clustering_final.csv                 ← Final clustering results
├── evaluasi_model.csv                         ← Model evaluation metrics
│
├── dashboard_clustering_full.png              ← Full clustering dashboard
├── metrik_internal.png                        ← Internal evaluation metrics
├── metrik_eksternal.png                       ← External evaluation metrics
├── tsne_spectral.png                          ← t-SNE visualization (Spectral)
│
└── timeseries_{COIN}_{METHOD}.png             ← Time series plots per coin per method
    ├── timeseries_BTC_KMeans.png
    ├── timeseries_BTC_DBSCAN.png
    ├── timeseries_BTC_GMM.png
    ├── timeseries_BTC_Spectral.png
    └── ... (ETH, SOL, XRP variants)
```

---

## Methodology

```
Raw Data (CSV)
     ↓
Exploratory Data Analysis (EDA)
     ↓
Data Preprocessing & Feature Engineering
     ↓
Clustering (K-Means · DBSCAN · GMM · Spectral)
     ↓
Cluster Evaluation
  ├── Internal Metrics (Silhouette Score, Davies-Bouldin, Calinski-Harabasz)
  └── External Metrics (Rand Index, Adjusted Rand Index)
     ↓
Visualization & Pattern Interpretation
```

---

## Results

Model evaluation results are stored in `evaluasi_model.csv`. Visualizations include:

- Time series clustering plots for each cryptocurrency × method combination (16 plots total)
- Internal and external metric comparisons across all four methods
- t-SNE dimensionality reduction plot for Spectral Clustering
- Full clustering dashboard (`dashboard_clustering_full.png`)

---

## Tech Stack

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat&logo=jupyter&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat&logo=numpy&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=flat&logo=scikit-learn&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557c?style=flat&logo=python&logoColor=white)

---

## How to Run

```bash
# 1. Clone the repository
git clone https://github.com/agnespriscilla/clustering-cryptocurrency-analysis.git
cd clustering-cryptocurrency-analysis

# 2. Install dependencies
pip install pandas numpy scikit-learn matplotlib seaborn jupyter

# 3. Open the notebook
jupyter notebook "clustering cryptocurrency analysis.ipynb"
```

---

## Author

**Agnes Priscilla Sekartaji Hadikusuma**
S1 Teknik Informatika · Institut Teknologi Sepuluh Nopember (ITS) Surabaya

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/agnespriscilla33)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white)](https://github.com/agnespriscilla)
[![Email](https://img.shields.io/badge/Email-D14836?style=flat&logo=gmail&logoColor=white)](mailto:agnes.priscilla33@gmail.com)
