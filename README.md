MLB Pitching Analysis with Unsupervised Learning -> Full paper as MLB Analysis Report
This project explores MLB pitching performance using unsupervised learning techniques like Principal Component Analysis (PCA), Factor Analysis, and Clustering. By identifying archetypes of pitchers based on statistical metrics, this analysis aims to uncover insights into pitching effectiveness and propose strategies for building competitive teams on a budget.

Overview
The MLB is a multi-billion dollar industry, and pitching effectiveness is a critical determinant of team success. This project investigates patterns in pitcher performance using a dataset of 855 MLB pitchers from the 2024 season, focusing on metrics such as ERA, strikeouts per nine innings (K/9), WHIP, and walk rate.

By reducing the dataset's complexity with PCA, identifying latent structures with Factor Analysis, and grouping players into clusters using K-Means and PAM, this analysis provides actionable insights into pitcher archetypes and team-building strategies.

Key Features
Data Preprocessing:

Filtering players with fewer than 5 games played to remove outliers.
Converting textual data to numeric values for metrics like win percentages and runs scored per 9 innings.
Removing redundant or highly correlated features.
Exploratory Data Analysis (EDA):

Visualized distributions of key metrics like ERA, WHIP, and K/9.
Compared starting pitchers and relievers through boxplots and scatter plots.
Unsupervised Learning Techniques:

PCA: Reduced 108 features to 8 principal components explaining ~67% of the variance.
Factor Analysis: Identified three latent factors representing archetypes (e.g., starters, relievers, and struggling pitchers).
Clustering: Applied K-Means and PAM to group players into distinct clusters based on performance metrics.
Insights for Team Building:

Identified archetypes of high-performing, budget-friendly pitchers.
Provided recommendations for balancing starting and relieving roles in pitching rotations.
Dataset
The dataset contains 108 features and 855 rows of MLB pitchers from the 2024 season. Key metrics include:

ERA (Earned Run Average): A measure of runs allowed per nine innings pitched.
WHIP (Walks and Hits per Inning Pitched): Indicates pitching efficiency.
K/9 (Strikeouts per Nine Innings): Reflects strikeout ability.
Additional features related to game performance, situational metrics, and team success.
Preprocessing Steps:
Filtered for players with at least 5 games played.
Standardized data for PCA and Factor Analysis.
Removed columns with near-zero variance and high correlation.
Methods
1. Principal Component Analysis (PCA):
Transformed high-dimensional data into uncorrelated components.
The first two components explained the most variance, representing archetypes like "high-performance starters" and "low-contact pitchers."
2. Factor Analysis:
Identified three factors representing archetypes:
Starters: Players with high innings pitched, games started, and low walks per plate appearance.
Struggling Pitchers: Players with high SLG and ERA.
Relievers/Closers: Players excelling in high-pressure game finishes.
3. Clustering:
Used K-Means and Partition Around Medoids (PAM) for grouping.
Three clusters revealed:
Cluster 1: Ineffective pitchers.
Cluster 2: Consistent, high-performing starters.
Cluster 3: Relievers/closers with situational effectiveness.
Results
PCA identified archetypes such as "non-hittable pitchers" and "reliable starters."
Clustering highlighted budget-friendly high-performers like Andrew Abbott ($1.3M/year) compared to stars like Hunter Greene ($8M/year).
Factor Analysis confirmed the clear separation between starters, relievers, and struggling pitchers.
