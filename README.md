# 🎓 Student Academic Performance Prediction using Machine Learning

This project focuses on predicting student academic performance based on multiple behavioral and academic factors using supervised machine learning algorithms.  
By leveraging data preprocessing, feature engineering, and model evaluation, this project identifies the key variables that influence student success and builds accurate prediction models.

> 📘 Developed by Monika Damelia Hutapea 

---

## 📁 Project Overview
The dataset contains information about students’ academic backgrounds, study behaviors, and other factors such as:
- **Gender**, **High School Type**, **Scholarship**, **Attendance**, **Weekly Study Hours**, and **Additional Activities**  
- The **target variable** is `Grade` — representing whether a student’s performance is classified as “Pass” or “Fail”.

The goal of this project is to **analyze patterns** influencing academic outcomes and **build predictive models** that can support early intervention strategies for students at risk of underperforming.

---

## 🧩 Objectives
- Perform **data cleaning and preprocessing** to ensure data quality.  
- Conduct **exploratory data analysis (EDA)** to understand variable relationships.  
- Implement machine learning algorithms (**Random Forest**, **KNN**) for classification.  
- Evaluate model performance using accuracy, precision, recall, and F1-score metrics.  
- Derive insights about the key factors influencing student performance.

---

## 🛠️ Tools & Libraries
- **Python 3.8+**
- **Pandas**, **NumPy**
- **Matplotlib**, **Seaborn**
- **Scikit-learn**
- **Feature-engine**
- **Jupyter Notebook / Google Colab**

---

## ⚙️ Workflow

### 1️⃣ Data Preprocessing
- Handle missing values using `SimpleImputer` (most_frequent strategy).  
- Encode categorical variables using:
  - `OrdinalEncoder` for ordered variables (e.g., Attendance, School Type).  
  - `LabelEncoder` for binary/categorical features (e.g., Additional Work, Scholarship).  
- Handle outliers using `Winsorizer` from `feature-engine`.  
- Normalize numerical features for model compatibility.

### 2️⃣ Exploratory Data Analysis (EDA)
- Visualize data distribution with histograms and countplots.  
- Generate correlation heatmap to identify influential variables.  
- Detect imbalance between pass/fail classes.

### 3️⃣ Model Building
- **Train-test split:** 80% training, 20% testing.  
- Build and train models:
  - **Random Forest Classifier**
  - **K-Nearest Neighbors (KNN)**  
- Perform **hyperparameter tuning** using `GridSearchCV` for Random Forest.

### 4️⃣ Model Evaluation
- Use the following metrics:
  - Accuracy  
  - Precision  
  - Recall  
  - F1-score  
- Visualize results with confusion matrices and classification reports.

---

## 📈 Results

### 🔹 Model Performance Summary

| Model | Accuracy | Precision | Recall | F1-score |
|:------|:---------:|:----------:|:-------:|:---------:|
| **Random Forest** | **86.21%** | 0.86 | **1.00** | 0.93 |
| **KNN (k=3)** | **86.21%** | 0.86 | **1.00** | 0.93 |

✅ Both **Random Forest** and **KNN** achieved strong predictive performance, with identical accuracy of **86.21%**.  
Random Forest provided higher interpretability and stability, while KNN performed well for smaller feature spaces.

---

## 💡 Key Insights
- **Attendance**, **Study Hours**, and **Additional Work** show strong correlation with higher grades.  
- Students who engage in regular study hours and maintain good attendance tend to perform significantly better.  
- Scholarship recipients and those with extracurricular activities maintain consistent academic performance.  
- Data imbalance affects recall for minority class (“Fail”), which could be improved with oversampling (e.g., SMOTE).

---

## 📊 Visualization Highlights
- **Correlation Heatmap:** Identifies key contributing factors to grade performance.  
- **Boxplots:** Show data distribution and outliers before/after Winsorization.  
- **Confusion Matrix:** Displays model prediction performance.  

---

