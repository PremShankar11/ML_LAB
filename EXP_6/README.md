# Experiment: Breast Cancer Classification using Decision Tree and Random Forest

## Author
**Name:** PREM SHANKAR.S

**RegNo:** 3122235001101

---

## Objective
To classify breast cancer tumors as malignant or benign using Decision Tree and Random Forest classifiers. The experiment also aims to analyze the impact of hyperparameter tuning, model ensembling, and feature importance on classification performance and generalization.

---

## Dataset
The Breast Cancer Wisconsin (Diagnostic) Dataset containing 569 samples. It includes 30 numerical features computed from a digitized image of a fine needle aspirate (FNA) of a breast mass, describing characteristics like radius, texture, perimeter, and area. The target variable is a binary class label indicating the diagnosis (M = malignant, B = benign).

---

## Operations Performed

1. **Dataset Loading & Preprocessing** Imported the `wdbc.data` dataset, assigned appropriate column names for the 30 features, and dropped the irrelevant 'id' column. The target variable 'diagnosis' was mapped from categorical labels ('M', 'B') to binary numerical values (1 for Malignant, 0 for Benign).

2. **Exploratory Data Analysis (EDA)** Inspected the dataset's shape and visualized the class distribution of the target variable using a count plot, identifying the dataset as slightly imbalanced (357 Benign vs 212 Malignant).

3. **Feature Correlation Analysis** Generated a feature correlation heatmap using Seaborn to identify highly correlated features. Strong correlations were observed among geometric measurements (e.g., radius, perimeter, area), indicating that some features contain redundant information.

4. **Train-Test Split** Split the dataset into training (80%) and testing (20%) sets to ensure proper model evaluation on unseen data.

5. **Baseline Decision Tree Model** Trained an initial baseline Decision Tree classifier and evaluated its performance on the test set, generating metrics such as accuracy (~94.7%), precision, recall, F1-score, and a Confusion Matrix.

6. **Hyperparameter Tuning – Decision Tree** Performed an extensive grid search with 5-fold cross-validation, tuning hyperparameters such as `criterion` (gini vs. entropy), `max_depth`, `min_samples_split`, and `min_samples_leaf`. Plotted the relationship between tree depth and cross-validation accuracy to identify the optimal complexity and prevent overfitting.

7. **Baseline Random Forest Model** Trained a baseline Random Forest classifier to establish ensemble performance. The baseline model immediately showed an improvement over the Decision Tree, achieving an initial accuracy of ~96.5%.

8. **Hyperparameter Tuning – Random Forest** Conducted cross-validation grid search to optimize the Random Forest model by tuning `n_estimators`, `max_depth`, and `max_features` to maximize both accuracy and F1-score.

9. **Cross-Validation Analysis** Evaluated the stability and generalization performance of both models by observing the accuracy across individual folds during 5-fold cross-validation.

10. **Model Comparison & ROC Analysis** Compared the final tuned Decision Tree and Random Forest models using bar charts representing 5-Fold CV Accuracy. Plotted Receiver Operating Characteristic (ROC) curves and calculated the Area Under the Curve (AUC) to compare the probability prediction power of both classifiers.

11. **Feature Importance Analysis** Extracted and visualized feature importances from the optimized Random Forest model to determine which geometric tumor properties contributed the most to the model's decision-making process.

---

## Conclusion
Both classifiers proved effective at diagnosing breast cancer; however, the Random Forest model outperformed the standalone Decision Tree in overall accuracy, F1-score, and AUC. While hyperparameter tuning successfully controlled the Decision Tree's tendency to overfit, the Random Forest classifier demonstrated superior robustness and generalization by naturally handling feature correlations and variance through its ensemble approach. Additionally, feature importance analysis successfully highlighted the most critical geometric tumor measurements driving the malignant classifications.

---

## References
- Scikit-learn Decision Tree Documentation
- Scikit-learn Random Forest Documentation
- Scikit-learn Model Evaluation (ROC, AUC, Confusion Matrix, Cross-validation)
- Seaborn & Matplotlib Documentation for Data Visualization
- UCI Machine Learning Repository – Breast Cancer Wisconsin (Diagnostic) Dataset