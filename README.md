# Car Price Prediction & Recommendation System

## Project Overview

This project is a complete Machine Learning system that predicts car prices and provides intelligent recommendations based on user input.

It is designed to simulate a real-world car marketplace where users can:

* Predict car prices
* Understand price factors
* Find cars within a budget
* Compare cars
* Get best value recommendations
* Discover similar cars
* Predict future depreciation

---

## Objectives

The main goals of this project are:

* Build a machine learning model for car price prediction
* Provide explainability of predictions
* Create recommendation systems based on user needs
* Simulate real-world business logic using data science

---

## Dataset Information

The dataset used in this project contains information about different cars, including:

* Make & Model
* Engine details (HP, Cylinders)
* Fuel type
* Transmission
* Mileage (city & highway)
* Vehicle size & style
* Popularity
* MSRP (used as Price)

### Important Note

The **Price (MSRP)** values in this dataset are **not real market prices**.

* The dataset contains **inconsistent and unrealistic price ranges**
* Some cars have very low prices (e.g. below 5000)
* No cars exceed around 100,000

Therefore:

> All predictions and recommendations are based on **dataset-specific values**, not real-world pricing.

---

## Technologies Used

* Python
* Pandas & NumPy
* Scikit-learn
* XGBoost (optional)
* Matplotlib (for EDA)
* Google Colab

---

## Machine Learning Models

The following models were trained and evaluated:

* Linear Regression
* Random Forest ✅ (Best Performance)
* XGBoost

### Evaluation Metrics

* R² Score
* Mean Absolute Error (MAE)

---

## Features Implemented

### Car Price Prediction

Predicts the price of a car based on user input features.

### Price Explanation

Shows important features affecting the predicted price using feature importance.

### Budget-Based Recommendation

Returns cars within a given price range.

### Car Comparison System

Compares two cars based on:

* Price
* Engine performance
* Mileage
* Age

Also suggests which car is better.

### Best Value Car Finder

Finds the best car under a budget using a custom scoring formula:

Score = (Engine HP + Mileage) / (Price × Car Age)

### Similar Cars Recommendation

Uses KNN (Nearest Neighbors) to find cars similar to a selected car.

### Depreciation Predictor

Predicts future car price based on increasing car age.

---

## Data Preprocessing

* Handling missing values
* Feature engineering:

  * Car Age
  * Mileage
  * HP per Cylinder
* One-Hot Encoding for categorical variables
* Feature scaling using StandardScaler
* ColumnTransformer + Pipeline used for clean workflow

---

## Exploratory Data Analysis (EDA)

Performed analysis on:

* Price distribution
* Price vs Year
* Price vs Mileage
* Brand-wise average price


---

## Limitations

* Dataset contains unrealistic price values
* Model is not trained on real market data
* Depreciation prediction is simulated, not time-series based


