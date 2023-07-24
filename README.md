# Crypto-Clustering
Unsupervised learning to predict if cryptocurrencies are affected by 24-hour or 7-day price changes.

The Crypto_Clustering.pynb Jupyter notebook reads crypto currency data from the crypto_market_data.csv in the Resources folder. Here are the steps to   
1. Data is scaled first and then a determine the the number of clusters using the elbow curve method.
2. Create the cluster predictions using K-means
3. Plot the clusters in two dimensions, x-axis: price_change_percentage_24h and y-axis: price_change_percentage_7d
4. Reduce dimensions to 3 principle components
5. Determine the numbe of clusters using the elbow curve method
6. Use K-Means to for cluster prediction
7. Plot the clusters in two dimensions, x-axis: PC1, y-axis:PC2.

!(Contrasting the clusters)[]

### Summary
Clusters 0 and 1 are more close to each other after using PCA. With fewer features, the outliers are more cleary defined in their own cluster, for example, the crypto 'celsius-degree-token' has a clear separation with PCA. With the orginal features cluster allocation for 'celsius-degree-token' seems artibitrary at least in 2 dimensions. However, there some loss of information when using PCA, the total explained variance is 89.5%, with PC1 covering 37.2%, PC2 covering 34.7%, and PC3 covering 17.6% respectively.