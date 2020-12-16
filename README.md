# Price Prediction of Berlin Airbnb accommodation

Project created at April 2020.

The datasets contain detailed listings data of current Airbnb listings in Berlin. <br>
The goal is to predict the Price of accomodation by Summary information. (Regression problem)<br>
 <br>
The dataset has 22552 rows and 32 columns.
 <br>

References: <br>
[Kaggle Berlin Airbnb Data Sources](https://www.kaggle.com/brittabettendorf/berlin-airbnb-data) <br>
[Predicting Prices: XGBoost & Feature Engineering](https://www.kaggle.com/brittabettendorf/predicting-prices-xgboost-feature-engineering) <br>

#### Task: 

1. Check basic info of dataset
<br><br>
2. Deal with Outlinear and Missing Value

        a. Exclude outliner from price data
        b. deal with missing values of features
<br>
3. perform Exploratory Data Analysis (EDA)

        a. Location vs Price
        b. room and property type vs Price
        c. Price Differences on a minimum_nights, number_of_reviews, reviews_per_month, and availability_365
        d. Correlations between reviews

<br>
4. Data Preprocessing on features

        a. Transfer 'latitude' and 'longitude' to the 'distance' from center
        b. Transfer data "amenities"
        c. Transfer 'interaction', and 'instant_bookable' data into bool
        d. drop the columns that is not helpful for prediction
        e. convert all string columns into categorical or numerical data 
        f. One-hot encoding on categorical features

<br>
5. Build ML Models 

        a. Linear Regression
        b. Random Forest
        c. XGBoost Regressor
        
#### Prediction result on Testing Set

1. linear regressor: R^2 = 0.4191
2. Random Forest Regressor: R^2 =  0.5170
3. XGBoost Regressor: R^2 = 0.5622

![subsmission result](rhttps://github.com/vivianchang2019/Berlin_Airbnb_Price_Prediction/blob/master/result/Airbnb_feature_importance.JPG?raw=true)