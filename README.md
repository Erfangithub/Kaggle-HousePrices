# Kaggle-HousePrices

## Contents
1. About this project: Predicting House Prices in Ames, Iowa
2. Installation

## 1. About this project: Predicting House Prices in Ames, Iowa

- The goal in this Kaggle project is to predict the House Prices based on 79 explanatory
variables that describe (almost) every aspect of residential homes in Ames, Iowa.
Link to the official page for this project: https://www.kaggle.com/c/house-prices-advanced-regression-techniques
- There is a Jupyter notebook regarding this project in this repository named:
  - HousePrices.ipynb
- This notebook contains a summary of my analysis for this project. At first we preprocess the data for machine learning
with a few simple steps. Using this preprocessed data we train promising machine learning models. And finally these models
are stacked to create a meta-model which makes the final predictions. Some details of the analysis (e.g. fine-tuning hyper
-parameters) are not shown. There are a few outliers in the data which heavily affect the final prediction error if not
treated separately, therefore we make separate predictions for these outliers.
- These steps are sufficient to obtain a Root-Mean-Squared-Error (RMSE) between the logarithm of the predicted value and the
logarithm of the observed sales price of about 0.1175 which puts the submission in the Top 4% on the Public Leaderboard.

## 2. Installation
- #### Requirements to run this project
  - Python 3 and Jupyter notebook need to be installed before running this project.
  - The python libraries used in this project are listed in the requirements.txt file and are as follows:
    - numpy
    - pandas
    - matplotlib
    - scikit-learn
    - xgboost
    - lightgbm
  - You can install these libraries by running the following in a terminal application (assuming conda is installed):
  
    $ conda install -c conda-forge --file requirements.txt
  
    - To install the packages one at a time you can run the following in a terminal application:
  
    $ conda install -c conda-forge packagename1
  
    - Where packagename1 can be replaced with numpy, pandas, matplotlib, scikit-learn, xgboost or lightgbm. For the first
      four packages the following command can also be used:
  
    $ pip install packagename2
  
    - Where packagename2 can be replaced with numpy, pandas, matplotlib or scikit-learn.
    
    - Note: pip or pip3 commands might also work (although there were some issues on my system) for installing xgboost or lightgbm.
      The installation commands that I have written above are the ones that worked on my MacBook Pro.
      
- #### Download the data
  - Download the zip file containing this repository.
  - Unzip the file and get into the folder named: Kaggle-HousePrices-master , via a terminal application.
  - Launch a Jupyter notebook and run the notebook related to this project!
