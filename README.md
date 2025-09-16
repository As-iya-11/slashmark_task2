# slashmark_task2
House Price Prediction using XGBoost
Description
This project utilizes machine learning techniques to predict house prices based on various features such as the number of bedrooms, square footage, year built, and location. The dataset used for training is kc_house_data1.csv. The model implemented is an XGBoost Regressor, which provides accurate price predictions. The goal is to analyze housing features and make data-driven price estimations.

Dataset Overview
The dataset consists of various house attributes, including:

bedrooms: Number of bedrooms
bathrooms: Number of bathrooms
sqft_living: Square footage of the living space
sqft_lot: Square footage of the lot
floors: Number of floors
waterfront: Whether the house is near a waterfront (binary)
view: Quality of the view
condition: Condition rating of the house
grade: Overall grade given to the house
yr_built: Year the house was built
yr_renovated: Year of the most recent renovation
zipcode: Zip code of the house
lat, long: Geographic coordinates
sqft_living15, sqft_lot15: Living and lot space of nearby houses
price (Target Variable): The house price to be predicted
Preprocessing Steps:
Handling Missing Values: Any missing data is removed to ensure consistency.
Feature Scaling: Standardization is applied to numerical features using StandardScaler.
Data Splitting: The dataset is split into training (80%) and testing (20%) sets.
Features Implemented
Data Preprocessing: Cleaning and transforming data for better model performance.
Model Training: Using XGBoost Regressor with:
n_estimators=100
learning_rate=0.1
max_depth=5
Prediction & Evaluation:
Mean Absolute Error (MAE): Measures average absolute difference between predicted and actual prices.
Mean Squared Error (MSE): Penalizes large errors more than MAE.
R-squared (R²) Score: Indicates how well the model explains the variance in prices.
Project Structure
├── dataset/                # Contains the house price dataset
├── house_price_prediction.py # Main Python script for training and evaluation
├── README.md               # Project documentation
└── requirements.txt        # Dependencies
Installation & Usage
Prerequisites
Python 3.x
Libraries: pandas, numpy, scikit-learn, xgboost
