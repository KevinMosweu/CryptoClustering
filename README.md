# CryptoClustering

## Description

In this challenge, knowledge of Python and unsupervised learning is used to predict if cryptocurrencies are affected by 24-hour or 7-day price changes.

## Steps

#### 1. Preparing the Data

Load the cryptocurrency data from the CSV and normalise the data.

#### 2. Determining the best number of clusters for the K-means model

Loop through a list of values from 1 to 11 for number of clusters, calculating the inertia of the K-means model of the data for each value. Plot inertia vs number of clusters and deterimine from the graph the best number of clusters.

#### 3. Clustering the cryptocurrencies data

Fit the cryptocurrencies data to a K-means model with the determined best number of clusters and make predictions on how the to cluster cryptocurrencies. Add those predictions to the original cryptocurrencies data and plot the 7 day price change percentage against the 24 hour price change percentage for the cryptocurrencies in a scatter plot, highliting clusters by colour.

#### 4. Optimizing data with Principal Component Analysis

Use PCA reduction on the normalised cryptocurrencies data to reduce the number of features of the data to 3 features.

#### 5. Determining the best number of clusters for the K-means model with PCA data

Repeat step 2 using the PCA reduced data instead to find the best number of clusters for this data.

#### 6. Clustering the PCA cryptocurrencies data

Repeat Step 3 using the PCA reduced data to make predictions for the clusters.

## Results

#### 1. Elbow Diagrams without and with Principal Component Analysis
![elbow_plot](https://github.com/KevinMosweu/CryptoClustering/assets/119974799/a2786aba-7881-4cb8-b50e-84d82cfef2ef)

![elbow_pca_plot](https://github.com/KevinMosweu/CryptoClustering/assets/119974799/d3920403-3344-402e-b57e-f6a77a9c84b1)


#### 2. Scatter Plots of clusters without and with Principal Component Analysis
![cluster_plot](https://github.com/KevinMosweu/CryptoClustering/assets/119974799/cf4a5332-5ab2-4cc9-9063-49d9db11d080)

![cluster_pca_plot](https://github.com/KevinMosweu/CryptoClustering/assets/119974799/059c2d69-26c9-45c0-94c6-23cbbaf4f4c6)


## Conclusion

The best number of clusters is 4 in both cases and the cluster scatter plot with the PCA predicted clusters has more overlap between clusters than the initial scatter plot. Using fewer features has made the clusters less clearly defined. Perhaps it would be better not to reduce the features.


