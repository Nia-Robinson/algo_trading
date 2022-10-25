# TEAM ONE - PROJECT TWO "ALGO-TRADING MODEL"

![image](https://user-images.githubusercontent.com/108433370/196785794-1f9f88d8-44bf-47f6-9a6c-0ddb95b1e069.png)

Team Members:

Adam Cooke

Nia Robinson

Ros Tiamzon

============================================================================================

# PROJECT GOAL

We want to create an Algo-Trading model/platform that individuals can have access to (via subscription, etc.) at an affordable price, where they can choose a specific type of asset (stocks, funds, bonds, digital assets, derivatives, swaps, options, futures, forwards, etc), and match with or explore trading strategies they like, and make profit with their excess cash.

============================================================================================

# MODEL, TOOLS, LIBRARIES
This project leverages python 3.7 with the following packages:

* [Pandas](https://pandas.pydata.org/) - Pandas is a powerfull tool for data analysis and manipulation. Pandas provides a plethora of useful functions that make it easy to express, analyze, and manipulate data.

* [sk-learn](https://scikit-learn.org/stable/) - This is a machine learning library for the python programming language. This library allows for the use of multiple machine learning models, tools, and algorithms.

* [Hvplot](https://hvplot.holoviz.org/) - This Module provides a high-level potting API that allows for users to easily generate a wide array of plot types. HvPlot's main benefit is that it allows for very interactive visualizations.

* [Numpy](https://numpy.org/) - This module offers comprehensive mathematical functions, used for working with arrays. Numpy allows for seamlessand speedy integration with a wide variety of databases.

* [PyTorch](https://pytorch.org/) - PyTorch is a machine learning framework based on the Torch library, used for applications such as computer vision and natural language processing.

* [Yfinance](https://pypi.org/project/yfinance/) - Yfinance is a python package that enables us to fetch historical market data from Yahoo Finance API in a Pythonic way.

* [Finta](https://github.com/peerchemist/finta) - This module offers common financial technical indicators that can be implemented in Pandas.

* [matplotlib](https://matplotlib.org/) - Matplotlib is a comprehensive library for creating static, animated, and interactive visualizations in Python. 



============================================================================================

# ABOUT THE PROJECT

Our project is to create a profitable trading algorithm - model that anyone can use or subscribe to.

We selected 3 type of asset types (securities) i.e. index fund, futures contract and a digital asset (cryptocurrency) for analysis.

We also selected different trading strategies for the 3 different asset types. We used the momentum trading strategy for an exchange traded fund (SPY), pullback strategy for futures contracts, and bollinger bands for a cryptocurrency.

We calculated standard deviations, sharpe ratios and cumulative returns for each type of asset. 

We used SK-Learn and PyTorch libraries to create prediction models for future prices.

The ultimate project goal is to create a platform for users to be able to use to choose a specific type of asset, match with a trading strategy, predict prices and make a profit using our trading algo - model/platform.  


===========================================================================================

# DATA PREPARATION - MODEL TRAINING 

Step 1:

Take in the data via the Yfinance library and turn it into a data frame, calculate the necessary information based on the specific strategy used. PMAVG/VMAVG vs BB Lower-Upper

Step 2:

Determine  entry and exit points based on the calculations used (trading signals) and make a plot to help visualize the trading patterns.

Step 3: 

Use a for loop along with the entry and exit points to make an algorithmic trading process that also keeps track of profits and losses over time.

Step 4: 

COLLECT > SCALE > TRAIN - TEST- SPLIT > PREDICT

Step 5: 

Use a for loop to run the model and have it so that every 1000 epochs it prints out the model loss. Then plot the results of the model that compare the actual price vs the model’s predicted price.


===========================================================================================

# RESULTS

## 1) INDEX FUND S&P 500 (SPY)
Dataframe

![image](https://user-images.githubusercontent.com/107158380/196812002-2b5f071f-e5ac-4afa-9ba0-3a2078cf0fcd.png)


Graph of price, moving average price and moving average volume

![image](https://user-images.githubusercontent.com/108433370/196787488-3f8d8a6b-f5b1-463c-91c6-ddd9988d22bb.png)


Trading signals

![image](https://user-images.githubusercontent.com/107158380/196812733-59970961-4239-4c54-aac4-354c834824f6.png)


Graph of trading signals

![image](https://user-images.githubusercontent.com/108433370/196787577-c4f165be-5e15-4c6e-894e-595add04d2a1.png)


Details of loss/gain for the buy/sell (based on trading signals)

![image](https://user-images.githubusercontent.com/108433370/196787848-f7aee07e-322b-4ea1-8bd1-e4f8818dc813.png)


Results of Back Testing

![image](https://user-images.githubusercontent.com/107158380/196812327-51612b28-1f6d-4a31-a924-6b048ab289c1.png)

![image](https://user-images.githubusercontent.com/107158380/196812357-f8b14590-2c6d-4081-ac63-9af85103f3ef.png)


## 2) FUTURES CONTRACT (COMMODITY - ORANGE JUICE TICKER OJ=F) 

Dataframe

![image](https://user-images.githubusercontent.com/108433370/196789157-aa384dec-cbd6-4582-a3fa-0588b8b35ae2.png)

Graph of price, price action (assumed moving average price is the high water mark) and momentum/volume (assumed moving average volume as the momentum criteria)

![image](https://user-images.githubusercontent.com/108433370/196788407-9c646dc8-a7d7-4a53-8607-e34be3a16b02.png)

Trading signals

![image](https://user-images.githubusercontent.com/108433370/196788862-77fa7757-3024-4cf2-bbfc-695c9a328cc8.png)

Graph of trading signals

![image](https://user-images.githubusercontent.com/108433370/196788465-8897a9a0-379a-45f2-9e5e-20b3ab4ee3aa.png)

Details of loss/gain for the buy/sell (based on trading signals)

![image](https://user-images.githubusercontent.com/108433370/196788539-213f0eca-d861-4f55-a46f-4eedf2505fd4.png)


Results of back-testing

![image](https://user-images.githubusercontent.com/108433370/196788624-e09bc953-6d94-4f26-a357-0a9ef973cdec.png)
![image](https://user-images.githubusercontent.com/107158380/196811824-b586ab65-324d-4ea4-8bfa-40fb37a9ed88.png)





## 3) CRYPTOCURRENCY - BITCOIN 

Dataframe

![image](https://user-images.githubusercontent.com/107158380/196811171-5f973953-3be3-4365-ba21-255680a77c68.png)


Graph of price, and Bollinger bands

![image](https://user-images.githubusercontent.com/107158380/196811310-c968717f-a39f-4b0c-b25f-48a7fa7e4fec.png)


Trading signals

![image](https://user-images.githubusercontent.com/107158380/196811406-e6772eb0-2e42-4e6d-b7f9-12305ae0bfde.png)


Graph of trading signals

![image](https://user-images.githubusercontent.com/107158380/196811515-5e70ec36-629d-4849-807c-1ab8f3dd208a.png)


Details of loss/gain for the buy/sell (based on trading signals)

![image](https://user-images.githubusercontent.com/107158380/196811667-6e847060-2f10-445f-af65-61929c686066.png)

![image](https://user-images.githubusercontent.com/107158380/196811700-ae30361a-2a53-444b-8f4b-29c84fd7991b.png)


Results of back-testing

![image](https://user-images.githubusercontent.com/107158380/196810761-accbb1a8-70fb-4a9d-bea4-90f6b822b162.png)

![image](https://user-images.githubusercontent.com/107158380/196810817-aaaaa68a-1654-433c-9238-0ba1c17a444d.png)




