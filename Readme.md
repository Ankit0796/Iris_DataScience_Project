# 🌸 Iris Flower Classification – Logistic Regression & EDA

This project demonstrates classification of iris flower species using **Logistic Regression**, along with **Exploratory Data Analysis (EDA)**, a rule-based model, and model tuning — all using the classic Iris dataset from scikit-learn.

---

## 📌 Problem Statement

Predict the species of an Iris flower (Setosa, Versicolor, or Virginica) based on the following features:
---

## 📊 Dataset Details

## 🌸 Iris Plants Dataset

## 📊 Data Set Characteristics

- **Number of Instances:** 150 (50 in each of the three classes)
- **Number of Attributes:** 4 numeric, predictive attributes and 1 target class
- **Missing Values:** None
- **Class Distribution:** 33.3% for each class
- **Creator:** R.A. Fisher  
- **Donor:** Michael Marshall (MARSHALL%PLU@io.arc.nasa.gov)  
- **Date:** July, 1988

---

## 🌿 Attribute Information

1. Sepal length in cm  
2. Sepal width in cm  
3. Petal length in cm  
4. Petal width in cm  
5. Class:
   - *Iris-setosa*
   - *Iris-versicolour*
   - *Iris-virginica*

---

## 📈 Summary Statistics

| Attribute      | Min | Max | Mean | Std Dev | Class Correlation |
|----------------|-----|-----|------|---------|--------------------|
| Sepal Length   | 4.3 | 7.9 | 5.84 | 0.83    | 0.7826             |
| Sepal Width    | 2.0 | 4.4 | 3.05 | 0.43    | -0.4194            |
| Petal Length   | 1.0 | 6.9 | 3.76 | 1.76    | 0.9490 *(high!)*   |
| Petal Width    | 0.1 | 2.5 | 1.20 | 0.76    | 0.9565 *(high!)*   |

---

## 📚 Background

This is perhaps the most well-known dataset in pattern recognition. First introduced by **Sir R.A. Fisher** in 1936, it has since become a standard for testing classification algorithms.

- The dataset contains 3 classes of 50 instances each.
- One class (*Iris-setosa*) is linearly separable from the other two.
- The other two classes (*Iris-versicolour* and *Iris-virginica*) are **not** linearly separable from each other.

Note: This version of the dataset is taken directly from Fisher's paper and matches the one in R. The UCI ML Repository version contains two incorrect data points.

---

## 📚 References

- Fisher, R.A. *The use of multiple measurements in taxonomic problems*.  
  Annual Eugenics, 7, Part II, 179–188 (1936); also in *Contributions to Mathematical Statistics*, John Wiley, NY, 1950.

- Duda, R.O., & Hart, P.E. (1973). *Pattern Classification and Scene Analysis*, John Wiley & Sons. ISBN: 0-471-22361-1. See page 218.

- Dasarathy, B.V. (1980). *Nosing Around the Neighborhood: A New System Structure and Classification Rule for Recognition in Partially Exposed Environments*. IEEE Transactions on Pattern Analysis and Machine Intelligence, Vol. PAMI-2, No. 1, 67–71.

- Gates, G.W. (1972). *The Reduced Nearest Neighbor Rule*. IEEE Transactions on Information Theory, May 1972, 431–433.

- Cheeseman et al. *AUTOCLASS II conceptual clustering system* (1988 MLC Proceedings, 54–64).

![Image](https://github.com/user-attachments/assets/cc0f0a6c-29c9-4d47-b175-53456789aa75)
- 
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

![Image](https://github.com/user-attachments/assets/17e883c3-88dc-489c-8032-c15dc4eb33f7)
![Image](https://github.com/user-attachments/assets/b6965834-8e3f-4b8f-88f9-4ad8d07b577d)
![Image](https://github.com/user-attachments/assets/d9ab66a2-2ff9-4804-8362-a780ac334f74)
![Image](https://github.com/user-attachments/assets/a0ceb170-f02e-416a-94df-ccdbdc35dea3)
- Pairplots showing class separability

![Image](https://github.com/user-attachments/assets/a6b241fc-df01-4af4-8202-8b71a537c819)
- Scatter plots grouped by species
- Analysis of feature-to-target relationships

---

## ✅ Manual Accuracy

![Image](https://github.com/user-attachments/assets/79daf451-8a9f-4dbe-bde2-498fff4183cc)

- Manual accuracy: **~96% on training data**

---

## 🔢 Logistic Regression Model

Trained using `LogisticRegression` from `sklearn`.

**Evaluated using:**
- ✅ Train/test split accuracy
- 🔁 10-fold Cross-validation
- 📊 Scatter plots for predicted vs actual labels

![Image](https://github.com/user-attachments/assets/753db0b0-bbd7-4fdc-b9a9-4b6c87e49fb0)
---

## 🔁 Model Tuning

- Hyperparameter `C` (inverse of regularization strength) tuned manually
- **Best performing value:** `C = 2`

![Image](https://github.com/user-attachments/assets/e278f474-d688-4d3f-bf45-930476d958af)

![Image](https://github.com/user-attachments/assets/09d56979-ab53-449d-8a9d-f80120eaf5e4)
---

## 🌟 Final Model Evaluation

- **Accuracy on test set:** 95%
- ✅ Visual analysis of misclassifications
- 🔍 Used plots to compare predictions with ground truth

---

## 📊 Results Summary

| Model                      | Accuracy         |
|---------------------------|------------------|
| Manual Rule-Based (Train) | ~95%             |
| Logistic Regression (CV)  | ~96%             |
| Logistic Regression (Tuning)| **95%**          |

---

## 🧰 Libraries Used

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`

![Image](https://github.com/user-attachments/assets/9c2f1e74-04f3-45e1-9b69-74e01a2f9f59)

---

## 📌 Insights

- Petal length and width are **highly predictive** features.
- Logistic Regression performs very well on **linearly separable** data like this.
- Visual EDA helps build intuition before modeling.

---

