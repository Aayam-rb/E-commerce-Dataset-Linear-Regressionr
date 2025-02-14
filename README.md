# Linear Regression Model for Predictions

## Project Overview
This project demonstrates how to use a Linear Regression model to predict values based on an e-commerce dataset. The dataset contains information on customers who purchase clothes online after receiving personalized styling advice. Customers engage in virtual styling sessions via video calls or chat-based consultations, where professional stylists provide tailored fashion recommendations. After the session, customers can browse and order suggested clothing items through the store’s mobile app or website at their convenience.

## Features
- Load a dataset using Pandas
- Preprocess and transform data for model input
- Train a Linear Regression model using Scikit-Learn
- Predict values for new data
- Save the updated dataset with predictions

## Dataset
The dataset captures details such as:
- **Customer Email**: Unique identifier for customers
- **Address**: Customer's location
- **Avatar**: Profile representation
- **Avg. Session Length**: Average length of a user session
- **Time on App**: Time spent on the mobile app
- **Time on Website**: Time spent on the website
- **Length of Membership**: Duration of user membership
- **Yearly Amount Spent**: Total spending by the customer
- **new_prediction**: Predicted spending value added to the dataset

## Problem Statement
"Should the company focus on improving its mobile app or website experience to maximize customer spending?"

## Installation & Requirements
Ensure you have the following libraries installed before running the project:
```bash
pip install pandas scikit-learn numpy
```

## How to Use
1. Load the dataset:
```python
import pandas as pd
new_data = pd.read_csv('predict_data.csv')
```
2. Preprocess and transform the data (if needed).
3. Predict values using a trained model:
```python
new_data["new_prediction"] = model.predict(new_data_transform)
```
4. Save the updated dataset:
```python
new_data.to_csv("predict_data_with_predictions.csv", index=False)
```

## Output
The final dataset includes a new column `new_prediction` containing the model's predicted values.



