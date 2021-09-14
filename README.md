# Ames-House-Price-Prediction-with-Advanced-Regression-Techniques

This competition is very important to me as it helped me to begin my journey on Kaggle few months ago.
Competition link: https://www.kaggle.com/c/house-prices-advanced-regression-techniques

![Competition Banner](https://github.com/arnabx007/Ames-House-Price-Prediction-with-Advanced-Regression-Techniques/blob/master/banner.jpg"")

About the dataset: Compared to the **Boston Housing Dataset** the **Ames Housing Dataset** is a large dataset with a total of around 2900+ observations and packed with 80 feature variables ('Boston Dataset' has 506 observations and only 14 variables). In the dataset there are,

* 20 continuous variables (relate to various area dimensions for each observation),
* 14 discrete variables (quantify the number of items occurring within the house),
* 46 categorical variables (23 nominal, 23 ordinal)

Read more about the dataset here: http://jse.amstat.org/v19n3/decock.pdf

It's a dataset packed with a lot of features of every type and a wide range of variations and problems in them. Hence getting a good score in this competition requires advanced EDA & modelling skills.

I have applied the following feature Engineering techniques here:

* **Imputing missing values** by analaysing each of the features seperately without dropping any of them
* **Removing extreme outliers** from the training data using both univariate & bivariate analysis
* **Transforming** ordinal features to numerical (i.e. label encoding) and numerical variables to categorical where necessary
* **Adding new features** both numerical and discrete/boolean special features
* **Analysing skewness** of the numerical features
* **Box Cox Transformation** of skewed features (instead of log-transformation because boxcox yield to slightly better models)
* **One-hot encoding** the nominal categorical variables

I have tried several ML algorithms and in the end stacking & ensembling approches:

* **Lasso (L1) Regression**
* **Ridge (L2) Regression**
* **ElasticNet**
* **Gradient Boosting** (xgboost, lightgbm etc.)
* **Averaging** all/selected base models
* **Model Stacking** with a meta regressor
* **Model blending** by assigning different weights to different models

After approaching and experimenting with all the above techniques my final LB score was 0.11994 (top 2% on the leaderboard the last time I submitted: September, 2020)

![LB](https://github.com/arnabx007/Ames-House-Price-Prediction-with-Advanced-Regression-Techniques/blob/master/LB.jpg"")
