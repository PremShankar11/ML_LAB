
# Machine Learning Lab – Experiment 1 (EDA & Feature Analysis)

This lab focuses on understanding datasets using Exploratory Data Analysis (EDA) and applying basic feature selection techniques using Python ML libraries.

## Libraries Used

* NumPy – numerical operations

* Pandas – data loading & manipulation

* Matplotlib & Seaborn – data visualization

* Scikit-Learn – preprocessing & feature selection

## 1. Iris Dataset

* Loaded Iris dataset and removed unnecessary ID column

* Checked data info, shape, and summary statistics

* Visualized data using:

    Histograms

    Box plots (outlier check)

    Bar chart for class distribution

    Correlation heatmap

* Observed minimal outliers and clear feature relationships

## 2. Loan Amount Prediction Dataset

* Loaded loan dataset and inspected structure

* Checked shape, column types, and descriptive statistics

* Identified outliers (age, income, loan amount, etc.)

* Verified no missing values

* Converted categorical values to numeric (Yes/No → 1/0)

* Separated numerical and categorical features

* Visualized:

    Histograms

    Box plots (before & after outlier handling)

    Bar plots for categorical features

    Correlation heatmap

* Applied IQR-based capping (winsorization) for outliers

* Used ANOVA (SelectKBest) for feature selection

* Split data into Train / Validation / Test sets

* Verified class distribution (no imbalance)

## 3. Diabetes Prediction Dataset

* Loaded diabetes dataset

* Reviewed column details and statistics

* Plotted:

    Histograms for numerical features

    Box plots for outlier detection

    Count plots for categorical variables

* Observed heavy class imbalance

* Analyzed correlations using heatmap

## 4. Email Spam Classification

* Loaded spam/ham email dataset

* Checked dataset structure and label distribution

* Cleaned text:

    Lowercasing

    Removing URLs & special characters

    Added word count and character count features

* Analyzed most common words (spam vs ham)

* Converted text to numerical features using TF-IDF

* Applied Chi-Square feature selection

* Identified top spam-related words