# Batch Gradient Descent (Linear Regression)  

This project demonstrates the implementation of **Linear Regression using Batch Gradient Descent** from scratch with NumPy, and compares it with **scikit-learn’s LinearRegression**. The goal is to understand how gradient descent works to minimize error and fit the best line for prediction.  

## 📌 Project Overview  
The objective is to model the relationship between an independent variable (`cgpa`) and the dependent variable (`package`) using **Batch Gradient Descent optimization**. Both the custom gradient descent implementation and **scikit-learn’s LinearRegression** are trained and evaluated.  

## 📂 Files  
- `Batch Gradient Descent.ipynb` — Main Jupyter notebook containing the entire workflow.  
- `placement.csv` — Dataset containing:  
  - `cgpa` (feature)  
  - `package` (target variable)  

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
   - Reads `placement.csv` into a Pandas DataFrame.  

3. **Data Exploration**  
   - Checking dataset shape, info, and statistics.  
   - Scatter plot to see the relationship between `cgpa` and `package`.  

4. **Data Preprocessing**  
   - Splitting into features (`X`) and target (`y`).  
   - Train-test split (80–20).  

5. **Model Training**  
   - **From Scratch**: Implemented **Batch Gradient Descent** with iterative updates to slope and intercept.  
   - **Scikit-learn**: Using `LinearRegression` for direct comparison.  

6. **Prediction**  
   - Generating predictions on test data.  
   - Visualizing regression line with actual data.  

7. **Evaluation**  
   - Metric: **R² Score**.  
   - Comparing performance between scratch and scikit-learn models.  

## 📊 Example Visualization  
- Scatter plot of actual vs predicted values.  

## 📈 Results  
- Batch Gradient Descent converges successfully to optimal parameters when the input is standardized.  
- Scratch implementation and scikit-learn implementation produce **similar predictions and R² scores**, confirming correctness.  
- Training loss decreases smoothly over iterations.  

## 🔍 Comparison: Scratch vs Scikit-learn  

| Metric      | Scratch Implementation | Sklearn Implementation |
|-------------|------------------------|-------------------------|
| R² Score    | ~Identical             | ~Identical             |  

✅ Both implementations yield **equivalent results**, proving the correctness of the scratch gradient descent model.  
