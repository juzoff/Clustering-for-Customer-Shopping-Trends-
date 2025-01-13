# Clustering-for-Customer-Shopping-Trends-
Analyzed the Customer Shopping Trends dataset using clustering to uncover patterns in purchasing behavior, preferred payment methods, and seasonal trends. Gained insights into customer segments to help businesses tailor marketing strategies, improve product offerings, and enhance customer experience.

---

## Components: 
### 1. Data Exploration and Initial Insights
- Loading the Dataset: Used pandas to load "shopping_trends_updated.csv" into DataFrame st.
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

![em](https://github.com/user-attachments/assets/a65407fa-b859-4a9f-a506-ac0e2ab72023)


### 3. Conducting Principal Component Analysis (PCA) and Visualization 
- Dimensionality Reduction:
  - PCA was used to reduce the feature space to 2 dimensions for easier visualization.
  - PCA components were calculated from the scaled features to capture the variance within the data in lower dimensions.

- Visualization:
  - Plotted the first two principal components with each point colored according to its cluster assignment, using matplotlib to create a scatter plot.
  - This visual representation helped in understanding how well-separated the clusters were in the reduced dimension space.

### 4. Summary of Analysis Steps and Results
- Process Overview:
  - From data loading and preprocessing, through clustering and dimensionality reduction, to visualization, each step was methodically executed to derive meaningful segments from the shopping trends data.
- Results:
  - Displayed mean values for each cluster, offering a quantitative summary of how different clusters behave or purchase.

### 5. Interpretation of Clusters, Insights, and Marketing Strategy Development
#### *Cluster 1: Accessory Enthusiasts
- Age: 44.21 (slightly older demographic)
- Purchase Amount (USD): 60.89 (moderate spending)
- Size, Season, Review Rating: Moderate values for size and season, slightly higher review ratings suggesting satisfaction.
- Subscription Status, Discount Applied, Promo Code Used: No use of subscriptions or discounts, indicating perhaps these customers are buying at full price due to brand loyalty or specific product interest.
- Previous Purchases: 25.64 (moderate history of purchases)
- Gender Distribution: More female (56%) than male (44%)
- Item Purchased: Strong preference for accessories like belts, handbags, jewelry, and sunglasses.
- Insights
  - This group shows a targeted interest in fashion accessories, possibly valuing quality or brand over price.
- Marketing Strategy/Strategic Actions:
  - Product Enhancement: Focus on premium accessory lines, exclusive designs.
  - Brand Loyalty Programs: Develop loyalty schemes tailored for accessory lovers, perhaps offering early access to new collections.
  - Influencer Marketing: Partner with fashion influencers who specialize in accessories to attract similar demographics.
  - Educational Content: Provide styling tips or accessory pairing guides to enhance customer engagement.

#### *Cluster 2: Clothing and Outerwear Enthusiasts
- Age: 43.70 (similar to Accessory Enthusiasts)
- Purchase Amount (USD): 59.99 (slightly less than accessories but still moderate)
- Size, Season: Moderate, with a clear focus on clothing and outerwear items.
- Review Rating: Slightly lower than Accessory Enthusiasts, suggesting room for improvement in satisfaction.
- Subscription Status, Discount Applied, Promo Code Used: No use of promotions, might be less price-sensitive.
- Previous Purchases: 24.77 (slightly less frequent than others)
- Gender Distribution: Balanced but slightly more female.
- Item Purchased: Dominance in clothing items like blouses, coats, jeans, etc.
- Insights:
  - This group has a wide interest in clothing, focusing on both everyday wear and outerwear.
- Marketing Strategy/Strategic Actions:
  - Seasonal Campaigns: Leverage seasonal changes with targeted outerwear promotions.
  - Fashion Trends: Keep up-to-date with fashion trends to offer what this group seeks in clothing.
  - Customer Feedback: Use feedback to improve product quality or fit, aiming to increase satisfaction.
  - Personalized Fittings: Offer virtual or in-store personalized fitting services.

#### *Cluster 3: Footwear Focused Shoppers
- Age: 44.44 (slightly older demographic)
- Purchase Amount (USD): 60.26 (slightly above average spending)
- Size, Season: Moderate, with a strong focus on footwear.
- Review Rating: Highest among clusters, indicating high satisfaction with footwear purchases.
- Subscription Status, Discount Applied, Promo Code Used: Some engagement with promotions, suggesting price sensitivity for footwear.
- Previous Purchases: 25.23 (consistent with other clusters)
- Gender Distribution: More male (67%) than female.
- Item Purchased: Exclusively focused on shoes, boots, sandals, and sneakers.
- Insights:
  - Specialization in footwear, with a preference for comfort or style in their purchases.
- Marketing Strategy/Strategic Actions:
  - Footwear Innovation: Invest in new materials or technologies for comfort and durability.
  - Comfort Campaigns: Market comfort alongside style, especially targeting male consumers.
  - Special Events: Host or sponsor running or walking events to promote footwear.
  - Loyalty Discounts: Offer loyalty points or discounts specifically for footwear purchases.

#### *Cluster 4: Promo-Driven Generalists (Male only)
- Age: 44.15 (consistent with other clusters)
- Purchase Amount (USD): 58.82 (lowest among clusters)
- Size, Season: Similar to others, with a broad range of items purchased.
- Review Rating: Similar to Clothing Enthusiasts, suggesting satisfaction but room for improvement.
- Subscription Status, Discount Applied, Promo Code Used: High engagement (1.00 for both discount applied and promo code used), indicating a highly price-sensitive group.
- Previous Purchases: 25.74 (highest among clusters, showing frequent purchases when incentivized)
- Gender Distribution: Exclusively male.
- Item Purchased: Spread across various categories but with a focus on clothing and accessories.
- Insights:
  - This group uses promotions to drive their buying decisions, showing cost-conscious behavior.
- Marketing Strategy/Strategic Actions:
  - Promotional Offers: Continuously offer deals and promotions to keep engagement high.
  - Exclusive Male Lines: Develop or promote lines specifically marketed to men, focusing on value.
  - Feedback Loop: Use this group's feedback to refine promotional strategies.
  - Cross-Selling: Use promotions to introduce new product categories to this group, leveraging their purchase frequency.
