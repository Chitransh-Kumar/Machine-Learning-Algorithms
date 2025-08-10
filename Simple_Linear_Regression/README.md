# Simple Linear Regression

This project demonstrates the implementation of **Simple Linear Regression** from scratch and using scikit-learn to predict students' final marks based on the number of hours they studied/attended.

## 📌 Project Overview
The goal is to model the relationship between **hours studied** (independent variable) and **final marks obtained** (dependent variable), visualize this relationship, train a regression model, and evaluate its performance.

## 📂 Files
- `Simple Linear Regression.ipynb` — Main Jupyter notebook containing the entire workflow.
- `Study_vs_Score_data.csv` — Dataset containing `Attendance_Hours` and `Final_Marks`.

## 🛠️ Requirements
Make sure you have the following Python libraries installed:
```bash
pip install numpy pandas matplotlib scikit-learn
```

## 🚀 Steps in the Notebook
1. **Importing Libraries**  
   - `numpy`, `pandas` for data handling.  
   - `matplotlib` for visualization.  
   - `scikit-learn` for model implementation.

2. **Loading Dataset**  
   Reads `Study_vs_Score_data.csv` into a Pandas DataFrame.

3. **Data Exploration**  
   - Checking shape, info, and basic statistics.  
   - Visualizing data using scatter plots.

4. **Data Preparation**  
   - Splitting dataset into training and testing sets.  
   - Separating features (`X`) and labels (`y`).

5. **Model Training**  
   - Using **LinearRegression** from `sklearn.linear_model`.  
   - Fitting the model to the training data.

6. **Prediction**  
   - Making predictions on test data.  
   - Visualizing the regression line over the scatter plot.

7. **Evaluation**  
   - Calculating metrics: **Root Mean Squared Error (MSE)** and **R² Score**.

## 📊 Example Visualization
The model fits a straight line to best represent the relationship between hours studied and marks scored.

## 📈 Results
- A strong positive correlation between study hours and marks obtained.
- R² Score close to **1**, indicating a good fit.


