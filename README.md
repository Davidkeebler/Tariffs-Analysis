# U.S. Tariffs Analysis (2025) – K-Means Clustering of Country Trade Profiles

This project analyzes U.S. international trade and tariff policy by performing k-means clustering on a country-level dataset of trade deficits, imports, exports, and tariffs. All trade numbers are normalized on a per-capita basis using available population figures.

## Project Workflow

1. **Data Acquisition:**
   - Dataset downloaded from [Kaggle](https://www.kaggle.com/datasets/danielcalvoglez/us-tariffs-2025)
   - Population data merged to enable per-capita transformations

2. **Data Cleaning & Preprocessing:**
   - Outliers identified with IQR method
   - All numerical trade/tariff columns coerced to numeric dtype; non-numeric values handled
   - NaN rows dropped for clustering accuracy
   - Tariff percentage strings parsed into floats

3. **Exploratory Data Analysis:**
   - Distributions of per-capita trade values visualized by quantile
   - Boxplots, violin plots, and strip plots reveal disparities, outliers, and heterogeneous economic ties
   - ![](https://github.com/Davidkeebler/Tariffs-Analysis/blob/main/images/EDA.png)

4. **Feature Engineering:**
   - Key features engineered: US trade deficit, exports/imports (per-capita), tariffs (numeric)
   - Derived columns for trade balance and simple relationship classification

5. **K-Means Clustering:**
   - StandardScaler for normalization
   - Various k (number of clusters) tested using inertia and silhouette scores
   - Chosen model (k=4) labels each country with a cluster reflecting trade-tariff profile
   - Cluster assignment visualized and summarized
![](https://github.com/Davidkeebler/Tariffs-Analysis/blob/main/images/clusters.png)

6. **Outlier & Case Study Selection:**
   - Countries combining both high tariffs and large trade deficits identified
   - Top outliers by tariff and deficit plotted and analyzed
![](https://github.com/Davidkeebler/Tariffs-Analysis/blob/main/images/outliers.png)

7. **Interpretation & Limitations:**
   - Clusters interpreted in terms of trade strategy, surplus/deficit dynamics, and likely U.S. policy posture
   - *Major limitation:* Many key U.S. partners (notably China, Vietnam, etc.) are absent from the provided dataset, meaning the results do not reflect U.S. tariff strategy toward its main rivals.
![](https://github.com/Davidkeebler/Tariffs-Analysis/blob/main/images/deficit%20trade%20relationships.png)

## Main Findings
- Most countries fall into clusters of balanced trade and low-to-moderate tariff values
- The highest alleged tariff rates are observed almost exclusively among low-volume, minor trading partners
- Strong outliers and cluster structure reflect dataset composition as much as real policy; caution advised due to missing major target countries

## Limitations & Recommendations
- **Missing Data:** Absence of China, Vietnam, and other top-ten partners makes policy analysis incomplete
- **Utility of Clustering:** Methodology robust, but conclusive results require a more comprehensive dataset
- **Reuse:** The provided code framework is ready for replication with a better dataset

## How to Run
- 

---
*Contact the author for feedback or suggestions. The project uses Python (pandas, sklearn, matplotlib, seaborn) for full reproducibility.*