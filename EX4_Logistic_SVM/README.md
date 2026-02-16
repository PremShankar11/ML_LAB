# Experiment 4: Spam Email Classification using Logistic Regression and SVM

## Author
**Name:** PREM SHANKAR.S   

---

## Objective
To classify emails as spam or ham using Logistic Regression and Support Vector Machine (SVM) classifiers and analyze the impact of hyperparameter tuning, kernel selection, and bias–variance behavior on classification performance.

---

## Dataset
The Spambase dataset containing numerical features extracted from email content, including word frequencies, character frequencies, and capitalization patterns, with a binary class label indicating spam or non-spam.

---

## Operations Performed

1. **Dataset Loading**  
   Imported the loan dataset and inspected its structure and target variable.

2. **Data Type Verification**  
   Verified that all features were numerical and suitable for Logistic Regression and SVM.

3. **Missing Value Analysis**  
   Checked for missing values and confirmed that the dataset contained no null entries.

4. **Feature Scaling**  
   Standardized numerical features to make regularization effective.

5. **Exploratory Data Analysis (EDA)**  
   Analyzed feature distributions and target variable behavior using plots.

6. **Train–Test Split**  
   Split the dataset into training and testing sets to evaluate generalization.

7. **Baseline Logistic Regression Model**  
   Trained a baseline Logistic Regression model to establish reference performance.

8. **Hyperparameter Tuning – Logistic Regression**  
   Applied Grid Search with 5-fold cross-validation to tune regularization type, solver, and regularization strength, with the best performance achieved at C = 10.

9. **SVM Kernel-wise Training**  
   Trained Support Vector Machine models using linear, polynomial, RBF, and sigmoid kernels to compare kernel behavior.

10. **Hyperparameter Tuning – SVM**
Performed Grid Search with 5-fold cross-validation to tune kernel parameters and regularization strength, identifying RBF kernel with C = 10 as optimal.

11. **Cross-Validation Analysis**
Used 5-fold cross-validation to evaluate model stability and generalization performance.

12. **Model Evaluation**
Evaluated final models using accuracy, precision, recall, F1-score, and training time.

13. **Performance Comparison**
Compared Logistic Regression and SVM models to identify the best-performing classifier.

14. **Kernel Behavior Analysis**
Analyzed the effect of different SVM kernels on classification accuracy and generalization.

15. **Bias–Variance Trade-Off Analysis**
   Studied how regularization and kernel choice affected model bias, variance, and overfitting.
   
---

## Conclusion
Both Logistic Regression and SVM performed effectively on the Spambase dataset; however, the Support Vector Machine with RBF kernel and regularization strength C = 10 achieved the best overall performance. Regularization played a key role in controlling model complexity for both classifiers, and the tuned SVM demonstrated a superior bias–variance trade-off with strong generalization on unseen data.

---

## References
- Scikit-learn Logistic Regression Documentation
- Scikit-learn Support Vector Machines Documentation
- Scikit-learn Hyperparameter Optimization
- Kaggle: Spambase Dataset
- UCI Machine Learning Repository – Spambase
