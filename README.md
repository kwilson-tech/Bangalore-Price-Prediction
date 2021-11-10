# Bangalore-Price-Prediction

Price prediction for the city of Bangalore in India. Mainly used XGBoost to predict the prices of residences. Used Geopy to convert the given address feature to the latitude/longitude of the given location. I’m not familiar with the domain of Bangalore and used KMeans Clustering in place of the latitude/longitude to group attributes according to their areas. Used Yellowbrick (elbow method) to calculate the optimal number of clusters in place of the address.

The originators of the dataset stated that their were unconfirmed values, so I created different models to see what would give the best results. 
* For the 1st model, I replaced unconfirmed values with 0's which gave very poor results.
* For the 2nd model, I removed the columns of those unconfirmed values and the results turned out very poor.
* For the 3rd model, I removed the rows that gave unconfirmed values and those gave pretty accurate results compared to the previous models. 

Libraries used:
* Numpy/Pandas/Matplotlib/Seaborn
* Sklearn
* Yellowbrick
* XGBoost
* Geopy/Folium

The dataset can be found on Kaggle. You can click [here](https://www.kaggle.com/ruchi798/housing-prices-in-metropolitan-areas-of-india).

References:

https://heartbeat.comet.ml/working-with-geospatial-data-in-machine-learning-ad4097c7228d
