# Machine Learning Lab – Experiment 2  
## Binary Classification using Naïve Bayes & KNN

This experiment implements **Naïve Bayes** and **K-Nearest Neighbors (KNN)** for a binary classification problem and compares their performance using multiple evaluation metrics.

## Dataset
- **Spambase Dataset** (Kaggle)
- Numerical features related to word and character frequencies
- Target label: `class` (Spam / Not Spam)

---

## Libraries Used
- NumPy, Pandas – data handling  
- Matplotlib, Seaborn – visualization  
- Scikit-learn – ML models, preprocessing, metrics  

---

## 1. Data Loading & Exploration
- Loaded dataset using Pandas
- Checked shape, column types, and basic statistics
- Verified no missing values
- Analyzed class distribution
- Visualized feature distributions using histograms

---

## 2. Data Preparation
- Split data into **features (X)** and **target (y)**
- Performed **stratified train-test split**
- Applied **Standard Scaling** for distance-based models

---

## 3. Naïve Bayes Models
Implemented and evaluated:
- **Gaussian Naïve Bayes**
- **Multinomial Naïve Bayes**
- **Bernoulli Naïve Bayes**

**Steps Done:**
- Model training
- Prediction on test data
- Measured:
  - Accuracy
  - Precision
  - Recall
  - F1-score
  - Confusion Matrix
  - Specificity & False Positive Rate
- Compared training and prediction time
- Generated ROC curves for comparison

---

## 4. K-Nearest Neighbors (KNN)
**Basic Model:**
- Trained baseline KNN using scaled data

**Hyperparameter Tuning:**
- Tested multiple `k` values
- Plotted Accuracy vs k
- Used:
  - Stratified K-Fold Cross Validation
  - Grid Search
  - Randomized Search

**Final Model:**
- Selected best `k`, distance metric, and weight type
- Evaluated using same metrics as Naïve Bayes
- Plotted confusion matrix and ROC curve

---

## 5. KDTree & BallTree Optimization
- Implemented KNN using:
  - KDTree
  - BallTree
- Compared accuracy, time, and memory usage
- Observed similar performance with improved efficiency

---

## 6. Model Comparison & Statistical Test
- Performed **cross-validation**
- Compared models using **precision scores**
- Applied **One-way ANOVA test**
- Identified statistically significant performance differences

---

## 7. Results Summary
- Bernoulli NB performed better among Naïve Bayes models
- Optimized KNN achieved highest overall performance
- KDTree KNN selected as the **best model**

---

## Conclusion
Naïve Bayes models are fast and simple but show higher bias.  
KNN, when properly tuned, provides better accuracy and generalization, with tree-based methods improving efficiency.

---

## References
- Scikit-learn Documentation  
- Spambase Dataset (Kaggle)  
