# JobSalaryPredictor

## README for Salary Years Model

This repository contains code for a model that predicts salary based on years of experience. The code is written in Python and uses the `pandas` and `numpy` libraries.

**Here's a breakdown of the code:**

* **Importing Libraries:**
  * `pandas (pd)`: Used for data manipulation and analysis.
  * `numpy (np)`: Used for numerical computations.
  * `matplotlib.pyplot (plt)' : Used for data visualization.

* **Data Preprocessing:**
  1. Reads the CSV file named "Salary_Data.csv" using `pd.read_csv`.
  2. Missing Values have been checked for by using info and describe methods giving a description of how many null values are counted.

* **Model Training:** 
  * Algorithm: The model uses Linear Regression from scikit-learn to predict salary based on years of experience.
  * Data Splitting: The code assumes you've already split your data into training and testing sets.The data is split into training (80%) and testing(20%) sets (X_train, y_train) for model fitting.
  * Model Fitting: The reg.fit(X_train, y_train) line fits the linear regression model to the training data. X_train represents the features (years of experience) and y_train represents the target variable (salary). The model learns the relationship between these features and targets.

* **Evaluation:** 
  * Prediction: The model predicts salary on the unseen test data using y_pred = reg.predict(X_test).
  * Visualization: The code creates two scatter plots:
  * Training Set: This plot visualizes the actual salary (y-axis) vs years of experience (x-axis) for the training data (green dots). It also overlays the predicted salary     line (blue line) based on the fitted model.
  * Test Set: Similar to the training set plot, this visualizes actual vs predicted salary for the unseen test data.

**Running the Script:**

1. Save the code as a Python file (e.g., `salary_predictor.py`).
2. Open a terminal or command prompt and navigate to the directory where you saved the file.
3. Run the script using `python salary_predictor.py`.

This README provides a basic structure. You can customize it further by adding:

* Links to relevant resources or tutorials.
* Information about the chosen machine learning algorithm.

