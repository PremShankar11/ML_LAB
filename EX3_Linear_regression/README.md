# Experiment 3: Regression Analysis using Linear and Regularized Models

## Author
**Name:** PREM SHANKAR.S 

---

## Objective
To implement linear and regularized regression models for predicting loan amount and analyze their performance, overfitting, and bias–variance behavior.

---

## Dataset
A real-world loan application dataset containing numerical and categorical features, with loan amount as the target variable.

---

## Operations Performed

1. **Dataset Loading**  
   Imported the loan dataset and inspected its structure and target variable.

2. **Missing Value Handling**  
   Handled missing values to ensure reliable model training.

3. **Categorical Feature Encoding**  
   Converted categorical variables into numerical form using encoding techniques.

4. **Feature Scaling**  
   Standardized numerical features to make regularization effective.

5. **Exploratory Data Analysis (EDA)**  
   Analyzed feature distributions and target variable behavior using plots.

6. **Train–Test Split**  
   Split the dataset into training and testing sets to evaluate generalization.

7. **Linear Regression Model**  
   Trained a baseline linear regression model for comparison.

8. **Ridge Regression Model**  
   Applied L2 regularization to reduce coefficient magnitudes and control variance.

9. **Lasso Regression Model**  
   Applied L1 regularization to encourage feature sparsity.

10. **Elastic Net Regression Model**  
    Combined L1 and L2 regularization to balance bias and variance.

11. **Hyperparameter Tuning**  
    Used 5-fold cross-validation with Grid/Random Search to find optimal parameters.

12. **Model Evaluation**  
    Evaluated all models using MAE, MSE, RMSE, R² score, and training time.

13. **Performance Comparison**  
    Compared cross-validation and test set performance across models.

14. **Coefficient Analysis**  
    Compared coefficients to study the effect of regularization.

15. **Overfitting and Underfitting Analysis**  
    Analyzed training and validation errors to assess model generalization.

16. **Bias–Variance Analysis**  
    Studied bias behavior of Linear Regression and variance reduction in regularized models.

---

## Conclusion
All regression models showed similar predictive performance, indicating good generalization. Regularization mainly improved coefficient stability rather than prediction accuracy, making Linear Regression an effective baseline for this dataset.

---

## References
- Scikit-learn Linear Models Documentation  
- Scikit-learn Hyperparameter Optimization  
- Kaggle: Predict Loan Amount Dataset
