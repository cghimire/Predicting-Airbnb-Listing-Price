
<p align="center">
  <a href="" rel="noopener">
 <img width=200px height=200px src="https://i.imgur.com/6wj0hh6.jpg" alt="Project logo"></a>
</p>

<h3 align="center">Predicting Airbnb listing Price</h3>

<div align="center">

</div>

---

<p align="left"> This project aims to use machine learning models to predict the base price for properties, and also to explore Airbnb listing data, in order to help Airbnb hosts maximize their earnings.
    <br> 
</p>

## 📝 Table of Contents
- [About](#about)
- [Data Exploration and Preparation](#data_exploration_and_preparation)
- [Data Modeling and Model Evaluation](#data-modeling)

## 🧐 About <a name = "about"></a>
Airbnb is a home-sharing platform that allows home-owners and renters ('hosts') to put their properties ('listings') online, so that guests can pay to stay in them. Hosts are expected to set their own prices for their listings. Although Airbnb and other sites provide some general guidance, there are currently no free services which help hosts price their properties.

Airbnb pricing is important to get right, particularly in big cities like London where there is lots of competition and even small differences in prices can make the difference between optimum occupancy and high earnings, or being priced out of the market. It is also a difficult thing to do correctly, in order to balance the price with occupancy (which varies inversely with price) in order to maximise revenue.

This project aims to use machine learning models to predict the base price for properties, and also to explore Airbnb listing data, in order to help Airbnb hosts maximize their earnings.

![alt text](https://github.com/cghimire/Predicting-Airbnb-Listing-Price/blob/master/Figures/Airbnb%20Search.png "Search Options")

## 🎈 Data Exploration and Preparation <a name="data_exploration_and_preparation"></a>

![alt text](https://github.com/cghimire/Predicting-Airbnb-Listing-Price/blob/master/Figures/metadata.png "Metadata")

*Metadata of the data which contains 20677 records (rows) and 106 features (columns). There are some missing values and I applied imputation method to handle those missing values. After I cleaned the date, dimension of the data is reduced to 13837 rows and 24 columns* 

![alt text](https://github.com/cghimire/Predicting-Airbnb-Listing-Price/blob/master/Figures/download.png "Plot categorical features")
*From the above histogram, it can be seen that one column only contain one category and can be dropped*

![alt text](https://github.com/cghimire/Predicting-Airbnb-Listing-Price/blob/master/Figures/price_distribution.png "Distribution of price")

*We see the distribution for pricing is strongly skewed right. This makes sense as a majority of the listings on Airbnb are single individual listings and Airbnb does strongly cater to travelers who are looking for cheaper places to stay for short durations of time*.

## Correlation: 

![alt text](https://github.com/cghimire/Predicting-Airbnb-Listing-Price/blob/master/Figures/Correlation.png "Correlation")

Correlation matrix shows that price column has positive correlation with beds, bedroom, and accommodates but are not highly correlated (less than 0.50).


## 🚀 Data Modeling and Model Evaluation <a name = "data-modeling"></a>
I used Random Forest and Neural networks model to predict listing price


![alt text](https://github.com/cghimire/Predicting-Airbnb-Listing-Price/blob/master/Figures/RMSE.png "RMSE")

The easier metric to understand is the mean absolute error, this means that our predictions were perfect but on average 39.28 away from the true prediction with the random forest model. Our model’s MAE is 39.28, which is fairly small given that our data’s PRICE range from 0 to about 2000.


RMSE is the difference between model predictions and true values. We get the RMSE value about 76: which means this model is better to predict the airbnb price. We can create models with different hyperparameters tuning to try and boost performance.

## Feature Selection:

![alt text](https://github.com/cghimire/Predicting-Airbnb-Listing-Price/blob/master/Figures/Feature%20Selection.png "Feature selection")

Based on my random forest regtression model, we can see that the amenities and accommodates are top 2 important features to predict price. Which makes sence because these two features are important to determine the listing price.

## Neural Network

The score return the coefficient of determination R^2 of the prediction. R square compares the fit of the chosen model with that of a horizontal straight line (the null hypothesis). If the chosen model fits worse than a horizontal line, then R square is negative. So, this is not a best fit model to predict the listing price.

## Future Plan

Due to time constraints, I couldn't able to do indepth analysis of all the features. If I get a chance to do further analysis in the future, I will perform some others ML models such as XGBoost to compare the best fit model to predict listing price. I tried to use XGBoost, but I got error while importing XGBoost library in my MacOS.

To further improve our models, I could include more feature engineering, for example time-based features.
