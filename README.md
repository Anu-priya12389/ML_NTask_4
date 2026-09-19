# ML Task 4 – Household Energy Consumption Prediction

## 📌 Project Overview

This project predicts **household energy consumption** using **Polynomial Regression**.

The model uses household-related and usage-related features to predict the total energy consumption in kWh.

## 🎯 Objective

The main objective of this project is to:

* Analyze the household energy consumption dataset.
* Handle missing values.
* Select important input features.
* Apply Polynomial Regression.
* Predict energy consumption.
* Evaluate the model using different performance metrics.
* Compare actual and predicted energy consumption.

## 📂 Dataset

The dataset used in this project is:

**Household Energy Consumption Dataset**

### Features Used

The following features are used as input variables:

* `Household_Size`
* `Avg_Temperature_C`
* `Peak_Hours_Usage_kWh`

### Target Variable

* `Energy_Consumption_kWh`

The target variable represents the total household energy consumption in kWh.

## 🛠️ Technologies Used

* Python
* Pandas
* Matplotlib
* Scikit-learn
* Google Colab / Jupyter Notebook

## 🔄 Workflow

1. Import the required Python libraries.
2. Load the CSV dataset.
3. Check the dataset shape.
4. Display the first few records.
5. Analyze the dataset information and statistics.
6. Check for missing values.
7. Remove rows containing missing values.
8. Select input features and target variable.
9. Split the dataset into training and testing sets.
10. Apply Polynomial Features with degree 2.
11. Train a Linear Regression model using the polynomial features.
12. Make predictions on the test data.
13. Evaluate the model.
14. Display actual and predicted energy consumption.
15. Visualize the actual vs predicted values.

## 🤖 Model Used

### Polynomial Regression

Polynomial Regression is used to model the relationship between the input features and energy consumption.

In this project:

* Polynomial degree = **2**
* Test size = **20%**
* Random state = **42**

The polynomial features are generated using:

```python
PolynomialFeatures(degree=2)
```

A Linear Regression model is then trained using these transformed features.

## 📊 Model Evaluation

The model is evaluated using the following metrics:

### 1. MAE – Mean Absolute Error

Measures the average absolute difference between the actual and predicted values.

### 2. MSE – Mean Squared Error

Measures the average squared difference between actual and predicted values.

### 3. RMSE – Root Mean Squared Error

It is the square root of MSE and represents the prediction error in the same unit as the target variable.

### 4. R² Score

Measures how well the model explains the variation in the target variable.

## 📈 Visualization

A scatter plot is created to compare:

* **Actual Energy Consumption**
* **Predicted Energy Consumption**

The plot helps to visually understand how closely the predictions match the actual values.

## 📋 Output

The notebook produces:

* Dataset information
* Descriptive statistics
* Missing-value information
* Polynomial Regression model
* MAE
* MSE
* RMSE
* R² Score
* Actual vs Predicted Energy Consumption table
* Actual vs Predicted scatter plot

## 📁 Project Structure

```text
ML_NTask_4/
│
├── ML_NTask_4.ipynb
├── household_energy_consumption.csv
└── README.md
```

## ✅ Conclusion

In this project, Polynomial Regression is applied to predict household energy consumption using household size, average temperature, and peak-hours usage.

The model performance is evaluated using MAE, MSE, RMSE, and R² score, and the actual and predicted values are visualized using a scatter plot.
