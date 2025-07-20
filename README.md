# Used-Car-price-prediction-using-Linear-and-Lasso-Regression-models


Predicting used car prices using Linear and Lasso Regression models. Includes data preprocessing, feature encoding, model training, evaluation with R² and MAE, and    visualizations. Lasso Regression outperformed Linear Regression in terms of accuracy.
Here's a clean and professional README file you can paste directly into your GitHub repository for the **Car Price Prediction using Linear and Lasso Regression** 

This project demonstrates how to predict the selling price of used cars using machine learning models—specifically **Linear Regression** and **Lasso Regression**. The project involves data preprocessing, model training, evaluation, and visualization.

## Table of Contents

* [Overview](#overview)
* [Dataset](#dataset)
* [Technologies Used](#technologies-used)
* [Data Preprocessing](#data-preprocessing)
* [Model Training & Evaluation](#model-training--evaluation)
* [Results](#results)
* [How to Run](#how-to-run)
* [Conclusion](#conclusion)

---

## Overview

Used car prices can vary based on a number of factors such as year, fuel type, transmission, and mileage. This project aims to predict the price using two regression techniques:

* **Linear Regression**
* **Lasso Regression**

The dataset is cleaned and preprocessed, categorical variables are encoded, and both models are evaluated using metrics like R² score and Mean Absolute Error (MAE).

---

## Dataset

The dataset contains information about used cars and includes the following features:

* Car\_Name
* Year
* Selling\_Price (Target)
* Present\_Price
* Kms\_Driven
* Fuel\_Type
* Seller\_Type
* Transmission
* Owner



## Technologies Used

* Python 3
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Scikit-learn



## Data Preprocessing

* Checked for missing values
* Converted categorical variables to numerical (e.g., Fuel\_Type, Seller\_Type, Transmission)
* Dropped unnecessary columns like `Car_Name`
* Split data into features (`X`) and target (`y`)
* Performed a train-test split (90% training, 10% testing)


## Model Training & Evaluation

Two models were trained:

### 1. Linear Regression

* Trained on the processed dataset
* Evaluated using R² score and MAE for both training and testing data

### 2. Lasso Regression

* Also trained on the same dataset
* Provided slightly better error metrics, making it a more suitable choice

---

## Results

Evaluation Metrics:

| Model             | R² Score (Train) | MAE (Train) | R² Score (Test)  | MAE (Test) |
| ----------------- | ---------------- | ----------- | ---------------- | ---------- |
| Linear Regression | \~0.87 (example) | Varies      | \~0.84 (example) | Varies     |
| Lasso Regression  | Higher than LR   | Lower       | Higher than LR   | Lower      |

Visualizations include scatter plots comparing **actual** vs **predicted** prices for both training and testing datasets.

---

## How to Run

1. Make sure Python and the necessary libraries are installed:

   ```bash
   pip install numpy pandas matplotlib seaborn scikit-learn
   ```

2. Place the dataset `car data.csv` in the appropriate path.

3. Run the Python script:

   ```bash
   python car_price_prediction_using_linear_and_lasso_regression_models.py
   ```

4. The script will output model performance metrics and visualizations.


## Conclusion

Both Linear and Lasso Regression models can predict car prices reasonably well. However, Lasso Regression showed slightly better performance in this case. This project demonstrates the importance of choosing the right regression technique based on evaluation metrics.



