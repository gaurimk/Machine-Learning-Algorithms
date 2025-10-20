Cross Validation Techniques
📘 Overview

Cross Validation is a statistical method used to evaluate and improve the performance of machine learning models. It ensures that the model generalizes well to unseen data by testing it on multiple subsets of the dataset.

🧠 Steps and Techniques Used

Dataset Used:

Breast Cancer dataset from Scikit-Learn.

Dropped unnecessary columns (id, Unnamed: 32).

Defined independent variables (X) and the dependent variable (y).

Model Used:

Implemented using Decision Tree Classifier from sklearn.tree.

Techniques Implemented:

🔹 a) Leave-One-Out Cross Validation (LOOCV)

Trains the model on all data except one observation.

Tests on the single left-out sample.

Repeats for all data points.

Advantage: Almost unbiased performance estimate.

Disadvantage: Very slow for large datasets.

🔹 b) Hold-Out Validation

Splits the data into training and testing sets (commonly 70–30 or 80–20).

Simple and fast approach.

Limitation: Model performance may vary depending on how data is split.

🔹 c) K-Fold Cross Validation

Divides data into k equal parts (folds).

Model trains on k−1 folds and tests on the remaining one.

Repeats k times and averages the scores.

Advantage: Reduces variance due to random sampling.

🔹 d) Stratified K-Fold Cross Validation

Similar to K-Fold but maintains class distribution in each fold.

Best for classification problems with imbalanced classes.

Ensures that each fold represents the overall dataset properly.

🔹 e) Repeated Random Test-Train Split (ShuffleSplit)

Randomly splits data multiple times into train and test sets.

Calculates and averages accuracy scores.

Benefit: Reduces the randomness effect and provides reliable results.

Evaluation Metric:

Used cross_val_score() from Scikit-Learn to compute average model accuracy across folds.

Observations:

Performance varies slightly across different cross-validation methods.

K-Fold and Stratified K-Fold provided more stable accuracy scores.

LOOCV gave the most precise but computationally expensive results.

Conclusion:

Cross-validation ensures better generalization and reduces overfitting.

It provides a more reliable performance estimate than a single train-test split.

Among all, Stratified K-Fold is generally the best choice for classification problems.
