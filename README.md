# 🚀 Startup Funding Data Cleaning Project

This project focuses on end-to-end **data cleaning** of a real-world startup funding dataset. It involves comprehensive preprocessing of noisy, incomplete, and inconsistent data to prepare it for further analysis or machine learning tasks. The project also includes the use of simple **ML models to impute missing values** in key columns.

---

## 📌 Objectives

- Load and explore raw startup funding data.
- Systematically clean various columns such as date, startup name, industry vertical, sub-vertical, city, and investment amount.
- Correct encoding issues, remove inconsistencies, and normalize values.
- Use ML models to intelligently fill missing values in crucial fields.
- Export a clean, analysis-ready version of the dataset.

---

## 📂 Dataset Features

| Column | Description |
|--------|-------------|
| `Date` | Date of funding |
| `Startup Name` | Name of the funded startup |
| `Industry Vertical` | Sector in which the startup operates |
| `Sub Vertical` | More specific segment within the industry |
| `City` | City where the startup is located |
| `Investor Name` | Name(s) of the investor(s) |
| `Investment Type` | Type of funding (Seed, Series A, etc.) |
| `Amount (USD)` | Amount raised in USD |
| `Remarks` | Additional notes, if any |

---

## 🛠️ Key Cleaning Steps

### 🔄 Basic Cleaning
- **Renamed columns** for better readability.
- **Decoded special characters** (e.g., `\xc2\xa0`) using regex.
- **Handled null values** using different techniques.

### 🗓️ Date Column
- Converted to `datetime` type.
- Removed inconsistencies in date format.

### 🏢 Categorical Columns
- Normalized values in:
  - `Startup Name`
  - `Industry Vertical`
  - `Sub Vertical`
  - `City`
  - `Investor Name`
  - `Investment Type`

### 💡 Intelligent Imputation
- Trained simple **ML models** (e.g., decision trees or label propagation) to fill:
  - `Industry Vertical`
  - `Sub Vertical`
  - `City`

### 💰 Amount Column
- Cleaned and converted `Amount (USD)` to float type.
- Handled formats like `"Undisclosed"` and `"NaN"`.

### 📝 Remarks Column
- Removed irrelevant or blank remarks.

---

## 📈 Outcome

- A clean, consistent, and complete version of the startup funding dataset.
- Ready for:
  - EDA (Exploratory Data Analysis)
  - Business insight generation
  - Predictive modeling or dashboards

---

## 📦 Tools & Libraries

- Python 🐍
- pandas, numpy
- scikit-learn (for ML imputation)
- matplotlib / seaborn (optional for visual validation)

---

## 📁 Output

- ✅ `clean_startup_funding.csv` (cleaned dataset)
- 📝 `Startup_funding.ipynb` (this notebook)

---

## ✍️ Author

**Ankit Dutt**  
Aspiring Data Scientist | Data Cleaning Enthusiast

---

## 🧠 Future Work Ideas

- Perform **EDA** on the clean dataset to identify funding trends.
- Build a **funding prediction model** based on startup characteristics.
- Create **interactive dashboards** in Power BI or Tableau.
