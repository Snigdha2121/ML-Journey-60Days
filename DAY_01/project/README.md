# 📌 Feature Scaling on the Iris Dataset

## 📖 Overview
In this project, I applied **feature scaling techniques** to the **Iris dataset** to standardize the data before using it in a machine learning model. This ensures that all features contribute equally and prevents bias due to differences in scale.

## 🚀 Concepts Covered
- **Train-Test Splitting**: Dividing data into training and testing sets.
- **Feature Scaling**: Applying both **Normalization (Min-Max Scaling)** and **Standardization (Z-score Scaling)**.
- **Data Visualization**: Understanding the impact of scaling using histograms.

## 📂 Project Structure
```
|-- project
    |-- README.md   # Documentation of the project
    |-- feature_scaling.ipynb   # Python script implementing feature scaling
```

## 📝 Steps in the Project
### 1️⃣ Loading the Dataset
- The **Iris dataset** from `sklearn.datasets` was loaded into a Pandas DataFrame.
- Displayed the first few rows to understand its structure.

### 2️⃣ Splitting Data into Training & Testing Sets
- Used **80% for training** and **20% for testing**.
- Ensured the test data remains unseen during training.

### 3️⃣ Applying Feature Scaling
#### 🔹 Normalization (Min-Max Scaling)
- Rescaled features to range **[0,1]** using the formula:
  
  ```
  X' = (X - X_min) / (X_max - X_min)
  ```

#### 🔹 Standardization (Z-score Scaling)
- Rescaled data to have **mean = 0** and **standard deviation = 1** using the formula:
  
  ```
  X' = (X - μ) / σ
  ```

### 4️⃣ Comparing Normalization vs. Standardization
- **Both methods were applied and compared** to understand their effects.
- Normalization scales values within a fixed range, whereas standardization ensures a mean of 0 and unit variance.
- Both techniques were applied separately to observe their impact on data distribution.

### 5️⃣ Visualizing the Effect of Scaling
- Used histograms to compare **original, normalized, and standardized** data distributions.

## 📊 Results & Observations
- **Normalization (Min-Max Scaling)** compressed values into a small range.
- **Standardization (Z-score Scaling)** adjusted values to have a mean of **0** and unit variance.
- **Visualization** showed clear differences in how both techniques transform data.
- **Comparison** helped understand when to use each method based on the dataset characteristics.

## 📌 Technologies Used
- **Python** 🐍
- **Scikit-Learn** (for dataset and preprocessing)
- **Pandas** (for data handling)
- **Matplotlib** (for visualization)

## 🎯 Next Steps
- Apply feature scaling to a different dataset.
- Explore the effect of scaling on machine learning model performance.

---
🚀 **This project reinforced my understanding of both Normalization and Standardization in machine learning!**
