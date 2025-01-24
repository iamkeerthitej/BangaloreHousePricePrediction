# Bangalore Housing Price Prediction

This code is a machine learning project using TensorFlow and other Python libraries to predict house prices. Here's a breakdown of the main sections:

## 1. Importing Libraries:
   - The necessary libraries such as NumPy, Pandas, Matplotlib, Seaborn, Warnings, TensorFlow, and scikit-learn are imported.

## 2. Loading Dataset:
   - The dataset is loaded from a CSV file named 'house2.csv' using Pandas. The dataset used is taken from Kaggle [A link to the original dataset](https://www.kaggle.com/datasets/amitabhajoy/bengaluru-house-price-data/data).

## 3. Exploratory Data Analysis (EDA):
   - A sample of the dataset is displayed, and basic information like shape and null values are checked.
   - Categorical columns like 'area_type', 'location', 'availability', and 'society' are dropped.
   - A distribution plot of the 'price' column and a heatmap of correlations between 'bath', 'balcony', and 'price' are visualized.

## 4. Data Cleaning:
   - Null values in the 'size', 'bath', 'balcony', and 'total_sqft' columns are addressed.
   - The 'size' column is processed to convert it into a numeric format.
   - 'bath' and 'balcony' columns are filled with mean values.
   - 'total_sqft' column is processed to handle different formats and missing values.

## 5. Model Implementation:
   - The dataset is split into features (X) and the target variable (y).
   - Standard scaling is applied to the features using scikit-learn.
   - A simple neural network model is created using TensorFlow's Keras API with input, hidden, and output layers.
   - The model is compiled using the Adam optimizer and mean squared logarithmic error loss.
   - It is trained on the training data and evaluated on the test data.

## 6. Model Usage:
   - The user is prompted to input the number of bedrooms, bathrooms, balconies, and total square footage for a new house.
   - The model is then used to predict the price of the house based on the provided inputs.

This code essentially performs data cleaning, exploratory data analysis, and implements a basic neural network model for predicting house prices based on given features. The model is trained and tested, and then it's used to make predictions for new input values.
