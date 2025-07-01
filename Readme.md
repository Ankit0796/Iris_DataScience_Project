# 🌸 Iris Flower Classification – Logistic Regression & EDA

This project demonstrates classification of iris flower species using **Logistic Regression**, along with **Exploratory Data Analysis (EDA)**, a rule-based model, and model tuning — all using the classic Iris dataset from scikit-learn.

---

## 📌 Problem Statement

Predict the species of an Iris flower (Setosa, Versicolor, or Virginica) based on the following features:

- Sepal length (cm)
- Sepal width (cm)
- Petal length (cm)
- Petal width (cm)

---

## 📊 Dataset Details

- **Source:** `sklearn.datasets.load_iris()`
- **Observations:** 150
- **Features:** 4
- **Target Classes:** 3 (balanced)

---

## ✅ Objectives

- Perform EDA to understand feature relationships
- Build a simple rule-based classifier
- Train a Logistic Regression model
- Evaluate using train/test split and cross-validation
- Tune hyperparameters
- Analyze misclassifications visually

---

## 🔍 Exploratory Data Analysis

- Histograms for each feature
- Pairplots showing class separability
- Scatter plots grouped by species
- Analysis of feature-to-target relationships

---

## ✅ Manual Accuracy

- Manual accuracy: **~98% on training data**

---

## 🔢 Logistic Regression Model

Trained using `LogisticRegression` from `sklearn`.

**Evaluated using:**
- ✅ Train/test split accuracy
- 🔁 10-fold Cross-validation
- 📊 Scatter plots for predicted vs actual labels

---

## 🔁 Model Tuning

- Hyperparameter `C` (inverse of regularization strength) tuned manually
- **Best performing value:** `C = 2`

---

## 🌟 Final Model Evaluation

- **Accuracy on test set:** 95%
- ✅ Visual analysis of misclassifications
- 🔍 Used plots to compare predictions with ground truth

---

## 📊 Results Summary

| Model                      | Accuracy         |
|---------------------------|------------------|
| Manual Rule-Based (Train) | ~98%             |
| Logistic Regression (CV)  | ~96%             |
| Logistic Regression (Test)| **95%**          |

---

## 🧰 Libraries Used

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`

---

## 📌 Insights

- Petal length and width are **highly predictive** features.
- Logistic Regression performs very well on **linearly separable** data like this.
- Visual EDA helps build intuition before modeling.

---

## 🧠 Future Work

- Try other models: **SVM**, **KNN**, **Decision Tree**, **XGBoost**
- Include **confusion matrix** and **classification report**
- Use dimensionality reduction techniques (**PCA**, **t-SNE**)
- Turn this into a **Streamlit** app for interactive prediction

---

## 🚀 How to Run

```bash
# 1. Clone this repository
git clone https://github.com/yourusername/iris-logistic-regression.git
cd iris-logistic-regression

# 2. Install dependencies
pip install -r requirements.txt

# 3. Launch the notebook
jupyter notebook iris_classification.ipynb
