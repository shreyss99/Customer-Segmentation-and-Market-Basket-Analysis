# FLAIR: Finding Loyalists & Analyzing Item Relations
## Customer Segmentation and Market Basket Analysis on Online Retail Data

The 'Online Retail 2' is a transactional data set that contains all the transactions occurring between 01/12/2010 and 09/12/2011 for a UK-based and registered non-store online retail. The company mainly sells unique, all-occasion gifts. Many customers of the company are wholesalers.

But first, let's see some deep understanding of both concepts:

- **Customer segmentation** is the problem of uncovering information about a firm's customer base based on their interactions with the business. In most cases, this interaction is in terms of their purchase behavior and patterns. We explore some of the ways in which this can be used.
- **Market basket analysis** is a method to gain insights into the granular behavior of customers. This is helpful in devising strategies that uncover a deeper understanding of the purchase decisions taken by customers. This is interesting, as a lot of times even the customer will be unaware of such biases or trends in their purchasing behavior.


### Methodology
1. **Exploratory Data Analysis**: Understanding dataset features and preprocessing to ensure data quality.
2. **Preprocessing**: Handling missing values, removing outliers, and preparing data for analysis.
3. **Adding New Features**: Utilizing RFM (Recency, Frequency, Monetary Value) model to assess customer value.
4. **Customer Segmentation**: Employing K-means++, Agglomerative clustering, and DBSCAN to segment customers based on RFM features.
5. **Association Rule Mining**: Using Apriori and FP-Growth algorithms to discover associations between purchased items.
6. **Evaluation**: Assessing cluster quality and association rules using metrics like Silhouette score, Dunn Index, and lift.

### Results
- **Customer Segmentation**: Identified distinct customer segments based on purchasing behavior using K-means++, Agglomerative, and DBSCAN clustering methods. Low-engagement customers with low frequency and recency make up one of the clusters, which logically leads to lower spending levels. To try and entice these customers to keep returning and shopping on the platform, promotions and discounts are the perfect fit for them. The other cluster stands for devoted, high-spending clients who make more frequent purchases and are more recent in their purchases; these clients are worthy of loyalty benefits and retention initiatives.
  
- **Association Rule Mining**: Discovered frequent item sets and association rules using Apriori and FP-Growth algorithms, revealing common purchasing patterns. Based on the rules obtained from the algorithms, we can understand the frequent items that the customers generally purchase. The antecedents of the rules give us a good estimate as to what consequent items will have a high chance of being purchased along with it. Hence such rules can be useful recommendations for those products bought together which is equivalent to placing these products together in a physical store.

### Conclusion
The integrated approach of customer segmentation and market basket analysis informs targeted marketing strategies and enhances customer satisfaction. Future extensions may involve exploring additional algorithms for sequential pattern mining and integrating demographic data for more refined customer analysis.

## Instructions
1. Explore the dataset and ensure data quality through preprocessing.
2. Utilize clustering techniques to segment the customer base.
3. Apply association rule mining algorithms to uncover purchasing patterns.
4. Evaluate results using appropriate metrics and refine strategies accordingly.

**Note**:
- Ensure necessary libraries (e.g., pandas, scikit-learn) are installed for Python implementation.
- Refer to the provided code snippets and references for detailed implementation and analysis.
