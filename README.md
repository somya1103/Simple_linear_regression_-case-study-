# Simple_linear_regression_-case-study-
Simple Linear Regression & Transformations on Breast Cancer Dataset

 1. Project Structure
    -

Show main files and folders:

```
├── data/                # Dataset (if allowed) or link
├── notebooks/           # Jupyter notebooks                
├── documentation/       # insights Plots & figures               
├── README.md            # Project documentation
```


2 Workflow / Steps
-

Document main steps:

1. Basic Inspection
2. Univariate & Bivariate Analysis
3. Train-Test Split
4. Model Fitting
5. Diagnostics (Residuals, QQ Plot, BP Test)
6. Fixing Violations (Box-Cox, Yeo-Johnson, etc.)
7. Influential Points
8. Metrics Evaluation
9. Cross-Validation
10. Visualizations (Actual vs Predicted, Residuals)
11. Retraining & Saving Model

 3. Results
    -

* Show evaluation metrics (MSE, RMSE, R², MAPE).
 (Actual vs Predicted scatter, Residual histogram).


4 Insights 
-
Data Quality: The dataset was clean — no missing or duplicate values, making it well-suited for direct modeling.

Feature Behavior: radius_mean and perimeter_mean showed strong correlation with the target, validating their predictive power.

Model Diagnostics: Initial regression revealed heteroscedasticity (BP test p-value ≈ 3.7e-09), meaning variance was not constant across residuals.

Transformations: Applying Box-Cox transformation successfully stabilized variance, improved residual distribution, and gave the best diagnostics compared to log, sqrt, and Yeo-Johnson.

Model Performance: Final regression achieved R² = 0.9061 and MAPE ≈ 4.42%, indicating highly accurate predictions with errors well within acceptable bounds.

5. Learnings
   -
Importance of Assumption Checks: Regression is not just about fitting — validating assumptions (normality, homoscedasticity, influential points) is crucial.

Transformations Matter: Correct transformation (Box-Cox here) can drastically improve model validity and interpretability.

Handling Influential Points: Identifying outliers, leverage, and Cook’s distance teaches how certain points can disproportionately influence model outcomes.

Model Validation: Using cross-validation gives confidence in generalizability, and documenting metrics/visuals makes the project professional for GitHub and interviews.

6. Acknowledgments / References
   -

* Kaggle dataset source (e.g., Breast Cancer dataset).

