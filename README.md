# CryptoClustering
The aim of this challenge was to predict if 24 hr or 7 day price changes affect cryptocurrencies. Using unsupervised machine learning techniques, including K-means clustering and Principal Component Analysis (PCA). It also explores the impact PCA has on clustering techniques.

# Steps
1. Prepare the data (scale)
2. Find the best value for k using the original data
3. Cluster the cryptocurrencies with K-means using the original data and plot
4. Optimize the clusters with PCA
5. Find the best value for k using the PCA data
6. Cluster the cryptocurrencies with K-means using the PCA data and plot
7. Visualize and compare the results

# Results
1. Elbow curve for both the original data (blue) and the PCA data (red)
![Screenshot 2024-07-01 183545](https://github.com/nikimhenderson/CryptoClustering/assets/158214783/7bbe574a-a34e-444c-a826-94dea3a7f013) <br/>
The PCA curve (red) has lower inertia compared to the original data (blue). This indicates that the PCA data are more tightly clustered, indicating that they are more easily separable.
PCA transforms the data into a new representation using its principal components that are ordered by variance explained. Components that are retained are the most important (have the highest variance),
 while less important components (with lower variance) are discarded. Reduced dimensions lead to a clearer separation of the clusters because the variance that contributes less is minimized.

3. Scatterplot of the original data clusters
![Screenshot 2024-07-01 183607](https://github.com/nikimhenderson/CryptoClustering/assets/158214783/8dacecc6-c721-4073-b06a-2db9fc78d439)<br/>
There is some clear overlap in this scatterplot indicating that the original data is not as easily separable. This indicates that employing the original data with more features fails
to adequately capture the patterns of the data.

5. Scatterplot of PCA data clusters<br/>
![Screenshot 2024-07-01 183624](https://github.com/nikimhenderson/CryptoClustering/assets/158214783/8c5d6cf4-711e-415b-8347-91319ca31dfc)<br/>
The PCA data clusters are more easily separable, have clear separation compared to the original data. This indicates that the PCA data, using fewer features, has reduced the noise
coming from features that are less important, which leads to more distinct patterns in the data.

# Conclusion
After visually analyzing the data, the cluster analysis indicates that there are 4 distinct clusters. Using Principal Componenent Analysis we are able to see a more clearly defined set of clusters, whereas without PCA our clusters are less clear.
