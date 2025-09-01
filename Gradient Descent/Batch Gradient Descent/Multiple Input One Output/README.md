# 📘 Batch Gradient Descent (Multiple Linear Regression)

This project demonstrates the implementation of **Multiple Linear
Regression using Batch Gradient Descent** from scratch with NumPy, and
compares it with **scikit-learn's LinearRegression**. The focus is to
understand how gradient descent optimizes parameters when multiple
features are involved, and how results compare with scikit-learn.

------------------------------------------------------------------------

## 📌 Project Overview

The objective is to model the relationship between multiple independent
variables (such as **engine size, cylinders, fuel consumption, etc.**)
and the dependent variable (**CO2 Emissions**) using **Batch Gradient
Descent optimization**.

Both the custom gradient descent implementation and **scikit-learn's
LinearRegression** are trained and evaluated to compare performance.

------------------------------------------------------------------------

## 📂 Files

-   `Batch Gradient Descent 2.ipynb` --- Main Jupyter notebook
    containing the full workflow.
-   `co2.csv` --- Dataset with columns including:
    -   Vehicle characteristics (`Engine Size`, `Cylinders`,
        `Fuel Consumption City`, etc.)
    -   `CO2 Emissions (g/km)` (target variable).

------------------------------------------------------------------------

## 🛠️ Requirements

Make sure you have the following Python libraries installed:

``` bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

------------------------------------------------------------------------

## 🚀 Steps in the Notebook

1.  **Importing Libraries**
    -   `numpy`, `pandas` for numerical and data handling.
    -   `matplotlib`, `seaborn` for visualization.
    -   `scikit-learn` for model comparison and preprocessing.
2.  **Loading Dataset**
    -   Reads `co2.csv` into a Pandas DataFrame.
3.  **Data Preprocessing**
    -   Dropping irrelevant columns (`Make`, `Model`).
    -   Encoding categorical variables (`Vehicle Class`, `Transmission`,
        `Fuel Type`, `Cylinders`) using **One-Hot Encoding**.
    -   Scaling numerical features using **StandardScaler**.
    -   Train-test split (80--20).
4.  **Model Training**
    -   **From Scratch**: Implemented **Batch Gradient Descent** with
        iterative updates to weights and bias.
    -   **Scikit-learn**: Used `LinearRegression` pipeline with
        preprocessing steps.
5.  **Prediction**
    -   Generating predictions on test data.
    -   Comparing actual vs predicted CO2 emissions.
6.  **Evaluation**
    -   Metric: **R² Score**.
    -   Performance comparison between scratch and scikit-learn models.

------------------------------------------------------------------------

## 📊 Example Visualizations

-   Scatter plots of numerical features vs `CO2 Emissions`.
-   Barplot of categorical features vs `CO2 Emissions`.

------------------------------------------------------------------------

## 📈 Results

-   Batch Gradient Descent converges successfully to optimal parameters
    when features are **standardized**.
-   The scratch implementation produces results **close to
    scikit-learn's model**, though slight differences may exist due to
    learning rate, convergence criteria, and numerical precision.
-   R² score comparison shows both approaches perform similarly.

------------------------------------------------------------------------

## 🔍 Comparison: Scratch vs Scikit-learn

  Metric     Scratch Implementation   Sklearn Implementation
  ---------- ------------------------ ------------------------
  R² Score   Slightly lower           Higher (benchmark)

✅ Both implementations validate that **Batch Gradient Descent can be
applied successfully for multiple linear regression**.
