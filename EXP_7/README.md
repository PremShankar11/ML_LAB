# Ensemble Learning Experiment: Bagging, Boosting, and Stacking

## Name: PREM SHANKAR.S

## RegNo: 3122235001101

## 📌 Objective
To implement and compare Bagging, Boosting, and Stacked Ensemble models on a classification dataset and analyze their performance.

---

## 🔹 Step 1: Data Loading & Preprocessing
Loaded the dataset from a CSV file, assigned proper column names, converted target labels (M/B → 0/1), and separated features and target.

---

## 🔹 Step 2: Exploratory Data Analysis (EDA)
Analyzed class distribution, visualized feature distributions, and examined correlations between features and target.

---

## 🔹 Step 3: Train-Test Split & Scaling
Split the dataset into 80–20 training and testing sets using stratification and applied feature scaling using StandardScaler.

---

## 🔹 Step 4: Bagging Implementation
Implemented a Bagging Classifier using Decision Trees and evaluated performance with cross-validation using accuracy and F1-score.

---

## 🔹 Step 5: Boosting Implementation
Applied AdaBoost and tuned hyperparameters, and evaluated using cross-validation metrics.

---

## 🔹 Step 6: Stacked Ensemble Model
Built a stacking model using SVM, Naive Bayes, and Decision Tree as base learners with Logistic Regression as meta-learner.

---

## 🔹 Step 7: Model Evaluation
Compared all models using accuracy, precision, recall, F1-score, confusion matrix, and ROC-AUC curve.

---

## 🔹 Step 8: Performance Comparison
Compiled results into comparison tables to analyze which ensemble method performed best.

---

## 🔹 Conclusion
Ensemble methods improved predictive performance, with Boosting and Stacking showing superior results compared to Bagging.

---

## 📚 References
- Scikit-learn Documentation  
- UCI Machine Learning Repository  
implement