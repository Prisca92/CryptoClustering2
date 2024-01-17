# CryptoClustering2

In this challenge, I had to use my knowledge of Python and unsupervised learning to predict if cryptocurrencies are affected by 24-hour or 7-day price changes.

First I Prepared the Data

-Used the StandardScaler() module from scikit-learn to normalize the data from the CSV file. -Created a DataFrame with the scaled data and set the "coin_id" index from the original DataFrame as the index for the new DataFrame.

Found the Best Value for k Using the Original Scaled DataFrame which was 4.

Optimized Clusters with Principal Component Analysis -Using the original scaled DataFrame, perform a PCA and reduce the features to three principal components. -Retrieved the explained variance to determine how much information can be attributed to each principal component which was -Used the elbow method on the PCA data to find the best value for k using the following steps:

Cluster Cryptocurrencies with K-means Using the PCA Data by -Initializing the K-means model with the best value for k. -Fit the K-means model using the PCA data. -Predicting the clusters to group the cryptocurrencies using the PCA data. -Created a scatter plot using hvPlot

And finally answering the following question: What is the impact of using fewer features to cluster the data using K-Means? After analysing the cluster analysis results I noticed that some areas seem to remain the same when using the K-Means however, when using cluster plots the colors have changed.
