
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
- [Data Modeling](#data-modeling)
- [Model Evaluation and Conclusion](#model-evaluation-and-conclusion)

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


## 🚀 Data Modeling <a name = "data-modeling"></a>
I used Random Forest and Neural networks model to predict listing price


![alt text](https://github.com/cghimire/Predicting-Airbnb-Listing-Price/blob/master/Figures/RMSE.png "RMSE")

The easier metric to understand is the mean absolute error, this means that our predictions were perfect but on average 40.25 away from the true prediction with the random forest model. Our model’s MAE is 39.28, which is fairly small given that our data’s PRICE range from 0 to about 2000.


RMSE is the difference between model predictions and true values. We get the RMSE value about 76: which means this model is better to predict the airbnb price. We can create models with different hyperparameters tuning to try and boost performance.



## Model Evaluation and Conclusion <a name = "model-evaluation-and-conclusion"></a>

Put the important feature bar chart


![alt text](https://github.com/cghimire/Bank-Marketing-Data-Mining/blob/master/Figures/AccuracyVsTreeSize.png "Accuracy Vs Treesize")

*This figure shows Effect of increasing tree count on accuracy in Random Forest Model*.

I performed three different classification models to classify whether a customer would open a bank account or not. Based on the model build for this project, Decision Tree and Random Forest model are more accurate to predict the output. The Random Forest model is a recommended model for this classification problem.

Since I have been using different data mining techniques, I am expecting the proposed classification models are powerful to predict the output. However, the proposed methods has some limitations. It is not feasible to study all the variables in detail, which might be interesting to predict the output, because of time limitation.

## Future Plan

Due to time constraints, I couldn't able to do indepth analysis of all the features. If I get a chance to do further analysis in the future, I will perform some others ML models such as XGBoost to compare the best fit model to predict listing price. I tried to use XGBoost, but I got error while importing XGBoost library in my MacOS.

To further improve our models, I could include more feature engineering, for example time-based features.
