# CryptoClustering
## Machine Learning: K-means and Principal Component Analysis (PCA)

<img width="650" alt="image" src="https://github.com/Colex317/CryptoClustering/assets/148498483/e1c166fb-89fe-4432-ac72-762d7fb0a4de">




The CryptoClustering assignment focused on using K-means and Principal Component Analysis (PCA) in unsupervised machine learning. Python and unsupervised learning are used to predict whether cryptocurrencies are affected by 24-hour or 7-day price changes.

# Steps:
**Prepare the Data**
- `StandardScalar` and `scikit-learn` were used to normalize the data from the CVS file.
- A dataframe was then created with the scaled data, and the index was set `coin_id` from the original dataframe as the index of the new dataframe.

<img width="1595" alt="image" src="https://github.com/Colex317/CryptoClustering/assets/148498483/f46926fd-503e-4997-9497-307a3adca005">


**Find the Best Value for k Using the Original Scaled DataFrame**
- The elbow method was used to find the best value for `k.` Based on the Elbow Curve, the optimal k value was 4 for the given data.

<img width="790" alt="image" src="https://github.com/Colex317/CryptoClustering/assets/148498483/04760de3-0283-4d32-a5f1-70ce309b0675">



**Cluster Cryptocurrencies with K-means Using the Original Scaled Data**
- The original scaled dataframe was used to cluster the cryptocurrency for the best value for k.

<img width="784" alt="image" src="https://github.com/Colex317/CryptoClustering/assets/148498483/01b09b5f-bbc0-499a-91b1-5e669d1ddabf">



**Optimize Clusters with Principal Component Analysis**
- The original scaled dataframe was used to perform a PCA and reduce the features to three principal components. The total explained variance of the three principal components is approximately 90%.

<img width="580" alt="image" src="https://github.com/Colex317/CryptoClustering/assets/148498483/e21b8ad5-e981-496b-af35-16e2be901d9d">



**Find the Best Value for k Using the PCA Data**
- The elbow method was used on the PCA data to find the best value for k. Based on this Elbow Curve, it looks like `k=4` is still the correct one. There is no difference between this k value (using the PCA data) and the k value found using the original data.

<img width="788" alt="image" src="https://github.com/Colex317/CryptoClustering/assets/148498483/d526d58a-c3b9-4a26-98d9-4bdf68e8969d">



**Cluster Cryptocurrencies with K-means Using the PCA Data**
- The cryptocurrencies were clustered for the best value for k on the PCA data.

<img width="792" alt="image" src="https://github.com/Colex317/CryptoClustering/assets/148498483/514a2a7b-d041-4437-95fd-c8896dc8b900">

## References
HoloViz (2023). Composing Plots. Retrieved from https://holoviz.org/tutorial/Composing_Plots.html
Geekforgeeks (2022). Reduce Data Dimensionality using PCA – Python. Retrieved from https://www.geeksforgeeks.org/reduce-data-dimentionality-using-pca-python/
