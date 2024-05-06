# CryptoClustering

## Background:

The following code is focused on data analysis using the K-means algorithm and principal component analysis (PCA) to classify cryptocurrencies according to their price fluctuations across various timeframes. Specifically, the code will examine price changes over intervals spanning 24 hours, 7 days, 30 days, 60 days, 200 days, and 1 year.

The code will require functions, libraries, dependencies, and import of a csv file. 
This code is available at Github under (https://github.com/algjor/CryptoClustering).

## Description of Code:
This code was completed using the following steps.

(1) - A repository was created called CryptoClustering in Git hub.

(2) - A starter code named Crypto_Clustering_starter_code.ipynb was created on the local Git repository and pushed to GitHub.

(3) - The csv file crypto_market_data.csv was imported for the data analysis.

(4) - The csv file was loaded into a Dataframe and indexed on "coin_id".

(5) - The data statistics was explored using the df.describe function to view the columns and data statistics.

(6) - The data was then normalized by scaling using the StandardScaler() module from scikit-learn with a dataframe created.

(7) - The best value for K was determined using the scaled dataframe and plotting the k-value.

(8) - Once the K-value was determined - this value was used to determined the predicted clusters for the data by suing the fit and predict functions.

(9) - To optimize clusters - the Principal Component Analysis was utilized to reduce features to three principal components and include in a dataframe.

(10) - The best value for K_pca was determined using the scaled dataframe and plotting the k-value.

(11) - The K_pca value was shown not to differ from the K-value of the original scaled data from the Elbow curves.

(12) - The features with the strongest positive and negative influence on each principal component was identified from the original data.

(13) - The key findings of the data analysis are:

    - Price change percentage 200d has the strongest positive influence on PCA1 at 59.4%.
    - Price change percentage 24h has the strongest negative influence on PCA1 at 41.6%.
    - Price change percentage 30d has the strongest positive influence on PCA2 at 56.2%.
    - Price change percentage 1y has the strongest negative influence on PCA2 at 15.0%.
    - Price change percentage 7d has the strongest positive influence on PCA3 at 78.7%.
    - Price change percentage 60d has the strongest negative influence on PCA3 at 36.1%.

