
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

![alt text](https://github.com/cghimire/Bank-Marketing-Data-Mining/blob/master/Figures/Correlation_3.png "Correlation Plot")

*This plot demonstrates the correlation between different variables. There is no strong relation between predictors and predicted variable y, however, there is some relationship between predictor variable duration and predicted output y*.
![alt text](https://raw.githubusercontent.com/cghimire/Bank-Marketing-Data-Mining/master/Figures/Job_barplot.png "Job bar plot")

*This plot shows the number of clients Vs job category. The highest number of clients are from the job category "admin" followed by blue-color category. Similarly,
there are less students involved in the telemarketing campaign*.




## ⛏️ Data Preparation <a name = "data-preparation"></a>

![alt text](https://github.com/cghimire/Bank-Marketing-Data-Mining/blob/master/Figures/RemoveOutlier_%20campaignVariable.png "Outlier before and after")

*This figure compares the two different plots with outliers and without outliers*.

## 🚀 Data Modeling <a name = "data-modeling"></a>

In order to model the data, I am performing three data-mining classification techniques: 1) Logistic Regression 2)Decision Tree Model 3) Random Forest Model.

![alt text](https://github.com/cghimire/Bank-Marketing-Data-Mining/blob/master/Figures/Decision%20Tree_final.png "Decision Tree")


*This figure represents the decision tree structure. For example, If number of employed is greater than 5088, then that client belongs to NO category with 94% of probability: that means the client is more likely to say NO*.

## Model Evaluation and Conclusion <a name = "model-evaluation-and-conclusion"></a>

Put the important feature bar chart


![alt text](https://github.com/cghimire/Bank-Marketing-Data-Mining/blob/master/Figures/AccuracyVsTreeSize.png "Accuracy Vs Treesize")

*This figure shows Effect of increasing tree count on accuracy in Random Forest Model*.

I performed three different classification models to classify whether a customer would open a bank account or not. Based on the model build for this project, Decision Tree and Random Forest model are more accurate to predict the output. The Random Forest model is a recommended model for this classification problem.

Since I have been using different data mining techniques, I am expecting the proposed classification models are powerful to predict the output. However, the proposed methods has some limitations. It is not feasible to study all the variables in detail, which might be interesting to predict the output, because of time limitation.

