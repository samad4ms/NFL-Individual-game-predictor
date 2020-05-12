# NFL-Individual-game-predictor
As my second NFL project, this one differs in that it attempts to predict the winning team of individual games with more sophisticated feature engineering and algorithmic modeling.

Data used: I web-scraped NFL game data, vegas odds, and team power rankings for the years 2009-2015 to create a dataset unlike anything that is publicly available. If you would like access to this dataset, please contact me.

Main files in this repo:

1) MODELING phase 2.ipynb<br>
This notebook contains the main feature engineering. Here I split the master dataframe into home and away tables, and then created exponential moving average features (EMA) to extract more signal from the trends that may have developed in previous games.

2) FINAL_MODELS.ipynb <br>
Here I predicted the individual game outcomes with Logistic regression, SVM and XGboost alogirthms. I avoided data leakage by preserving the chornology of the data while grid searching parameters, training and testing. The final models predict the correct game winner roughly 64% of the time. 

