# 📌 Encoding Categorical Data in the Titanic Dataset

## 📖 Overview
In this project, I applied **categorical data encoding techniques** to the **Titanic dataset** to convert non-numeric data into a machine-readable format.

## 🚀 Concepts Covered
- **One-Hot Encoding**: Converting categorical features into multiple binary columns.
- **Label Encoding**: Assigning numerical values to categorical labels.
- **Feature Transformation**: Preparing categorical variables for use in machine learning models.

## 📂 Project Structure
```
|-- project
    |-- README.md   # Documentation of the project
    |-- project_03.ipynb   # Python script implementing categorical encoding
```

## 📝 Steps in the Project

### 1️⃣ Import Required Libraries
- Loaded essential Python libraries including **Pandas, NumPy, and Scikit-Learn** for data manipulation and encoding.

### 2️⃣ Load the Dataset
- Imported the **Titanic dataset** from a publicly available URL.
- Displayed the first few rows to examine its structure.
- Checked data types to identify categorical variables.

### 3️⃣ Select Categorical Features for Encoding
- Chose **'Pclass'** and **'Sex'** as the categorical features for transformation.

### 4️⃣ Apply One-Hot Encoding (Independent Variables)
- Used **OneHotEncoder** from Scikit-Learn to convert categorical variables into multiple binary (0/1) columns.
- Applied **ColumnTransformer** to ensure encoding was performed correctly while retaining other features.

### 5️⃣ Apply Label Encoding (Dependent Variable)
- Used **LabelEncoder** to transform the **'Sex'** column into numerical values:
  - **Male → 1, Female → 0**
- This method is useful when dealing with ordinal or binary categorical variables.

### 6️⃣ Display Encoded Data
- Printed the **One-Hot Encoded** results for independent variables.
- Verified the **Label Encoded** values for categorical labels.

## 📌 Technologies Used
- **Python** 🐍
- **Pandas** (for data handling)
- **NumPy** (for numerical operations)
- **Scikit-Learn** (for preprocessing and encoding)

## 🎯 Next Steps
- Explore additional encoding techniques such as **Target Encoding** and **Binary Encoding**.
- Implement encoding on more complex datasets with multiple categorical variables.
- Use encoded data in a machine learning model for classification tasks.

---
🚀 **This project reinforced my understanding of categorical encoding in machine learning!**
