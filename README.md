# Bitcoin Price Forecasting

This repository provides a solution for forecasting Bitcoin prices over the next two months using historical data. The task involves preprocessing the data, applying Linear Regression, and evaluating the model's performance.

---

## **Problem Description**

The goal is to forecast the value of Bitcoin for the next two months using Linear Regression. The following steps are followed:
1. Create a target column as the average of `low` and `high` values.
2. Preprocess the `date` column to a numerical format.
3. Use all other columns as features while dropping `open` and `close`.
4. Train the Linear Regression model with a 70-30 train-test split.
5. Evaluate the model using **Mean Absolute Error (MAE)** and **Mean Squared Error (MSE)**.
6. Visualize the regression line estimated by the model.

---

## **Implementation Steps**

### **1. Data Preparation**
- **Target Column**: Calculate the average of `low` and `high` as the target column.
- **Dropped Columns**: Remove `open` and `close` as they are strongly correlated with the target value.
- **Date Conversion**: Convert the `date` column into a numeric format (e.g., UNIX timestamp) for easier processing.

### **2. Model Selection**
- Use **Linear Regression** to predict the target variable.
- Optionally implement Linear Regression from scratch for deeper understanding.

### **3. Data Splitting**
- Split the data into training and testing sets in a **70:30** ratio.

### **4. Model Evaluation**
- Calculate **Mean Absolute Error (MAE)** and **Mean Squared Error (MSE)** on the test set.

### **5. Visualization**
- Plot the predicted regression line against the actual values.
