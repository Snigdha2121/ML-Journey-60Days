# 📅 Day 03 - Encoding Categorical Data  

## 📖 What I Learned  

### 🔹 Why Encode Categorical Data?  
Machine learning models only understand numerical data, but real-world datasets often contain categorical variables like gender, country, or yes/no responses. Encoding is necessary to convert these categories into numerical values so that models can process them effectively.  

### 🔹 Types of Encoding  

#### **1️⃣ One-Hot Encoding (For Independent Variables)**  
- Used when a categorical variable has **no inherent order** (e.g., colors, countries, product types).  
- Creates multiple binary columns, where each category is represented as either 0 or 1.  
- Prevents models from assuming any ranking or hierarchy between categories.  

#### **2️⃣ Label Encoding (For Dependent Variables)**  
- Converts categorical values into numeric labels (e.g., "Yes" → 1, "No" → 0).  
- Works well when the categories have a **logical order** (e.g., "Low" < "Medium" < "High").  
- Can introduce unintended biases if applied to unordered categories.  

### 🔹 Key Takeaways  
- Encoding is essential to prepare categorical data for machine learning models.  
- **One-Hot Encoding** is best for unordered categorical variables to avoid misinterpretation.  
- **Label Encoding** is useful for ordinal data but should be used carefully to prevent misleading relationships.  
- Choosing the correct encoding technique is crucial for ensuring accurate model predictions.  

---

🚀 See you on Day 4! 🎯  
