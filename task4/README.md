# 📉 Customer Churn Prediction System

## 📌 Project Overview

This project builds a **Machine Learning model** to predict whether a customer is likely to **leave (Churn)** or **remain** with a company. It demonstrates a complete end-to-end machine learning workflow, from data preprocessing and feature engineering to model training, evaluation, and deployment-ready model export.

The project utilizes **Scikit-learn Pipelines** and **GridSearchCV** to build and optimize classification models for customer churn prediction.

---

## 🎯 Objective

The primary objectives of this project are:

- Predict whether a customer is likely to churn.
- Perform data preprocessing and feature engineering.
- Train multiple machine learning models.
- Optimize model performance using hyperparameter tuning.
- Evaluate models using standard classification metrics.
- Export the best-performing model for future predictions.

---

## 📂 Dataset

**Dataset:** Customer Churn Dataset

The dataset contains customer information, including demographic details, account information, subscribed services, and the target variable indicating whether the customer has churned.

### Target Variable

- **Churn**
  - Yes → Customer leaves the company.
  - No → Customer remains with the company.

---

## 🛠️ Technologies Used

- Python 🐍
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn
- Joblib

---

## 🤖 Machine Learning Models

The project compares the performance of two classification algorithms:

- Logistic Regression
- Random Forest Classifier

### Model Optimization

- GridSearchCV
- Scikit-learn Pipelines
- StandardScaler
- One-Hot Encoding

---

## ⚙️ Project Workflow

### 1. Install Required Libraries

Install all required packages before running the notebook.

```bash
pip install -r requirements.txt
```

---

### 2. Load Dataset

- Loaded the customer churn dataset using **Pandas**.
- Displayed dataset information and previewed the data.

---

### 3. Data Cleaning

Data preprocessing includes:

- Checking the **TotalCharges** column.
- Converting **TotalCharges** to numeric values.
- Handling invalid entries.
- Removing missing records.

---

### 4. Feature Engineering

The following preprocessing steps are performed:

- Removed **customerID**.
- Converted **Churn** into numerical labels.
- Applied **One-Hot Encoding** to categorical features.

---

### 5. Train-Test Split

The dataset is divided into:

- **80% Training Set**
- **20% Testing Set**

using **train_test_split()**.

---

### 6. Model Training

Two machine learning models are trained:

- Logistic Regression
- Random Forest Classifier

A preprocessing pipeline applies:

- StandardScaler
- One-Hot Encoding
- Classification Model

---

### 7. Hyperparameter Tuning

The models are optimized using **GridSearchCV**, which automatically searches for the best hyperparameter combinations to improve predictive performance.

---

### 8. Model Evaluation

Performance is evaluated using:

- Accuracy Score
- Precision
- Recall
- F1-Score
- Classification Report
- Confusion Matrix

A confusion matrix heatmap is also generated for visual analysis.

---

### 9. Model Export

The best-performing pipeline is saved as:

```text
customer_churn_prediction_pipeline.joblib
```

This allows the trained model to be reused without retraining.

---

## 📊 Results

The trained machine learning pipeline successfully predicts customer churn using optimized classification models.

### Evaluation Metrics

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

---

## 🚀 Features

- End-to-End Machine Learning Pipeline
- Automated Data Preprocessing
- Feature Engineering
- Logistic Regression Model
- Random Forest Classifier
- Hyperparameter Optimization with GridSearchCV
- Confusion Matrix Visualization
- Export Trained Model with Joblib
- Deployment-Ready Prediction Pipeline

---

## 💾 Output

After successful execution, the notebook generates:

- Trained Machine Learning Pipeline
- Classification Report
- Confusion Matrix
- Model Evaluation Metrics
- Saved Model File (`customer_churn_prediction_pipeline.joblib`)

---

## 📂 Project Structure

```text
Customer_Churn_Prediction/
│
├── Customer_Churn_Code.ipynb
├── customer_churn.csv
├── customer_churn_prediction_pipeline.joblib
├── requirements.txt
├── README.md
└── images/
    └── confusion_matrix.png
```

---

## ▶️ How to Run

### 1. Clone the Repository

```bash
git clone <repository-url>
cd Customer_Churn_Prediction
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Add the Dataset

Place **customer_churn.csv** inside the project directory.

If using **Google Colab**, upload the dataset to Google Drive and update the dataset path in the notebook.

Example:

```text
/content/drive/MyDrive/customer_churn.csv
```

### 4. Open the Notebook

Launch:

```text
Customer_Churn_Code.ipynb
```

### 5. Run All Cells

Execute every notebook cell in sequence.

### 6. Saved Model

After training completes, the best model is automatically saved as:

```text
customer_churn_prediction_pipeline.joblib
```

---

## 📌 Future Improvements

- Experiment with XGBoost and LightGBM.
- Handle class imbalance using SMOTE.
- Deploy the model using Flask or FastAPI.
- Build an interactive Streamlit dashboard.
- Monitor model performance using MLflow.
- Perform feature importance analysis for better interpretability.

---

## 👨‍💻 Author

**Sharjeel Raza**

Machine Learning Project — Customer Churn Prediction System

---

## ⭐ Acknowledgements

- Scikit-learn
- Pandas
- Matplotlib
- Seaborn
- Joblib
