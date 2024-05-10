# CryptoClustering

## Challenge Overview: Utilize Python and unsupervised learning techniques to predict whether cryptocurrencies are influenced by 24-hour or 7-day price changes.

## Data Preparation:
Load the data from the "crypto_market_data.csv" file into a DataFrame.
Examine summary statistics and plot the data to understand its distribution.
Normalize the data using StandardScaler() from scikit-learn.
Create a new DataFrame with the scaled data, retaining the "coin_id" index.
## Finding Optimal k:
Employ the elbow method to determine the best value for k.
Iterate through a range of k values (1 to 11), computing the inertia for each.
Plot a line chart to visualize the inertia values and identify the optimal k.
Answer the question: What is the best value for k?
## Clustering with K-means:
Initialize a K-means model with the optimal k value.
Fit the model to the original scaled DataFrame and predict clusters.
Create a scatter plot using hvPlot, coloring points by cluster labels.
Add "coin_id" in hover data to identify each cryptocurrency.
## Principal Component Analysis (PCA):
Perform PCA on the original scaled DataFrame, reducing features to three principal components.
Determine the explained variance for each principal component.
Create a new DataFrame with PCA data, retaining the "coin_id" index.
## Finding Optimal k with PCA Data:
Apply the elbow method on PCA data to find the best k value.
Plot the inertia values for different k values.
Answer the question: What is the best k value when using PCA data? Does it differ from the original data?
## Clustering with K-means using PCA Data:
Initialize K-means with the optimal k from PCA.
Fit the model to PCA data and predict clusters.
Plot a scatter plot similar to the original data's, using PCA features.
Answer the question: What is the impact of using fewer features to cluster the data using K-Means?
