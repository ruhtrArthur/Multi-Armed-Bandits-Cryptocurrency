# Optimizing Cryptocurrency Return Using Multi-Armed Bandits
Optimizing Cryptocurrency Return Using Multi-Armed Bandits - Personal Project 

#### Data: Cryptocurrency Historical Prices

Prices of top cryptocurrencies including Bitcoin, Ethereum, Ripple, Bitcoin cash
https://www.kaggle.com/sudalairajkumar/cryptocurrencypricehistory

![alt text](bike_share.jpg)

#### About this dataset:  

The dataset has one csv file for each currency. Price history is available on a daily basis from April 28, 2013. This dataset has the historical price information of some of the top crypto currencies by market capitalization. 

Date : date of observation <br>
Open : Opening price on the given day <br>
High : Highest price on the given day <br>
Low : Lowest price on the given day <br>
Close : Closing price on the given day <br>
Volume : Volume of transactions on the given day <br>
Market Cap : Market capitalization in USD

#### Contributor:

Arthur Qin <br>

#### Goal:

Things like Block chain, Bitcoin, Bitcoin cash, Ethereum, etc are constantly coming in the articles I read. I came across Multi-Armed Bandits in my Experiment Design class and want to see how I can optimize cryptocurrency portfolio return using multi-armed bandits. <br>

#### Process - Feature Engineering:

1. Cleaning and extracting variables to convert them to numeric values
2. Frequency encoding for some variables
3. One-hot encoding the categorical variables
4. Balanced the dataset 

#### Data Modeling:

Pipeline 
1. Simple Imputer with strategy='median'
2. Models fitted - Regularized Linear Regression, Decision Tree, Random Forest, Gradient Boosting
3. Hyperparameters tuning

#### Model Evaluation:

Compared various fitted model on basis on evaluation of validation set on metric: RMSE

#### Conclusion:

1. Gradient Boost outperformed the other models (Linear Regressions, Random Forest, XGBoost and Gradient Boost) for travel time prediction. <br>
2. Noises significantly impact results. By dropping misleading outliers, RMSE dropped over 75%. Consider changing evaluation metrics. <br>
3. Cross Validation on tree-based Spark ML takes long time, potentially due to how Spark ML optimizes splits of continuous variables. (approximating quantile instead of using exact splits) <br>
4. For Bike Riders : Optimize path according to duration <br>
5. For Bike Sharing Service Company: maintain the system in a balanced state (optimize docks for different stations)
