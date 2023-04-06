# Cryptocurrencies

Using Unsupervised Machine Learning to cluster and analyze potential tradable cryptocurrencies for client.

## Overview

In this analysis, we analyzed a cryptocurrencies dataset using unsupervised machine learning since there is no known output of what we are looking for. The first thing we did is sorting through the dataset to identify the cryptocurrencies that are currently traded or mined. Once done, the data will be classified into groups based on our machine learning model. This analysis will then be displayed in several visualization graphs and plots to be used as references for client. This results will help determine posible crytocurrencies that would potentially be good for future investment.

The following methods were used for our analysis:
* Loaded, cleaned and preprocessed the dataset
* Reduced the data dimensions using Principal Component Analysis (PCA)
* Created cryptocurrency clusters using K-Means
* Created visual classification results using 2D and 3D plots

## Results

After preprocessing our dataset (only traded or mined crypto were selected, and any Null values are eliminated), we got a clean usable dataset contained 532 rows. We transformed any string data that cannot be processed by Machine Learning then scaled it down, and reducing to 3 dimensions or features using PCA methods

### Clustering Using K-Means

In order to successfully classify the crypto, we create Elbow Curve to determined the best K-values or number of clusters that we would identify. According to the graph below, we found that the best K-value is 4 (when we plot the curve for K from 0 to 10)

![image](https://user-images.githubusercontent.com/114631804/230492482-875354e7-727f-4b0c-bd24-0c38659bed3c.png)

### Clustered Tradable Crypto Table

We then ran the K-Means module with 4 clusters using 3 features to came up with the clustered table below with 532 tradable Cryptocurrencies

![image](https://user-images.githubusercontent.com/114631804/230494062-5b4350e7-acb4-4964-b2c3-606a4aa98f6b.png)

### 3D Scatter Plot with Clusters

This 3D graph show 3 dimensions or features of 4 different clustered groups after using PCA to reduce the dimensions from 95. It shows higher concentration in 2 classifications 1 and 2 with only few in 3 and 4.

![image](https://user-images.githubusercontent.com/114631804/230495384-062bf4dd-f80e-4fa8-be29-751b553d29be.png)

### 2D Scatter Plot with TotalCoinMined vs TotalCoinSupply

We used MinMaxScaler to scale the minimum and maximum values of the dataset to be 0 and 1 respectively, which provides a perfect visualization for the 2D graph. This shows the difference in potential of value of different classifications (Supply vs Demand).

![image](https://user-images.githubusercontent.com/114631804/230498191-53fcbe6d-5b4b-4c4b-b45b-8ae69adc1aff.png)


## Summary

Based on our analysis, we identified 532 potential tradable crytocurrencies. This crptos were then classified to 4 diferrent group using 3 features by Unsupervised Machine Learning Technique. However, in order to better understand and recommend these cryptocurrencies as future investment, we need to dive deeper into the dataset with using more features and more sophisticated methods, ie.deep learning.
