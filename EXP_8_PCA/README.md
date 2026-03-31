# Experiment 8: Effect of PCA on Regression and Classification Models

## Name PREM SHANKAR.S

## RegNo 3122235001101

## 📌 Objective
To study the impact of Principal Component Analysis (PCA) on the performance of regression and classification models.

---

## 📂 Dataset
- Dataset: **PCA Full Lab Dataset (1000 Samples)**
- Features: Academic scores, attendance, and performance-related attributes
- Targets:
  - Regression: `Final_Score_Regression`
  - Classification: `Performance_Level_Classification`

---

## 🔹 Step 1: Data Loading & Exploration
The dataset was loaded using Pandas, and basic information such as number of samples, features, and distributions of target variables were analyzed.

---

## 🔹 Step 2: Preprocessing
No missing values were found; the classification target was label encoded, and all features were standardized using StandardScaler.

---

## 🔹 Step 3: PCA Implementation
PCA was applied after standardization, retaining 95% of variance, reducing features from 11 to 7 while preserving most information.

---

## 🔹 Step 4: Regression Models
Linear Regression and Random Forest Regressor were trained using 5-fold cross-validation on both original and PCA-transformed data.

---

## 🔹 Step 5: Classification Models
Logistic Regression and SVM were evaluated using 5-fold cross-validation, comparing performance with and without PCA.

---

## 📊 Evaluation Metrics
- Regression:
  - Mean Squared Error (MSE)
  - R² Score
- Classification:
  - Accuracy
  - F1-score (macro)

---

## 📉 Visualization
Scree plots and comparison graphs were generated to analyze explained variance and model performance differences.

---

## 🔍 Key Observations
- PCA slightly improved Linear Regression and Logistic Regression performance.
- Random Forest showed minimal change due to its robustness to feature redundancy.
- SVM performance decreased slightly after PCA, likely due to loss of nonlinear relationships.

---

## ✅ Conclusion
PCA is useful for reducing dimensionality and improving linear model performance, but may not benefit tree-based models and can sometimes negatively affect nonlinear models like SVM.

---