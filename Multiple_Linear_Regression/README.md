
# Multiple Linear Regression  

This project demonstrates the implementation of **Multiple Linear Regression** from scratch and using **scikit-learn** to predict employees’ salaries based on multiple experience and certification factors.  

## 📌 Project Overview  
The goal is to model the relationship between several independent variables (experience and certifications) and the dependent variable (salary). Both the mathematical **Normal Equation approach (scratch)** and **scikit-learn’s LinearRegression** are implemented and compared.  

## 📂 Files  
- `Multiple Linear Regression.ipynb` — Main Jupyter notebook containing the entire workflow.  
- `SalaryMulti.csv` — Dataset containing:  
  - `Total Experience`  
  - `Team Lead Experience`  
  - `Project Manager Experience`  
  - `Certifications`  
  - `Salary` (target variable)  

## 🛠️ Requirements  
Make sure you have the following Python libraries installed:  
```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```  

## 🚀 Steps in the Notebook  
1. **Importing Libraries**  
   - `numpy`, `pandas` for data handling.  
   - `matplotlib`, `seaborn` for visualization.  
   - `scikit-learn` for model implementation and preprocessing.  

2. **Loading Dataset**  
   Reads `SalaryMulti.csv` into a Pandas DataFrame.  

3. **Data Exploration**  
   - Checking shape, info, and statistics.  
   - Correlation analysis between features and salary.  
   - Visualizing relationships using scatter/box plots.  

4. **Data Preprocessing**  
   - Feature-target split (`X`, `y`).  
   - Train-test split (80–20).  
   - Feature standardization using `StandardScaler`.  

5. **Model Training**  
   - **From Scratch**: Implemented using the **Normal Equation**.  
   - **Scikit-learn**: Using `LinearRegression` wrapped in a `Pipeline` with `StandardScaler`.  

6. **Prediction**  
   - Generating predictions on test data.  
   - Comparing model predictions with actual salaries.  

7. **Evaluation**  
   - Metrics: **R² Score**.  
   - Coefficients and intercept interpretation.  

## 📊 Example Visualization  
Scatter/regression plots showing the relationship between experience, certifications, and salary.  

## 📈 Results  
- Strong positive correlation between experience-related features and salary.  
- Custom implementation and scikit-learn implementation yield **identical coefficients and intercepts**, confirming correctness.  
- R² Score indicates the model fits the data well.  

## 🔍 Comparison: Scratch vs Scikit-learn  

| Feature                       | Scratch Coefficients | Sklearn Coefficients |
|-------------------------------|----------------------|-----------------------|
| Total Experience              | Identical            | Identical             |
| Team Lead Experience          | Identical            | Identical             |
| Project Manager Experience    | Identical            | Identical             |
| Certifications                | Identical            | Identical             |
| **Intercept**                 | Identical            | Identical             |  

✅ Both implementations produce the **same parameters and predictions**, validating the scratch solution.  
