# Internship-Task-1
# Task 1: Data Cleaning & Preprocessing - Titanic Dataset

This repository contains my solution for **Task 1: Data Cleaning and Preprocessing** as part of the AI & ML Internship.

## 📁 Dataset
Dataset used: [Kaggle - Titanic Dataset](https://www.kaggle.com/datasets/yasserh/titanic-dataset)

Uploaded File: `Titanic-Dataset.csv`

---

## ✅ Objective
Prepare raw Titanic dataset for use in machine learning models by performing:
- Null value handling
- Categorical encoding
- Feature scaling
- Outlier detection

---

## 🛠️ Tools Used
- Python 3
- Jupyter Notebook
- Libraries:
  - `pandas`
  - `numpy`
  - `matplotlib`
  - `seaborn`
  - `scikit-learn`

---

## 🔧 Steps Performed

### 1. Data Loading
- Loaded the dataset using `pandas.read_csv()`
- Explored structure using `.info()`, `.describe()`, and `.isnull().sum()`

### 2. Handling Missing Values
- `Age`: Filled missing values using **mean**
- `Embarked`: Filled missing using **mode**
- Dropped `Cabin` column due to too many missing values
- Dropped remaining null rows if any

### 3. Encoding Categorical Variables
- `Sex`: Binary encoding (male = 0, female = 1)
- `Embarked`: One-hot encoding (converted to multiple columns)

### 4. Feature Scaling
- Standardized `Age` and `Fare` using **`StandardScaler`** from `sklearn`

### 5. Outlier Detection (Optional)
- Used **boxplot** to visualize outliers in `Fare`
- Removed outliers above the 95th percentile (optional for cleaning)

### 6. Save Cleaned Data
- Exported final cleaned dataset to `cleaned_titanic.csv`

---

## 📄 Files Included
- `Titanic-Dataset.csv` – Original dataset
- `cleaned_titanic.csv` – Final cleaned dataset
- `titanic_cleaning.ipynb` – Jupyter notebook with full code
- `README.md` – This documentation file

---

## 📤 Submission
- [Form Link to Submit GitHub Repository](https://forms.gle/8Gm83s53KbyXs3Ne9)

---

## 🔍 Interview Questions Practice
1. What are the types of missing data?
2. Difference between label encoding and one-hot encoding?
3. Why normalize or standardize data?
4. How do you handle outliers?
5. Why is preprocessing crucial before training ML models?

---

## 🙌 Thank You!
For learning and guidance provided as part of the internship program.
