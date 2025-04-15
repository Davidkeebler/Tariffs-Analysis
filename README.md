
# Tarrifs Analysis Project

## Goal
The primary aim of this project is to analyze U.S. trade relationships using k-means clustering, focusing on how tariffs affect these relationships. By organizing countries into distinct profiles based on trade metrics normalized per capita, we aim to understand the efficacy and potential impacts of U.S. tariffs.

## Methodology
1. **Data Collection and Preparation**: We used a dataset containing U.S. trade figures, including exports, imports, and deficits, normalized per capita to ensure fair comparisons across countries regardless of population size.
2. **Exploratory Data Analysis (EDA)**: The dataset was examined for outliers and trends using statistical methods and visualizations. Outliers based on trade metrics were identified using the interquartile range to understand exceptional trading circumstances or economic anomalies.
3. **Normalization and Clustering**: Trade figures were normalized by population, followed by k-means clustering to group countries into three clusters based on their trade profiles.
4. **Analysis by Cluster**: The clusters were analyzed to understand trade balances, political relationships, and the potential impact of tariffs on each group.

## Political Implications
![](https://github.com/Davidkeebler/Tariffs-Analysis/blob/main/images/clusters.png)
- **Cluster 0** involves countries largely favoring U.S. exports with minimal imports. The political relationship is stable, with tariffs having limited strategic leverage.
- **Cluster 1**'s profile shows dependency on U.S. imports, highlighting potential diplomatic leverage for the U.S.
- **Cluster 2** reveals countries with balanced trade, where tariffs could strategically shift the equilibrium or enhance domestic resilience.

## Results
![](https://github.com/Davidkeebler/Tariffs-Analysis/blob/main/images/deficit%20trade%20relationships.png)
- **Cluster 0**: This group had high trade deficits favoring the U.S., suggesting these countries export minimally to the U.S.; thus, tariffs may have a limited economic impact.
- **Cluster 1**: Countries in this cluster had high per capita trade deficits, favoring other countries, indicating dependency on U.S. imports, allowing for strategic tariff leverage.
- **Cluster 2**: Exhibiting moderate deficits or balanced trade, tariffs here could adjust economic equilibrium, influencing trade patterns significantly in either enhancing domestic capacities or straining economic ties.
![](https://github.com/Davidkeebler/Tariffs-Analysis/blob/main/images/outliers.png)

## Future Work
1. **Broader Economic Indicators**: Incorporate GDP growth, inflation rates, and unemployment statistics for a well-rounded analysis.
2. **Longitudinal Study**: Track trade dynamics and tariff impacts over time to measure evolving trends.
3. **Policy Simulation**: Develop predictive models to test potential economic and political outcomes under various tariff scenarios.
4. **Missing Information**: The dataset is missing critical import and export information for certain countries, reducing the quality of the analysis.

Overall, the analysis provided insights into the U.S.'s strategic trade positions and the effectiveness of tariff policies in potentially enhancing economic influence without destabilizing existing trade relations. 