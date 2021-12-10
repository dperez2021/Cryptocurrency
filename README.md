# Analysis of the Cryptocurrency Market

## Overview

The Purpose of this project is to create a report for an investment bank interested in offering a new cryptocurrency investment portfolio. The report includes what crpytocurrencies are on the trading market and hwo they could be grouped to create a classification system for this new investment. In order to complete this project, I will be performing unsupervised machine learning functions on data provided using CryptoCompare.

## Resources

- Data Source: crypto_data.csv, CryptoCompare
- Software: Python 3.7.7, Anaconda Navigator 1.9.12, Conda 4.8.4, Jupyter Notebook 6.0.3

## Results

I started by cleaning the data from the crypto_data.csv to only have cryptocurrencies that are actively trading, have a defined algorithm, and have a complete set of data. This left me with 532 different cryptocurrencies. 

We will produce the elbow curve below using the K-Means method iterating on k values from 1 to 10.

![ELBOW CURVE](https://user-images.githubusercontent.com/88256967/145496071-12203820-708f-4742-897f-7888b5cc5ded.PNG)


The best k value appears to be 4 so we would conclude on an output of 4 clusters to categorize the crpytocurrencies.

From there we created a 3-D graph to show how the different cryptocurrencies are grouped together. Each point includes its name as well as the algorithm used to create the cryptocurrency.

![3D SCATTER PLOT WITH CLUSTER](https://user-images.githubusercontent.com/88256967/145495872-01dcaeae-0044-432a-a0e4-1d1658c2bed6.PNG)

We then created a 2-D graph to shwo the relationship between total coin supply and total coines mined to show how each currency compares to the rest. Each point includes its currency name.

![TotalCoinsMines](https://user-images.githubusercontent.com/88256967/145495928-b983edca-59d5-4672-8b68-aa4dd37a6c3d.PNG)

Both these scatter plots show the distribution and the four clusters of cryptocurrencies.
We can identify the outliers like the unique cryptocurrency in the class #2.

## Tradeable CryptoCurrencies Table

![Table of CryptoCurrency](https://user-images.githubusercontent.com/88256967/145496840-df54cfb6-f6a0-403d-9406-7eab4aba8724.PNG)

Identifying the only cryptocurrency in class #2 we discover BitTorrent from table above.


## Summary

We have identified the classification of 532 cryptocurrencies based on similarities of their features. We should still analyze to more detail in order to determine the performance and potential interest for the investment bank's clients.

