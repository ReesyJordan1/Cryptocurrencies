# Cryptocurrencies
## Overview
In this project, I am working on the crypto currency dataset. The goal of our analysis is to build a machine learning model to cluster similar crtypto currincies in the trading market together.

![intro.jpg](images/intro.jpg)

For this problem, the clustering algorith implemented is the KMeans algorithm. However, some data preprocessing needed to be done in order to start using the data. First, some filteration is done, then data encoding is applied using pandas `get_dummies()`. Afterwards, we applied standard scaling. Moreover, we reduced the data dimensionality using PCA into three principal components. Using these three principal components, we trained our KMeans model.

## Results

In this section we discuss the results found during conducting our analysis.

##### Using elbow method, we can see that k = 4 is recommended for this data
![elbow.png](images/elbow.png)

##### 3D scatter of the 3 pca components alognside with the KMeans predicstions
![ed.png](images/3d.png)

##### Scatter plot of x=TotalCoinsMined and y = TotalCoinSupply
![scaled.png](images/scaled.png)



## Summary

It's much easier to plot the data and visualize the results by employing the power of PCA in dimensionality reduction. Moreover, we found out that K = 4 is the best value for our KMeans model. Training the model using these principal components and with K = 4, we can group similar crypto currencies together.
