# 🩺 Chronic Kidney Disease Prediction

This machine learning project predicts whether a patient has **Chronic Kidney Disease (CKD)** using clinical and laboratory data.  
The project is implemented using **Python** and common **data science libraries**, with the complete workflow demonstrated in a Jupyter Notebook.

---

## 📌 Project Overview

- **Problem Type:** Classification
- **Dataset Size:** 400 records, 26 features
- **Target Variable:** `classification`
- **Algorithm Used:** Random Forest Classifier
- **Environment:** Jupyter Notebook / Google Colab

---

---

## 📊 Dataset Description

The dataset contains medical attributes such as:

- Age, Blood Pressure, Specific Gravity  
- Albumin, Sugar, Blood Glucose Random  
- Blood Urea, Serum Creatinine  
- Hemoglobin, Sodium, Potassium  
- Clinical conditions like Hypertension, Diabetes, Anemia  
- **Target column:** `classification` (CKD / Not CKD)

---

## 🧹 Data Preprocessing

The following steps were performed in the notebook:

- Loaded dataset using **pandas**
- Checked shape, columns, data types, and missing values
- Handled missing values:
  - **Numerical columns:** filled with median
  - **Categorical columns:** filled with mode
- Encoded categorical features using **LabelEncoder**
- Standardized features using **StandardScaler**
- Verified data quality (no duplicates, no null values)

---

## 📈 Exploratory Data Analysis (EDA)

- Visualized class distribution using a **count plot**
- Generated a **correlation heatmap** to understand feature relationships

---

## 🤖 Model Training

- Split data into **70% training** and **30% testing**
- Trained a **Random Forest Classifier**
- Used scaled features for better performance

```python
RandomForestClassifier(random_state=42)

📏 Model Evaluation

Evaluation metrics used:
Accuracy Score
Confusion Matrix
Classification Report

Result:

Achieved very high accuracy on the test dataset
Note: High accuracy may indicate strong patterns in the data and should be validated carefully for real-world deployment.

⚙️ Requirements

Install the required dependencies using:
pip install -r requirements.txt

▶️ How to Run the Project

Clone the repository:
git clone https://github.com/guttulaswathi/kidney-disease-prediction.git


Navigate to the project folder:
cd kidney-disease-prediction


Install dependencies:

pip install -r requirements.txt
Open the notebook:
jupyter notebook
Run all cells in Chronic_Kidney_Disease_Prediction.ipynb

🧠 Key Learnings

Handling missing values is crucial in medical datasets
Feature scaling improves machine learning model performance
Random Forest performs well on structured clinical data
EDA helps understand class distribution and feature correlation

👩‍💻 Author

Guttula Swathi
Machine Learning & AI Enthusiast

🚀 Future Enhancements

Save trained model for reuse
Deploy model using Flask or Streamlit
Add cross-validation
Improve generalization and validation strategy
Modularize code into Python scripts






