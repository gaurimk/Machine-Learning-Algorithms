# 🧩 Scikit-Learn Pipelines — Titanic Dataset

This project demonstrates the use of **Scikit-Learn Pipelines** to streamline a complete Machine Learning workflow — from data preprocessing to model training and evaluation — using the classic **Titanic dataset**.

---

## 🧠 Overview
In traditional ML workflows, preprocessing and model training steps are often performed separately.  
**Pipelines** in `scikit-learn` allow these steps to be combined into a single object, ensuring clean, consistent, and reproducible code.

This project automates:
- Data cleaning and preprocessing  
- Feature encoding and imputation  
- Model training and evaluation  

---

## 📂 Folder Contents
| File Name | Description |
|------------|-------------|
| `titanic-using-pipeline.ipynb` | Jupyter Notebook implementing ML pipelines using scikit-learn |
| `README.md` | Description and documentation of the pipeline project |

---

## ⚙️ Implementation Steps
1. **Data Loading**  
   Load the Titanic dataset and explore its structure.

2. **Preprocessing Pipeline**  
   - Handle missing values using `SimpleImputer`  
   - Encode categorical variables using `OneHotEncoder`  
   - Combine transformations using `ColumnTransformer`

3. **Modeling Pipeline**  
   - Integrate preprocessing and modeling in one pipeline  
   - Use classifiers like `DecisionTreeClassifier`, `RandomForestClassifier`, or `LogisticRegression`

4. **Model Evaluation**  
   - Assess accuracy and cross-validation scores  
   - Compare multiple models efficiently

---

## 🧰 Libraries Used
- `pandas`  
- `numpy`  
- `scikit-learn`  
- `matplotlib`  
- `seaborn`

---

## 🎯 Key Advantages of Using Pipelines
- Simplifies ML workflow management  
- Prevents data leakage between training and testing  
- Makes model deployment easier  
- Supports hyperparameter tuning with `GridSearchCV`

---

## ✨ Author
**Gauri Kutakole**  
*Machine Learning Algorithms Repository*  
📅 Updated: October 2025
