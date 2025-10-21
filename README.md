# California House Price Prediction using Linear Regression

## Project Overview

This project focuses on predicting median house prices in California using the **California Housing dataset**.
It applies **supervised machine learning** techniques to build a **Linear Regression model** that captures the relationship between various housing features (like average income, house age, and population) and the target variable — **median house price**.
The project demonstrates a complete machine learning workflow including data preprocessing, visualization, model training, and evaluation.

## Workflow

### 1. Data Loading

* The dataset is imported using `sklearn.datasets.fetch_california_housing()`.
* It contains **20,640 samples** and **8 numerical features** such as median income, average rooms, average bedrooms, population, and latitude/longitude.
* The target variable (`PRICE`) represents the **median house value** in units of $100,000.

### 2. Exploratory Data Analysis (EDA)

* A **distribution plot** shows the variation of house prices.
* A **correlation heatmap** helps visualize relationships among different features and the target variable.
* These visualizations help identify which features are most influential in predicting house prices.

### 3. Data Preprocessing

* The data is split into **training (80%)** and **testing (20%)** subsets using `train_test_split`.
* Features are **standardized** using `StandardScaler` to normalize values and improve model performance.

### 4. Model Building

* A **Linear Regression model** is trained using the scaled training data.
* This algorithm fits a linear relationship between the independent variables (features) and the dependent variable (price).

### 5. Model Evaluation

* The trained model is evaluated on the test data using the following metrics:

  * **Mean Squared Error (MSE)** – measures average squared difference between actual and predicted prices.
  * **Root Mean Squared Error (RMSE)** – indicates the model’s prediction error in real units.
  * **R² Score** – explains the proportion of variance in the target variable captured by the model.
* A **scatter plot** of actual vs predicted prices visualizes model performance.

## Techniques Used

* Supervised Learning (Regression)
* Feature Scaling (Standardization)
* Model Evaluation Metrics (MSE, RMSE, R²)
* Data Visualization (Distribution Plot, Correlation Heatmap, Scatter Plot)

## Libraries and Tools

| Library      | Purpose                                                         |
| ------------ | --------------------------------------------------------------- |
| NumPy        | Numerical computation                                           |
| Pandas       | Data manipulation and analysis                                  |
| Matplotlib   | Data visualization                                              |
| Seaborn      | Statistical plotting                                            |
| Scikit-learn | Dataset handling, preprocessing, model training, and evaluation |

## Results

* The Linear Regression model successfully predicts house prices with good accuracy.
* Correlation analysis reveals **median income** as the most significant predictor of housing prices.
* Visual comparisons between actual and predicted prices show a strong positive relationship.
