# 🤖 Auto Tagging Support Tickets Using LLM

## 📌 Project Overview

This project was developed as part of the **DevelopersHub Corporation AI/ML Engineering Advanced Internship – Task 5**.

The objective is to automatically classify IT support tickets into the appropriate department and generate the **top 3 relevant tags** using a **Large Language Model (LLM)**. The project compares **Zero-Shot Prompting** and **Few-Shot Prompting** techniques to evaluate the effectiveness of prompt engineering for text classification.

---

## 🎯 Objective

The primary goals of this project are:

- Automatically classify support tickets into the correct department.
- Generate the top 3 most relevant tags for each ticket.
- Compare Zero-Shot and Few-Shot prompting approaches.
- Evaluate classification performance using machine learning metrics.

---

## 📂 Dataset

**Dataset:** IT Support Ticket Data

The dataset contains real-world IT support tickets with the following columns:

- **Body** (Support Ticket Description)
- **Department** (Target Label)
- **Priority**
- **Tags**

The **Department** column is used as the ground-truth label for evaluating model performance.

---

## 🛠️ Technologies Used

- Python 🐍
- Google Colab
- OpenAI API
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn

---

## 🤖 Large Language Model

### Model Used

- **GPT-4.1-mini**

### Prompting Techniques

- Zero-Shot Prompting
- Few-Shot Prompting

---

## ⚙️ Project Workflow

### 1. Data Loading

- Loaded the IT Support Ticket dataset.
- Explored the dataset structure.
- Checked for missing values.

### 2. Data Preprocessing

- Selected the required columns.
- Sampled a subset of support tickets for API-based evaluation.
- Cleaned and standardized prediction outputs before evaluation.

### 3. Zero-Shot Classification

The model classified support tickets without being provided any examples.

**Generated Output:**

- Predicted Department
- Top 3 Relevant Tags

### 4. Few-Shot Classification

The model classified support tickets after being provided with representative examples.

**Generated Output:**

- Predicted Department
- Top 3 Relevant Tags

### 5. Performance Evaluation

Predicted departments were compared with the ground-truth labels using:

- Accuracy
- Classification Report
- Confusion Matrix

---

## 📊 Results

The Large Language Model successfully classified support tickets and generated relevant tags using prompt engineering.

### Observed Performance

| Prompting Technique | Accuracy |
|--------------------|----------:|
| Zero-Shot | **25%** |
| Few-Shot | **25%** |

> **Note:** The reported accuracy is based on the evaluated sample. Performance may vary depending on the dataset quality, prompt design, sample size, and category overlap.

---

## 📈 Evaluation Metrics

The project evaluates performance using:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

---

## 🚀 Features

- LLM-based Support Ticket Classification
- Zero-Shot Prompting
- Few-Shot Prompting
- Automatic Department Prediction
- Top 3 Tag Generation
- Performance Evaluation
- Export Predictions to CSV
- Confusion Matrix Visualization

---

## 💾 Output

The notebook generates:

- Department Predictions
- Top 3 Generated Tags
- Prediction CSV File
- Evaluation Metrics
- Performance Visualizations

---

## 📂 Project Structure

```text
Task-5-Auto-Tagging-LLM/
│
├── Task5_Auto_Tagging.ipynb
├── IT Support Ticket Data.csv
├── predictions.csv
├── requirements.txt
├── README.md
└── images/
    ├── confusion_matrix.png
    └── accuracy_comparison.png
```

---

## 📌 Future Improvements

- Improve prompt engineering with more representative examples.
- Evaluate additional Large Language Models.
- Fine-tune an open-source language model for improved accuracy.
- Build a Streamlit web application for real-time ticket classification.
- Implement Retrieval-Augmented Generation (RAG) for knowledge-aware ticket routing.

---

## 🎓 Internship Task

**DevelopersHub Corporation**

**AI/ML Engineering Advanced Internship**

**Task 5 – Auto Tagging Support Tickets Using LLM**

---

## 👨‍💻 Author

**Sharjeel Raza**

AI/ML Engineering Advanced Internship — DevelopersHub Corporation

---

## ⭐ Acknowledgements

- OpenAI
- Google Colab
- Scikit-learn
- Pandas
- Matplotlib
- Seaborn
- DevelopersHub Corporation
