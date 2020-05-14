# Optimizing Cryptocurrency Return Using Multi-Armed Bandits
Optimizing Cryptocurrency Return Using Multi-Armed Bandits - Personal Project 

#### Data: Cryptocurrency Historical Prices

Prices of top cryptocurrencies including Bitcoin, Ethereum, Ripple, Bitcoin cash
https://www.kaggle.com/sudalairajkumar/cryptocurrencypricehistory

![alt text](Bitcoin.jpg)

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

#### Process:

I performed 500 rounds of simulations to determine which arm has the highest return in each simulation. In each bandit approach, I balanced between exploitation and exploration to maximize our cumulative return and minimize the regret. For each simulation, I assumed I invested $1 per day on a single token and determine how much return it can generated with that single token using different bandit algorithms. 

#### Algorithms Used:

1. Epsilon Greedy
2. Softmax
3. Upper Confidence Bound
4. Thompson Sampling

#### Evaluation:

Compared various fitted model on basis on evaluation of validation set on metric: cumulative reward/return

#### Conclusion:

After 500 rounds of simulations, the upper confidence bound algorithm gave us the highest reward out of the four algorithms.
