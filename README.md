# Cryptocurrencies

## Overview

Martha is a senior manager for the Advisory Services Team at Accountability Accounting, was tasked to create a report that includes what cryptocurrencies are on the trading market and how they could be grouped to create a classification system for a new investment. She has decided to use unsupervised machine learning and to group the cryptocurrencies, by using clustering algorithm.

## Purpose

The purpose of this analysis includes:

- Preprocessing the Data for PCA

- Reducing Data Dimensions Using PCA

- Clustering Cryptocurrencies Using K-means

- Visualizing Cryptocurrencies Results

## Resources

Data souces: crypto_data.csv, CryptoCompare

Data tools: Python 3.7.6, Jupyter Notebook, sklearn, plotly, hvplot

## Results

### Preprocessing the Data for PCA
By using Pandas, we preprocess the dataset in order to perform PCA. A new DataFrame is created that stores all cryptocurrency names from the CoinName column and retains the index from the crypto_df DataFrame. The below image shows the crypto_df DataFrame:

![]()

### Reducing Data Dimensions Using PCA
Using the Principal Component Analysis (PCA) algorithm, we reduce the dimensions of the X DataFrame to three principal components and place these dimensions in a new DataFrame. A new DataFrame named pcs_df was created that includes the following columns, PC 1, PC 2, and PC 3, and uses the index of the crypto_df DataFrame as the index.The below figure shows the dataframe:

![]()

### Clustering Cryptocurrencies Using K-means

With K-means algorithm, we will create an elbow curve using hvPlot to find the best value for K from the pcs_df DataFrame. Then, we will run the K-means algorithm to predict the K clusters for the cryptocurrencies’ data.The following image shows the new clustered_df dataframe:

![]()

### Visualizing Cryptocurrencies Results

#### 3D-Scatter plot 

We create a 3D scatter plot using the Plotly Express scatter_3d() function to plot the three clusters from the clustered_df DataFrame.

![]()

The below image shows us the table for tradable cryptocurrencies:

![]()

#### 2D-Scatter plot 

In order to create a 2D-Scatter plot of TotalCoinMined vs TotalCoinSupply, a new dataframe was created containing these columns, and CoinNames and Class columns from the previous dataset.

![]()

The below image shows the 2D-Scatter plot. 






