# 🌿 Ensemble Learning (Voting, Bagging, Boosting, Stacking)

## 📘 Overview
This project explains and compares four popular **Ensemble Learning techniques** — **Voting, Bagging, Boosting, and Stacking** — using the **Iris dataset**.  
Ensemble Learning means combining multiple models to get better and more accurate results than a single model alone.

---

## 🎯 Objective
To understand how different ensemble methods work and how they improve model performance.

---

## 📂 Dataset
- **Dataset Name:** Iris Dataset  
- **Source:** `sklearn.datasets`  
- **Features:**
  - Sepal Length  
  - Sepal Width  
  - Petal Length  
  - Petal Width  
- **Target:** Species (Setosa, Versicolor, Virginica)

---

## 🧩 Ensemble Techniques

### 🟦 1. Voting Classifier
- Combines predictions from **different models** (like Logistic Regression, Decision Tree, KNN, etc.).  
- Each model gives its own prediction, and the **majority vote** decides the final result.  
- Two types:
  - **Hard Voting:** Majority class wins.  
  - **Soft Voting:** Average of prediction probabilities.

✅ **Goal:** Combine the strengths of multiple models.  
✅ **Example:** Logistic Regression + SVM + KNN.

---

### 🟩 2. Bagging (Bootstrap Aggregating)
- Uses **the same model** multiple times on **different random subsets** of the data.  
- The results of all models are then combined (averaged or voted).  
- Helps to make the model more stable and less overfitted.

✅ **Goal:** Reduce overfitting and model variance.  
✅ **Example:** Random Forest (Bagging of Decision Trees).

---

### 🟧 3. Boosting
- Builds models **one after another**, where each new model **tries to correct the mistakes** made by the previous one.  
- It gives more importance to the data points that were misclassified earlier.  
- Examples: **AdaBoost**, **Gradient Boosting**, **XGBoost**.

✅ **Goal:** Reduce model bias and improve accuracy.  
✅ **Idea:** Focus on difficult examples step by step.

---

### 🟪 4. Stacking
- Combines **different models** and uses another model (called a **meta-model**) to learn the best way to combine their predictions.  
- The meta-model takes predictions from base models as input.

✅ **Goal:** Learn how to best blend multiple models for maximum performance.  
✅ **Example:** Base models → Decision Tree, KNN, SVM; Meta-model → Logistic Regression.
