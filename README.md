# Clustering-for-Customer-Shopping-Trends-
Analyzed the Customer Shopping Trends dataset using clustering to uncover patterns in purchasing behavior, preferred payment methods, and seasonal trends. Gained insights into customer segments to help businesses tailor marketing strategies, improve product offerings, and enhance customer experience.

---

## Outcome - ***Development of 4 Consumer Clusters:***

#### Cluster 1: Footwear Focused Shoppers
- Purchase Patterns: The data shows 100% of purchases in the Footwear category (Category_Footwear = 1.0), emphasizing their focus on shoes. Items like boots (0.240401), sandals (0.267112), and sneakers (0.24207) are frequently bought, suggesting seasonal or activity-specific purchases.

#### Cluster 2: Accessory Enthusiasts
- Purchase Patterns: Exclusive purchase in Accessories (Category_Accessories = 1.000000) with items like belts, handbags, and sunglasses, supporting the notion of accessories as status or style symbols.

#### Cluster 3: Promo-Driven Generalists (Male only)
- Gender: Exclusively male (100% male), which fits with the description of strategic shopping behavior.
- Price Sensitivity: The 100% discount usage rate underscores their price sensitivity.
- Engagement: High subscription rate (62.20%) matches with being responsive to marketing communications to catch deals.
- Promo Code Used: The 100% promo code usage rate further describes this cluster.

#### Cluster 4: Clothing and Outerwear Enthusiasts
- Purchase Patterns: Focus on Clothing and Outerwear (84.82% and 15.18% respectively), with no discount usage, indicating a focus on quality or fashion over price.

---

## Components: 
### 1. Data Exploration and Initial Insights
- Loading the Dataset: Used pandas to load "shopping_trends_updated.csv" into DataFrames st and st2.
- Initial Data Inspection:
  - Displayed the first few rows with st.head() to see sample data entries.
  - Used st.info() to get an overview of data types, non-null counts, and memory usage, which helps in identifying data quality issues like missing values.

### 2. Standardization and Clustering Analysis
- Data Preprocessing:
  - Encoding: Applied Label Encoding for ordinal data and One-Hot Encoding for nominal data to convert categorical variables into a format suitable for clustering.
  - Standardization: Utilized StandardScaler to normalize the feature set, ensuring each feature contributes equally to the clustering process by having zero mean and unit variance.
- K-means Clustering:
  - Elbow Method: Plotted inertia versus the number of clusters to determine the optimal cluster count, aiming for a point where adding more clusters doesn't significantly reduce inertia.
  - Cluster Assignment: With 4 clusters chosen, K-means was applied to segment customers based on their shopping patterns.

### 3. Conducting Principal Component Analysis (PCA)
- Dimensionality Reduction:
  - PCA was used to reduce the feature space to 2 dimensions for easier visualization.
  - PCA components were calculated from the scaled features to capture the variance within the data in lower dimensions.

### 4. Clustering and Principal Component Analysis (PCA) Visualization
- Visualization:
  - Plotted the first two principal components with each point colored according to its cluster assignment, using matplotlib to create a scatter plot.
  - This visual representation helped in understanding how well-separated the clusters were in the reduced dimension space.

### 5. Summary of Analysis Steps and Results
- Process Overview:
  - From data loading and preprocessing, through clustering and dimensionality reduction, to visualization, each step was methodically executed to derive meaningful segments from the shopping trends data.
- Results:
  - Displayed mean values for each cluster, offering a quantitative summary of how different clusters behave or purchase.

### 6. Interpretation of Clusters, Insights, and Marketing Strategy Development
- 
