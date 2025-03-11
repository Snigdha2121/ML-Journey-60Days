# 📅 Day 02 - Data Preprocessing in Python

## 📖 What I Learned

### 🔹 Importing Necessary Libraries
To begin with data preprocessing, we need to import essential libraries:
- **Pandas** (`pd`) - For data manipulation and analysis.
- **NumPy** (`np`) - For numerical operations.
- **Matplotlib** (`plt`) - For data visualization.

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
```

### 🔹 Loading a Dataset
After importing the necessary libraries, the dataset is loaded using `pandas`:
```python
df = pd.read_csv("dataset.csv")
print(df.head())
```
- The `head()` function helps inspect the first few rows of the dataset.

### 🔹 Dependent vs. Independent Variables
- **Independent Variables (X):** Input features used for predictions.
- **Dependent Variable (y):** The target/output variable we aim to predict.
- The last column is typically the dependent variable.

### 🔹 Separating Independent & Dependent Variables
- Used **iloc** to extract independent (`X`) and dependent (`y`) variables.
- **Python slicing rule:** The range includes the lower bound but **excludes** the upper bound.

```python
X = df.iloc[:, :-1].values  # Selecting all columns except the last one
y = df.iloc[:, -1].values   # Selecting only the last column
```

### 🔹 Handling Missing Values
Handling missing values is crucial in data preprocessing. Several methods are available:

#### **1️⃣ Deleting Rows with Missing Values**
- If missing values are minimal in a large dataset, removing them may not significantly impact the analysis.
```python
df.dropna(inplace=True)
```

#### **2️⃣ Imputing Missing Values**
- If missing values are frequent, we replace them using a statistical measure (mean, median, or mode).
- Used **SimpleImputer** from `sklearn.impute` to replace missing values:
```python
from sklearn.impute import SimpleImputer
imputer = SimpleImputer(strategy='mean')
X[:, 1:3] = imputer.fit_transform(X[:, 1:3])
```

#### **3️⃣ Forward & Backward Filling (`fillna()`)**
- Forward filling (`ffill`) replaces missing values with the last observed value.
- Backward filling (`bfill`) replaces missing values with the next available value.
```python
df.fillna(method='ffill', inplace=True)
```

---
🚀 **Stay tuned for Day 3, where I'll continue learning about data preprocessing!** 🎯
