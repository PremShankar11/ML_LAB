# Experiment: Handwritten Character Classification using Perceptron and Multi-Layer Perceptron (MLP)

## Author
**Name:** PREM SHANKAR.S

**RegNo:** 3122235001101

---

## Objective
To classify handwritten alphanumeric characters (0-9, A-Z, a-z) by implementing a custom Multiclass Perceptron Learning Algorithm (PLA) and a Multi-Layer Perceptron (MLP) classifier. The experiment also aims to analyze the impact of feature scaling, hyperparameter tuning, and network architecture on model performance and training convergence. 

---

## Dataset
The dataset (`english.csv`) consists of 3,410 images of English characters and digits spanning 62 unique classes. The original images are in RGB format with a resolution of 1200x900 pixels.

---

## Operations Performed

1. **Dataset Loading** Imported the image paths and labels from `english.csv` using Pandas and verified the total sample size (3,410 samples).

2. **Exploratory Data Analysis (EDA)** Inspected image properties (size and mode) using the PIL library and visualized a sample image with its corresponding label using Matplotlib.

3. **Data Preprocessing & Image Transformation** Iterated through the image dataset to convert all images to grayscale, resized them to 28x28 pixels, normalized pixel values by dividing by 255.0, and flattened them into 1D arrays of 784 features.

4. **Train-Validation-Test Split** Split the preprocessed dataset into training (70%), validation (15%), and testing (15%) sets using stratified sampling to maintain class distributions.

5. **Custom Perceptron Implementation** Developed a custom binary `Perceptron` class and extended it to a `MulticlassPerceptron` using a One-vs-Rest strategy to handle the 62 target classes.

6. **Baseline PLA Training & Evaluation** Trained the custom Multiclass Perceptron on the training set and evaluated it on the validation set, yielding an initial validation accuracy of approximately 6.4%.

7.**One-Hot Encoding & Baseline MLP Training** Encoded target variables using `OneHotEncoder` and trained a baseline `MLPClassifier` without feature scaling, resulting in a low validation accuracy of ~1.5%.

8. **Feature Scaling** Applied `StandardScaler` to standardize the features, which significantly improved the MLP's ability to learn and converge.

9. **Hyperparameter Tuning – MLP Network Architecture** Experimented with different hidden layer configurations (e.g., single layer of 128, two layers of 256 and 128, and three layers of 512, 256, and 128 nodes) to observe the effect of depth on accuracy.

10. **Hyperparameter Tuning – Learning Rate & Optimizers** Tuned learning rates (0.01, 0.001, 0.0005) and optimizers (SGD vs. Adam), identifying that an Adam optimizer with a learning rate of 0.001 and two hidden layers (256, 128) provided the optimal performance.

11. **Final Model Evaluation** Evaluated the optimized MLP model on the test set, generating accuracy metrics (~46.5%), a classification report (precision, recall, f1-score), and a Confusion Matrix.

12.**Convergence and Performance Comparison** Plotted and analyzed the training loss convergence curves between the custom PLA and the best MLP model, and explicitly compared their final macro-averaged precision, recall, and F1-scores.

---

## Conclusion
The Multi-Layer Perceptron (MLP) heavily outperformed the custom Multilayer Perceptron (PLA) for the complex task of classifying 62 different handwritten characters. While the custom PLA struggled to capture non-linear patterns (achieving an accuracy of ~8.6% on the test set), the tuned MLP achieved a test accuracy of ~46.5%. Feature scaling using `StandardScaler` proved to be a critical step, as the MLP completely failed to converge on unscaled data. 

Furthermore, tuning the hidden layer architecture and learning rate effectively optimized the model's ability to generalize unseen images. 

---

## References
- Scikit-learn Neural Network (MLPClassifier) Documentation
- Scikit-learn Preprocessing (StandardScaler, OneHotEncoder) Documentation
- PIL (Pillow) Documentation for Image Processing
- Pandas & NumPy Documentation
- Matplotlib Pyplot Documentation