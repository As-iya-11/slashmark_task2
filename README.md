# 🏡 House Price Prediction using XGBoost

## 📌 Description
This project uses **machine learning** to predict house prices based on different features like number of bedrooms, square footage, year built, and location.  
The model is built using an **XGBoost Regressor**, which provides accurate price predictions.  
Dataset used: `kc_house_data1.csv`

The main goal is to analyze housing features and provide **data-driven price estimations**.

---

## 📊 Dataset Overview
The dataset contains several features of houses, including:

- `bedrooms`: Number of bedrooms  
- `bathrooms`: Number of bathrooms  
- `sqft_living`: Living area (square feet)  
- `sqft_lot`: Lot size (square feet)  
- `floors`: Number of floors  
- `waterfront`: Whether house is near a waterfront (0 or 1)  
- `view`: Quality of the view  
- `condition`: Condition rating of the house  
- `grade`: Overall grade given to the house  
- `yr_built`: Year built  
- `yr_renovated`: Year of most recent renovation  
- `zipcode`: Location zipcode  
- `lat, long`: Geographic coordinates  
- `sqft_living15`, `sqft_lot15`: Living and lot size of nearby houses  
- `price` (**Target Variable**): House price to be predicted  

---

## ⚙️ Preprocessing Steps
- **Handling Missing Values** → Removed missing data for consistency.  
- **Feature Scaling** → Standardized numerical features using `StandardScaler`.  
- **Data Splitting** → 80% Training, 20% Testing.  

---

## 🚀 Features Implemented
- **Data Preprocessing** → Cleaning and transforming data for better model accuracy.  
- **Model Training** → XGBoost Regressor with parameters:  
  - `n_estimators = 100`  
  - `learning_rate = 0.1`  
  - `max_depth = 5`  
- **Prediction & Evaluation** using metrics:  
  - **Mean Absolute Error (MAE)** → Average absolute error  
  - **Mean Squared Error (MSE)** → Penalizes large errors  
  - **R² Score** → Explains variance in predicted prices  

---

## 📂 Project Structure
├── dataset/ # Contains the house price dataset
├── house_price_prediction.py # Main script for training & evaluation
├── README.md # Project documentation
└── requirements.txt # List of dependencies
