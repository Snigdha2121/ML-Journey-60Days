# 📌 Handling Missing Values in the Titanic Dataset

## 📖 Overview
In this project, I handled missing values in the **Titanic dataset** using different techniques to clean and preprocess the data.

## 🚀 Concepts Covered
- **Identifying Missing Values**: Checking for null values in the dataset.
- **Data Cleaning**: Handling missing data using different imputation techniques.
- **Feature Engineering**: Preparing the dataset for further analysis or modeling.

## 📂 Project Structure
```
|-- project
    |-- README.md   # Documentation of the project
    |-- project_02.ipynb   # Python script implementing data cleaning
```

## 📝 Steps in the Project

### 1️⃣ Import Necessary Libraries
- Loaded required Python libraries including Pandas, NumPy, and Scikit-Learn.

### 2️⃣ Load the Dataset
- The **Titanic dataset** was loaded from a publicly available source.
- Displayed the first few rows to understand its structure.

### 3️⃣ Check for Missing Values
- Identified missing values in different columns of the dataset.
- Printed the count of missing values for each feature.

### 4️⃣ Separating Independent & Dependent Variables
- Defined **X** (independent variables) and **y** (dependent variable).
- Ensured proper separation for further preprocessing.

### 5️⃣ Handling Missing Values
#### 🔹 Method 1: Deleting Rows with Missing Values (if minimal)
- Removed rows with missing values when they were few and would not affect the dataset significantly.

#### 🔹 Method 2: Imputation (Replacing Missing Values with Mean)
- Used **SimpleImputer** from Scikit-Learn to replace missing values in numerical columns (**Age, Fare**) with the mean of respective columns.

#### 🔹 Method 3: Forward Fill for Categorical Data
- Used **.ffill()** (forward fill) to replace missing values in the **Embarked** column based on the previous row value.

### 6️⃣ Verify Changes
- Checked for missing values again to ensure all were handled correctly.
- Printed the updated count of missing values, which should be zero.

## 📌 Technologies Used
- **Python** 🐍
- **Pandas** (for data handling)
- **NumPy** (for numerical operations)
- **Scikit-Learn** (for preprocessing)

## 🎯 Next Steps
- Apply similar preprocessing techniques to other datasets.
- Perform feature engineering to enhance model performance.

---
🚀 **This project reinforced my understanding of handling missing data in machine learning!**
